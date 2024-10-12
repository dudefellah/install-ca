# GitHub Action for Installing a Custom CA

## Usage

Example Workflow Usage

```yaml
- name: Install My CA
  uses: dudefellah/install-ca@v1
  with:
    cert: ${{ env.MY_CERTIFICATE_AUTHORITY }}
    name: myca

- name: Check out your collection repository
  uses: actions/checkout@v4

- name: Do some other junk...
```

## Options

The follow options can be provided to this GitHub Action.

### `certificate_authority`

This is the contents of your certificate authority file in PEM format.

### `name`

A name to provide for your cert.  This is mostly meaningless, but will inform the name of the path and file written.

## License

This action is primarily licensed and distributed as a whole under the GNU General Public License v3.0 or later.

See [LICENSES/GPL-3.0-or-later.txt](https://github.com/ansible-community/github-action-build-collection/blob/main/COPYING) for the full text.

All files have a machine readable `SDPX-License-Identifier:` comment denoting its respective license(s) or an equivalent entry in an accompanying `.license` file. This conforms to the [REUSE specification](https://reuse.software/spec/).
