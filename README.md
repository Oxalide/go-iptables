# go-iptables

[![GoDoc](https://godoc.org/github.com/jeremmfr/go-iptables/iptables?status.svg)](https://godoc.org/github.com/jeremmfr/go-iptables/iptables)
[![Build Status](https://github.com/jeremmfr/go-iptables/workflows/Go%20Tests/badge.svg)](https://github.com/jeremmfr/go-iptables/actions)

Go bindings for iptables utility.

In-kernel netfilter does not have a good userspace API. The tables are manipulated via setsockopt that sets/replaces the entire table. Changes to existing table need to be resolved by userspace code which is difficult and error-prone. Netfilter developers heavily advocate using iptables utlity for programmatic manipulation.

go-iptables wraps invocation of iptables utility with functions to append and delete rules; create, clear and delete chains.
