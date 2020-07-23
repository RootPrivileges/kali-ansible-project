# kali-ansible-project

## Background

The (one day soon!) one-stop repository for automatically deploying a mission-ready Kali installation, regardless of whether it's in a virtual machine, cloud image or bare metal! The Kali Ansible Project is intended to be the DevOps toolkit to create a Gold-Master installation of everyone's favourite hacking distribution with all of the tools needed for a variety of jobs.

This repository will be the result of the conversion of my (in)famous bash script, built up over the last decade, to create the Kali image I daily use for penetration testing. It's taken inspiration from a lot of places (such as [g0tmi1k's build scripts, all the way back to Backtrack](https://github.com/g0tmi1k/os-scripts/)) with a healthy dose of the extra tools I've needed throughout my career (where they still exist!).

On top of applications straight from the Kali package repositories, there's going to be a number of fixes to scripts and code repositories being cloned left, right and centre!

Eventually (once this gets nearer completion), I'll add Packer configs to build pre-made images to download and a bash script to curl which will allow the deployment to happen on local installations too - you won't be just limited to Vagrant and VirtualBox!

## Prerequisites

### Vagrant

- Virtualbox >= 6.1.0 (necessary to have the VM start on boot with working graphics)

## Commands

### Vagrant

#### Start kali VM

```
vagrant up
```

#### Stop kali VM

```
vagrant halt
```

#### Re-run provisioning on kali VM

```
vagrant provision
```

#### Completely remove kali VM

```
vagrant destroy
```

#### Update underlying kalilinux/rolling image

```
vagrant box update
```
