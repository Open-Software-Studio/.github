# .github

The organisation's profile — what renders on
[github.com/Open-Software-Studio](https://github.com/Open-Software-Studio).

GitHub reads an org profile from exactly one place: `profile/` in a repository
named `.github`. There is no setting and no alternative path.

## These files are copies

`profile/README.md` and `profile/banner.svg` come from
**[branding](https://github.com/Open-Software-Studio/branding) → `org/profile/`**,
which is the source. The banner is generated there from the same tokens as the
mark, so it cannot show a wordmark the studio has moved on from. Edit it there.

## Syncing

```bash
cp ../branding/org/profile/README.md profile/README.md
cp ../branding/org/profile/banner.svg profile/banner.svg
git commit -am "profile: sync from branding" && git push
```

## One caveat

GitHub shows this profile to the public only while **this repository is public**.
It is private for now, matching the rest of the organisation; editing it here
does not make the profile readable from outside until that flips.
