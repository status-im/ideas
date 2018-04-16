## Preamble

    Idea: 143
    Title: Seamless Login
    Status: Draft
    Created: 2018-05-04


## Summary

When a user opens Status or taps on a push notification they should be able to start using the app securely, quickly and without any interruptions.

## Swarm Participants
- Lead Contributor: @alwx
- Testing & Evaluation: @asemiankevich
- PM: @chadyj
- UX: @andmironov
- UXR: @jpbowen @hesterbruikman


## Product Overview

Status frequently logs out users when the app is in the background and forces users to log in again when opening the app. Being repeatedly and unexpectedly logged out has led to frustration and complaints (see Instabug and internal reports) which negatively impact the user experience and potentially contributes to churn. Also, users are encouraged to have complex passwords but this can be cumbersome to enter.

By reducing friction around the critical point of returning to the app users can spend more time in Status which will help DAU and retention (Q2 OKR).

This idea seeks to make logging in seamless through both technical and UX methods.


### Product Description

The Status login process should smooth as possible, and this can be achieved with the (optional) use of device security features such as Touch ID or a pin code. In addition to the password prompt, a user can use choose to securely use their fingerprint. This will be set up during onboarding and toggled in settings.

Note, all transactions require authentication, so even if the phone was lost or stolen a third party couldn’t transfer funds. This idea does not cover the transaction flow.

For future iterations, this swarm will research the security implications and explore enhancements around logging in, logging out, and recovering from crashes.

### Security and Privacy Implications

todo: Alwx

### Iteration 1

Research security, technical, and UX implications of adding TouchID-like features in addition to the password.

### Iteration 2

During onboarding give users the option to setup seamless authentication (if their device supports it) and use the device/OS conventions to enable, or skip. There will be a setting to manage this preference.

## Iteration 3

Research crashes, logouts, and other related issues in Status. Some exploration has started [here#2869](https://github.com/status-im/status-react/issues/2869#issuecomment-376098196).

Propose fixes that improve both security and usability.

## Iteration 4

Implement improves from iteration 3.


## Success Metrics

- UXR validates workflow on real devices with real users
- 90% of surveyed users are satisfied with loggging in
- 0 password related issues in Instabug


## Exit criteria

When iterations 1-4 are complete the success metrics should be evaluated. If the results are successful this swarm can be closed. If work is needed an additional iteration can be done to address shortcomings.

## Supporting Role Communication

- Core
- Marketing
- Test team

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).