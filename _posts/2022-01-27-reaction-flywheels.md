---
layout: post
author: perry
title: Reaction Flywheels
description: And a whole lotta math
summary: The math behind omega, MOI, and angular displacement for reaction whee;s
tags: [math, space]
date: 2022-01-27 19:12:24 -0800
usemathjax: true
---
# Reaction Wheels

$$ I_s $$ is the moment of inertia (MOI) of the spacecraft

$$ \omega_s $$ is the desired angular velocity of the spacecraft

$$ \omega_m $$ is the maximum angular velocity the motor can produce

$$ I_f $$ is the necessary flywheel MOI

We start by calculating the inertial-frame flywheel angular velocity,
which slightly differs from the motor's as the stator is mounted to a
spacecraft

$$ \omega_f = \omega_m - \omega_s $$

We then apply this to the conservation of angular momentum

$$ \omega_f I_f = \omega_s I_s $$

$$ (\omega_m - \omega_s) I_f = \omega_s I_s $$

$$ I_f = \frac{\omega_s I_s}{\omega_m - \omega_s} $$

To obtain the necessary flywheel moment of inertia to achieve the desired
spacecraft angular velocity.

Note that this is independent of the maximum output torque of the motor,
only the maximum angular velocity, as a lower torque will only reduce the
angular acceleration and not the final angular velocity.