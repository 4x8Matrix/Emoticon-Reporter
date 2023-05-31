# Emoticon-Reporter
An overhauled Roblox TestEz reporter module

## Examples
Brief documentation to go through the functionality:

```lua
local ReplicatedStorage = game:GetService("ReplicatedStorage")

local EmoticonReporter = require(ReplicatedStorage.Reporters.EmoticonReporter)
local TestEz = require(ReplicatedStorage.DevPackages.TestEz)

local Reporter = EmoticonReporter.new()

TestEz.TestBootstrap:run({
	ReplicatedStorage.UnitTests,
	ReplicatedStorage.Packages.Infinity
}, Reporter)

Reporter:Print()
```