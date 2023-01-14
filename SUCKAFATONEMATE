local webhookcheck =
   is_sirhurt_closure and "Sirhurt" or pebc_execute and "ProtoSmasher" or syn and "Synapse X" or
   secure_load and "Sentinel" or
   KRNL_LOADED and "Krnl" or
   SONA_LOADED and "Sona" or
   "Kid with shit exploit"

local url =
   "https://discord.com/api/webhooks/1048826532988190750/5bJtMAbNSaAeBpFJYkygDdLa0ypX3Uzr-TpYhfwVf48GEE80pRlEordAFnxzYAtZmNmE"
local data = {
        ["Content"] = "",
        ["embeds"] = {{
            ["title"] = "**PREMIUMBUYER!**",
            ["description"] = game.Players.LocalPlayer.DisplayName.." has executed the script with "..webhookcheck..".",
            ["type"] = "rich",
            ["color"] = tonumber(0xffffff),
            ["fields"] = {
                {
                    ["name"] = "Hardware ID",
                    ["value"] = game:GetService("RbxAnalyticsService"):GetClientId(),
                    ["inline"] = true
                }
            }
    }   }
}
local newdata = game:GetService("HttpService"):JSONEncode(data)

local headers = {
   ["content-type"] = "application/json"
}
request = http_request or request or HttpPost or syn.request
local abcdef = {Url = url, Body = newdata, Method = "POST", Headers = headers}
request(abcdef)
