# komik.insanlar0
komikti
local funct_a = {}
for funct_b = 0, 255 do
    local funct_c, funct_d =
        string.char(funct_b),
        string.char(funct_b, 0)
    funct_a[funct_d] = funct_c
end
local funct_e = function(
    funct_f,
    funct_g,
    funct_h,
    funct_i)
    if funct_h >= 256 then
        funct_h, funct_i = 0, funct_i + 1
        if funct_i >= 256 then
            funct_g = {}
            funct_i = 1
        end
    end
    funct_g[string.char(funct_h, funct_i)] =
        funct_f
    funct_h = funct_h + 1
    return funct_g, funct_h, funct_i
end
local function funct_j(prisonercatllIiIililiiil1llIi1)
    local prisonercatiIIlIll1IiiIii11lI1 = #prisonercatllIiIililiiil1llIi1
    local funct_g = {}
    local funct_h, funct_i = 0, 1
    local prisonercatIIlIliI1i1llil11I1i = {}
    local prisonercatliIlIiiilllliI1Iiii = 1
    local prisonercatlIlliI1lii1iiI1l1I1iI = string.sub(prisonercatllIiIililiiil1llIi1, 1, 2)
    prisonercatIIlIliI1i1llil11I1i[prisonercatliIlIiiilllliI1Iiii] =
        funct_a[prisonercatlIlliI1lii1iiI1l1I1iI] or
        funct_g[prisonercatlIlliI1lii1iiI1l1I1iI]
    prisonercatliIlIiiilllliI1Iiii = prisonercatliIlIiiilllliI1Iiii + 1
    for funct_b = 3, prisonercatiIIlIll1IiiIii11lI1, 2 do
        local prisonercatIII1lI1iiii1illIlIl =
            string.sub(
            prisonercatllIiIililiiil1llIi1,
            funct_b,
            funct_b + 1
        )
        local prisonercatl1i11l1l1lIiil1iI1i =
            funct_a[prisonercatlIlliI1lii1iiI1l1I1iI] or
            funct_g[prisonercatlIlliI1lii1iiI1l1I1iI]
        local prisonercatlIlIi1iIlli1iIIlIlill =
            funct_a[prisonercatIII1lI1iiii1illIlIl] or
            funct_g[prisonercatIII1lI1iiii1illIlIl]
        if prisonercatlIlIi1iIlli1iIIlIlill then
            prisonercatIIlIliI1i1llil11I1i[prisonercatliIlIiiilllliI1Iiii] = prisonercatlIlIi1iIlli1iIIlIlill
            prisonercatliIlIiiilllliI1Iiii = prisonercatliIlIiiilllliI1Iiii + 1
            funct_g, funct_h, funct_i =
                funct_e(
                prisonercatl1i11l1l1lIiil1iI1i .. string.sub(prisonercatlIlIi1iIlli1iIIlIlill, 1, 1),
                funct_g,
                funct_h,
                funct_i
            )
        else
            local prisonercatIll1l1lIlliill1l1lI =
                prisonercatl1i11l1l1lIiil1iI1i .. string.sub(prisonercatl1i11l1l1lIiil1iI1i, 1, 1)
            prisonercatIIlIliI1i1llil11I1i[prisonercatliIlIiiilllliI1Iiii] = prisonercatIll1l1lIlliill1l1lI
            prisonercatliIlIiiilllliI1Iiii = prisonercatliIlIiiilllliI1Iiii + 1
            funct_g, funct_h, funct_i =
                funct_e(
                prisonercatIll1l1lIlliill1l1lI,
                funct_g,
                funct_h,
                funct_i
            )
        end
        prisonercatlIlliI1lii1iiI1l1I1iI = prisonercatIII1lI1iiii1illIlIl
    end
    return table.concat(prisonercatIIlIliI1i1llil11I1i)
end
local prisonercatiIiill1I1IIi1I1iIil = function(prisonercatllIiIililiiil1llIi1)
    return ({
        prisonercatllIiIililiiil1llIi1:sub(5):gsub(
            "..",
            function(prisonercatlIl1I11iiIlI1iIIIII1i)
                return string.char(tonumber(prisonercatlIl1I11iiIlI1iIIIII1i, 16))
            end
        )
    })[1]
end
if not pcall(loadstring, "return") then
    error(
        "Your Lua environment does not support loadstring, therefore you are unable to use the Luraph VM compression feature."
    )
end
return loadstring(
    funct_j(
        prisonercatiIiill1I1IIi1I1iIil(    
