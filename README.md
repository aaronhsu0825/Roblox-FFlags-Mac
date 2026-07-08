# Roblox FFlags Mac

Simple Roblox FFlag examples and setup guide for Mac without bootstrapper tools.

## What this repo is

This repo shows how to add Roblox FFlags on Mac by using a `ClientAppSettings.json` file.

The grey sky FFlag is only used as an example.

## Example: Grey Sky

The example file is here:

```text
examples/grey-sky.json
```

It contains:

```json
{
  "FFlagDebugSkyGray": "True"
}
```

## How to use it on Mac

Open **Terminal** and paste this:

```bash
mkdir -p ~/Library/Preferences/Roblox/ClientSettings

cat > ~/Library/Preferences/Roblox/ClientSettings/ClientAppSettings.json <<'EOF'
{
  "FFlagDebugSkyGray": "True"
}
EOF
```

Then fully quit Roblox and reopen it.

## How to check if it worked

Run this:

```bash
cat ~/Library/Preferences/Roblox/ClientSettings/ClientAppSettings.json
```

You should see:

```json
{
  "FFlagDebugSkyGray": "True"
}
```

## How to remove it

Run this:

```bash
rm ~/Library/Preferences/Roblox/ClientSettings/ClientAppSettings.json
```

Then fully quit Roblox and reopen it.

## Notes

Some FFlags may stop working if Roblox changes them.
This repo is for learning and examples.
