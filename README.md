local Rayfield = loadstring(game:HttpGet('https://[Log in to view URL]'))()

local Window = Rayfield:CreateWindow({
   Name = "modded_scripts",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "Made by tubergamer000",
   LoadingSubtitle = "Quality Ahead",
   Theme = "Dark Blue", -- Check https://[Log in to view URL]

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Big Hub"
   },

   Discord = {
      Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = false, -- Set this to true to use our key system
   KeySettings = {
      Title = "tubergamer key ",
      Subtitle = "Key System",
      Note = "script beta muito bom key (beta_V3)", -- Use this to tell the user how to get a key
      FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"beta_V3"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local MainTab = Window:CreateTab("Main", 4483362458) -- Title, Image
local MainSection = MainTab:CreateSection("dupe luck")

local Button = MainTab:CreateButton({
   Name = "Inf Luck",
   Callback = function()
   local args = {
    [1] = "GetReward",
    [2] = "PassReward",
    [3] = 5,
    [4] = false
}

while true do
    game:GetService("ReplicatedStorage"):WaitForChild("Remote"):WaitForChild("RemoteEvent"):FireServer(unpack(args))
    wait(end0) -- Adjust the delay time as needed (in seconds)
            end
   end,
})
local Button = MainTab:CreateButton({
   Name = "Use Luck(keep always on)",
   Callback = function()
   local args = {
    [1] = "DrawCard"
}
