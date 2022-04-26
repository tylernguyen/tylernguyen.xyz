## Threat Model

## 1Password

!!! recommendation

    ![1Password](/assets/img/uses-this/banners/1Password-light.svg#only-light){ align=right }
    ![1Password](/assets/img/uses-this/banners/1Password-dark.svg#only-dark){ align=right }

    1Password is my preferred password manager. It also manages any OTP multi-factor authentication I need.

    [Visit 1password.com](https://1password.com/){ .md-button .md-button--primary } [1Password White Paper](https://1passwordstatic.com/files/security/1password-white-paper.pdf){ .md-button }

!!! warning

    1Password is not open source.

## Yubikey

!!! recommendation

    ![YubiKeys](/assets/img/uses-this/icons/Yubikey.png){ align=right }

    Yubikey supports the most security protocols. It is also widely supported by the industry and security conscious community.

    [Visit yubico.com](https://www.yubico.com){ .md-button .md-button--primary } [Privacy Policy](https://www.yubico.com/support/terms-conditions/privacy-notice){ .md-button }

!!! warning

    Yubikey's firmware is not open source and cannot be updated without purchasing a new key.

!!! note

    The following OPSEC workflow is designed around 1Password and Yubikey. Your experience may vary with other password managers and hardware tokens.

## GPG Encryption, and SSH

[/drduh/YubiKey-Guide](https://github.com/drduh/YubiKey-Guide) is a solid, up-to-date, and comprehensive setup guide. Even Yubico's official docs often do not go into as much details as this Git repository.

I follow this repository when setting up GPG and SSH authetnication with the Yubikey.

### 1Password for SSH

1Password recently released their own [SSH agent](https://developer.1password.com/docs/ssh). This can be useful if there is a need for multiple SSH keys across different access and services. 
