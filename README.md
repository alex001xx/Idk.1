-- Kaiser Hub: versi贸n reconstruida y editable para sintaxis Lua 5.1 / Luau.
-- Verificaci贸n: compilador Luau; arranque simulado de ambas interfaces comparado con el original.
-- Pantalla de claves: 140 objetos y 292 operaciones. Interfaz principal: 845 objetos y 2.186 operaciones.
-- No se ha probado dentro de Roblox ni en un ejecutor espec铆fico.
-- No usa goto ni etiquetas de Lua 5.2. Las cadenas ya est谩n descifradas.
-- main inicia la interfaz sin el control de integridad a帽adido por el ofuscador.
-- main_integrity_bootstrap conserva ese control como referencia y no se ejecuta al iniciar.
-- La validaci贸n de claves del programa se conserva en verify_access_key.
-- Los nombres originales de variables no son recuperables; captures conserva las referencias compartidas.
-- Las regiones de flujo no estructuradas utilizan pasos expl铆citos con nombres, sin c贸digo cifrado.
local unpack_values = table.unpack or unpack
local function pack_values(...)
    return {n = select("#", ...), ...}
end
local runtime_env = (getfenv and getfenv()) or _ENV or _G
local function bind(callback, captures)
    return function(...)
        return callback(captures, {...})
    end
end
local callbacks = {}

-- main_integrity_bootstrap; bloques originales: 62
-- Comprobaci贸n del ofuscador conservada para inspecci贸n; no es el punto de entrada editable.
callbacks.main_integrity_bootstrap = function(captures, arguments)
    local A, B, D, Eh, F, G, Hh, I, J, K, M, O, P, Q, R, W, Zh, a, branch_result, ch, g, hh, ih, kh, l, m, n, o, q, u, w, x, y, z
    local e7 = {}
    do
        local temp_1
        temp_1 = {}
        temp_1.value = "GCk1x4aKpbKFD1c"
        B, l = temp_1, -1
    end
    while true do
        do
            local temp_1
            temp_1 = (1 + l)
            branch_result = ((false and (temp_1 >= 1)) or ((not false) and (temp_1 <= 1)))
            l = temp_1
        end
        if (not branch_result) then
            do
                local temp_1, temp_3, temp_4, temp_5, temp_9
                temp_1 = {}
                B.value = true
                temp_3 = string.gmatch
                temp_4 = {}
                temp_5 = {}
                temp_5.value = temp_3
                temp_4.value = bind(callbacks.callback_96, {})
                temp_1.value = false
                temp_9 = pcall(bind(callbacks.callback_97, {temp_1}))
                branch_result = temp_9
                I, l, o, u = temp_9, temp_5, temp_1, temp_4
            end
            if branch_result then
                I = o.value
            end
            do
                local temp_1, temp_2
                temp_1 = math.random
                temp_2 = {}
                temp_2.value = temp_1
                branch_result = table
                A, q = table, temp_2
            end
            if branch_result then
                A = table.unpack
            end
            branch_result = A
            I = A
            if (not branch_result) then
                I = unpack
            end
            do
                local temp_1, temp_13, temp_14, temp_3, temp_4, temp_8
                temp_1 = {}
                temp_1.value = I
                temp_3 = q.value(3, 65)
                temp_4 = {}
                temp_4.value = temp_3
                temp_8 = ({unpack_values({pcall(bind(callbacks.callback_203, {}))})})[2]
                temp_13 = tonumber(unpack_values({l.value(tostring(temp_8), ":(%d*):")()}))
                temp_14 = {}
                temp_14.value = temp_13
                A, J, K, M, Q, n, y, z = 0, temp_1, 0, temp_8, temp_4.value, 0, temp_14, temp_4
            end
            while true do
                do
                    local temp_1
                    temp_1 = (1 + n)
                    branch_result = ((false and (temp_1 >= Q)) or ((not false) and (Q >= temp_1)))
                    n = temp_1
                end
                if (not branch_result) then
                    do
                        local temp_1
                        temp_1 = B.value
                        branch_result = temp_1
                        n = temp_1
                    end
                    if branch_result then
                        n = (A == K)
                    end
                    B.value = n
                    branch_result = B.value
                    if (not branch_result) then
                        return unpack_values({unpack_values({bind(callbacks.callback_12, {u})()})})
                    end
                    do
                        local temp_1, temp_2, temp_3, temp_4, temp_5, temp_6, temp_7
                        temp_1 = {}
                        temp_2 = {}
                        temp_3 = {}
                        temp_3.value = nil
                        temp_4 = {}
                        temp_4.value = nil
                        temp_2.value = 2
                        temp_5 = math.floor
                        temp_6 = {}
                        temp_7 = {}
                        temp_7.value = temp_5
                        temp_6.value = 0
                        temp_1.value = {}
                        A, B, D, J, a, g, l, o, q, u, z = math.random, temp_4, 0, table.remove, temp_1, temp_7, string.char, temp_2, temp_6, temp_3, {}
                    end
                    while true do
                        do
                            local temp_1, temp_2
                            temp_1 = (not false)
                            temp_2 = (D + 1)
                            branch_result = ((false and (temp_2 >= 256)) or (temp_1 and (256 >= temp_2)))
                            D = temp_2
                        end
                        if not branch_result then break end
                        z[D] = D
                    end
                    while true do
                        do
                            local temp_3
                            temp_3 = J(z, A(1, (# z)))
                            a.value[temp_3] = l((temp_3 - 1))
                            branch_result = ((# z) == 0)
                        end
                        if not (not branch_result) then break end
                    end
                    do
                        local temp_1, temp_124, temp_125, temp_126, temp_131, temp_136, temp_137, temp_138,
                            temp_143, temp_144, temp_145, temp_148, temp_15, temp_151, temp_152, temp_157,
                            temp_16, temp_160, temp_161, temp_164, temp_167, temp_172, temp_173, temp_174,
                            temp_175, temp_177, temp_20, temp_24, temp_25, temp_29, temp_3, temp_30, temp_34,
                            temp_35, temp_4, temp_45, temp_46, temp_47, temp_48, temp_49, temp_5, temp_53,
                            temp_56, temp_6, temp_60, temp_61, temp_67, temp_68, temp_84
                        temp_1 = {}
                        temp_1.value = {}
                        temp_3 = bind(callbacks.next_decryption_byte, {temp_1, q, o, g})
                        temp_4 = {}
                        temp_4.value = temp_3
                        temp_5 = {}
                        temp_6 = {}
                        temp_6.value = temp_5
                        u.value = setmetatable({}, {["__index"] = temp_6.value, ["__metatable"] = nil})
                        B.value = bind(callbacks.decode_cached_string, {temp_6, temp_1, a, q, o, temp_4})
                        temp_15 = game.GetService(game, "HttpService")
                        temp_16 = {}
                        temp_16.value = temp_15
                        temp_20 = game.GetService(game, "Players")
                        temp_24 = game.GetService(game, "CoreGui")
                        temp_25 = {}
                        temp_25.value = temp_24
                        temp_29 = game.GetService(game, "RunService")
                        temp_30 = {}
                        temp_30.value = temp_29
                        temp_34 = game.GetService(game, "TweenService")
                        temp_35 = {}
                        temp_35.value = temp_34
                        tostring(temp_20.LocalPlayer.UserId)
                        temp_45 = bind(callbacks.callback_73, {u, B, temp_30})
                        temp_46 = bind(callbacks.callback_74, {u, B})
                        temp_47 = {}
                        temp_47.value = temp_45
                        temp_48 = {}
                        temp_48.value = temp_46
                        temp_49 = {}
                        temp_49.value = bind(callbacks.build_loading_interface, {temp_25, u, B, temp_47, temp_35, temp_30, temp_48})
                        temp_53 = {}
                        temp_53.value = "https://files.catbox.moe/54lm4f.jpg"
                        temp_56 = {}
                        temp_56.value = "KaiserHub_Media"
                        temp_60 = (temp_56.value .. "/KaiserHub_Bg.jpg10")
                        temp_61 = {}
                        temp_61.value = temp_60
                        temp_67 = Instance.new("ScreenGui")
                        temp_68 = {}
                        temp_68.value = temp_67
                        temp_68.value.Name = "KaiserAuthUI"
                        temp_68.value.Parent = temp_25.value
                        temp_84 = Instance.new("Frame", temp_68.value)
                        temp_84.Size = UDim2.new(0, 320, 0, 170)
                        temp_84.Position = UDim2.new(0.5, -160, 0.5, -85)
                        temp_84.BackgroundTransparency = 1
                        temp_84.BorderSizePixel = 0
                        temp_84.Active = true
                        temp_84.ClipsDescendants = true
                        Instance.new("UICorner", temp_84).CornerRadius = UDim.new(0, 12)
                        temp_124 = Instance.new("ImageLabel")
                        temp_125 = {}
                        temp_125.value = temp_124
                        temp_126 = temp_125.value
                        temp_126.Name = "BackgroundImage"
                        temp_131 = temp_125.value
                        temp_136 = UDim2.new
                        temp_137 = temp_136(1, 0, 1, 0)
                        temp_131.Size = temp_137
                        temp_138 = temp_125.value
                        temp_143 = UDim2.new
                        temp_144 = temp_143(0, 0, 0, 0)
                        temp_138.Position = temp_144
                        temp_145 = temp_125.value
                        temp_145.BackgroundTransparency = 1
                        temp_148 = temp_125.value
                        temp_151 = temp_53.value
                        temp_148.Image = temp_151
                        temp_152 = temp_125.value
                        temp_157 = Enum.ScaleType
                        temp_160 = temp_157.Crop
                        temp_152.ScaleType = temp_160
                        temp_161 = temp_125.value
                        temp_161.ImageTransparency = 0
                        temp_164 = temp_125.value
                        temp_164.ZIndex = 1
                        temp_167 = temp_125.value
                        temp_167.Parent = temp_84
                        temp_172 = game.GetService
                        temp_173 = temp_172(game, "UserInputService")
                        temp_174 = {}
                        temp_174.value = temp_173
                        temp_175 = bind(callbacks.callback_76, {u, B, temp_174, temp_35})
                        temp_175(temp_84)
                        temp_177 = temp_47.value
                        temp_177(temp_84)
                        branch_result = getcustomasset
                        D, F, Hh, K, M, P, R, W, a, l, m, o, q, w, y = temp_48, temp_125, getcustomasset, temp_47, temp_49, temp_84, temp_61, temp_53, temp_35, temp_16, temp_174, temp_25, temp_30, temp_56, temp_68
                    end
                    if (not branch_result) then
                        branch_result = getsynasset
                        Zh = getsynasset
                        if (not branch_result) then
                            branch_result = fileasset
                            ch = fileasset
                            if branch_result then
                                ch = bind(callbacks.callback_15, {u, B})
                            end
                            Zh = ch
                        end
                        Hh = Zh
                    end
                    do
                        local temp_1
                        temp_1 = {}
                        temp_1.value = Hh
                        branch_result = isfile
                        Hh, ih = isfile, temp_1
                    end
                    if (not branch_result) then
                        branch_result = is_file
                        kh = is_file
                        if (not branch_result) then
                            branch_result = readfile
                            Eh = readfile
                            if branch_result then
                                Eh = bind(callbacks.callback_70, {})
                            end
                            kh = Eh
                        end
                        Hh = kh
                    end
                    do
                        local temp_1
                        temp_1 = {}
                        temp_1.value = Hh
                        branch_result = writefile
                        Hh, Zh = writefile, temp_1
                    end
                    if (not branch_result) then
                        Hh = write_file
                    end
                    do
                        local temp_1
                        temp_1 = {}
                        temp_1.value = Hh
                        branch_result = isfolder
                        Hh, kh = isfolder, temp_1
                    end
                    if (not branch_result) then
                        Hh = bind(callbacks.callback_81, {})
                    end
                    do
                        local temp_1
                        temp_1 = {}
                        temp_1.value = Hh
                        branch_result = makefolder
                        Hh, ch = makefolder, temp_1
                    end
                    if (not branch_result) then
                        Hh = bind(callbacks.callback_68, {})
                    end
                    do
                        local temp_1, temp_102, temp_103, temp_108, temp_109, temp_118, temp_119, temp_12,
                            temp_124, temp_127, temp_138, temp_141, temp_142, temp_143, temp_148, temp_149,
                            temp_150, temp_155, temp_156, temp_157, temp_162, temp_167, temp_172, temp_173,
                            temp_174, temp_177, temp_182, temp_183, temp_184, temp_189, temp_192, temp_193,
                            temp_196, temp_199, temp_204, temp_207, temp_208, temp_214, temp_215, temp_218,
                            temp_221, temp_226, temp_227, temp_232, temp_233, temp_242, temp_243, temp_248,
                            temp_249, temp_254, temp_257, temp_272, temp_275, temp_280, temp_281, temp_284,
                            temp_287, temp_292, temp_293, temp_300, temp_303, temp_306, temp_309, temp_310,
                            temp_311, temp_314, temp_317, temp_320, temp_323, temp_324, temp_325, temp_328,
                            temp_331, temp_332, temp_333, temp_336, temp_339, temp_34, temp_340, temp_341,
                            temp_344, temp_347, temp_348, temp_349, temp_35, temp_352, temp_355, temp_356,
                            temp_357, temp_358, temp_359, temp_36, temp_360, temp_361, temp_364, temp_365,
                            temp_366, temp_367, temp_370, temp_371, temp_372, temp_83, temp_84, temp_85,
                            temp_88, temp_89, temp_90, temp_91, temp_94, temp_97
                        temp_1 = {}
                        temp_1.value = Hh
                        task.spawn(bind(callbacks.callback_26, {kh, Zh, temp_1, ih, ch, w, R, W, F, u, B}))
                        temp_12 = Instance.new("UIStroke", P)
                        temp_12.Color = Color3.fromRGB(255, 255, 255)
                        temp_12.Thickness = 3
                        temp_12.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
                        temp_34 = Instance.new("UIGradient", temp_12)
                        temp_35 = {}
                        temp_35.value = temp_34
                        temp_36 = temp_35.value
                        temp_83 = ColorSequence.new({ColorSequenceKeypoint.new(0, unpack_values({Color3.fromRGB(255, 255, 255)})), ColorSequenceKeypoint.new(0.25, unpack_values({Color3.fromRGB(255, 255, 255)})), ColorSequenceKeypoint.new(0.5, unpack_values({Color3.fromRGB(0, 0, 0)})), ColorSequenceKeypoint.new(0.75, unpack_values({Color3.fromRGB(0, 0, 0)})), unpack_values({ColorSequenceKeypoint.new(1, unpack_values({Color3.fromRGB(192, 192, 192)}))})})
                        temp_36.Color = temp_83
                        temp_84 = {}
                        temp_84.value = nil
                        temp_85 = q.value
                        temp_88 = temp_85.RenderStepped
                        temp_89 = bind(callbacks.callback_27, {temp_35, u, B, temp_84})
                        temp_90 = temp_88.Connect
                        temp_91 = temp_90(temp_88, temp_89)
                        temp_84.value = temp_91
                        temp_94 = Instance.new
                        temp_97 = temp_94("TextLabel", P)
                        temp_102 = UDim2.new
                        temp_103 = temp_102(1, 0, 0, 25)
                        temp_97.Size = temp_103
                        temp_108 = UDim2.new
                        temp_109 = temp_108(0, 0, 0.14, 0)
                        temp_97.Position = temp_109
                        temp_97.Text = "Kaiser Hub Ingresa Tu Key"
                        temp_118 = Color3.fromRGB
                        temp_119 = temp_118(255, 255, 255)
                        temp_97.TextColor3 = temp_119
                        temp_124 = Enum.Font
                        temp_127 = temp_124.BuilderSansBold
                        temp_97.Font = temp_127
                        temp_97.TextSize = 20
                        temp_97.BackgroundTransparency = 1
                        temp_97.ZIndex = 3
                        temp_97.Parent = P
                        temp_138 = Instance.new
                        temp_141 = temp_138("TextBox", P)
                        temp_142 = {}
                        temp_142.value = temp_141
                        temp_143 = temp_142.value
                        temp_148 = UDim2.new
                        temp_149 = temp_148(0, 280, 0, 42)
                        temp_143.Size = temp_149
                        temp_150 = temp_142.value
                        temp_155 = UDim2.new
                        temp_156 = temp_155(0.5, -140, 0.38, 0)
                        temp_150.Position = temp_156
                        temp_157 = temp_142.value
                        temp_157.PlaceholderText = "Pega tu key aqu铆"
                        temp_162 = temp_142.value
                        temp_162.Text = ""
                        temp_167 = temp_142.value
                        temp_172 = Color3.fromRGB
                        temp_173 = temp_172(24, 24, 28)
                        temp_167.BackgroundColor3 = temp_173
                        temp_174 = temp_142.value
                        temp_174.BackgroundTransparency = 0.2
                        temp_177 = temp_142.value
                        temp_182 = Color3.new
                        temp_183 = temp_182(1, 1, 1)
                        temp_177.TextColor3 = temp_183
                        temp_184 = temp_142.value
                        temp_189 = Enum.Font
                        temp_192 = temp_189.BuilderSansBold
                        temp_184.Font = temp_192
                        temp_193 = temp_142.value
                        temp_193.TextSize = 14
                        temp_196 = temp_142.value
                        temp_196.ZIndex = 3
                        temp_199 = temp_142.value
                        temp_199.Parent = P
                        temp_204 = Instance.new
                        temp_207 = temp_142.value
                        temp_208 = temp_204("UICorner", temp_207)
                        temp_214 = UDim.new
                        temp_215 = temp_214(0, 12)
                        temp_208.CornerRadius = temp_215
                        temp_218 = Instance.new
                        temp_221 = temp_218("TextButton", P)
                        temp_226 = UDim2.new
                        temp_227 = temp_226(0, 130, 0, 38)
                        temp_221.Size = temp_227
                        temp_232 = UDim2.new
                        temp_233 = temp_232(0.5, -65, 0.72, 0)
                        temp_221.Position = temp_233
                        temp_221.Text = "Verificar"
                        temp_242 = Color3.fromRGB
                        temp_243 = temp_242(192, 192, 192)
                        temp_221.BackgroundColor3 = temp_243
                        temp_248 = Color3.new
                        temp_249 = temp_248(0, 0, 0)
                        temp_221.TextColor3 = temp_249
                        temp_254 = Enum.Font
                        temp_257 = temp_254.BuilderSansBold
                        temp_221.Font = temp_257
                        temp_221.TextSize = 14
                        temp_221.Active = true
                        temp_221.AutoButtonColor = false
                        temp_221.ZIndex = 3
                        temp_221.Parent = P
                        temp_272 = Instance.new
                        temp_275 = temp_272("UICorner", temp_221)
                        temp_280 = UDim.new
                        temp_281 = temp_280(0, 12)
                        temp_275.CornerRadius = temp_281
                        temp_284 = Instance.new
                        temp_287 = temp_284("UIStroke", temp_221)
                        temp_292 = Color3.fromRGB
                        temp_293 = temp_292(255, 255, 255)
                        temp_287.Color = temp_293
                        temp_287.Thickness = 2.5
                        temp_300 = Enum.ApplyStrokeMode
                        temp_303 = temp_300.Border
                        temp_287.ApplyStrokeMode = temp_303
                        temp_306 = Instance.new
                        temp_309 = temp_306("UIGradient", temp_287)
                        temp_310 = {}
                        temp_310.value = temp_309
                        temp_311 = temp_310.value
                        temp_314 = {}
                        temp_317 = ColorSequence.new
                        temp_320 = ColorSequenceKeypoint.new
                        temp_323 = Color3.fromRGB
                        temp_324 = {temp_323(0, 0, 0)}
                        temp_325 = temp_320(0, unpack_values(temp_324))
                        temp_328 = ColorSequenceKeypoint.new
                        temp_331 = Color3.fromRGB
                        temp_332 = {temp_331(255, 255, 255)}
                        temp_333 = temp_328(0.25, unpack_values(temp_332))
                        temp_336 = ColorSequenceKeypoint.new
                        temp_339 = Color3.fromRGB
                        temp_340 = {temp_339(255, 255, 255)}
                        temp_341 = temp_336(0.5, unpack_values(temp_340))
                        temp_344 = ColorSequenceKeypoint.new
                        temp_347 = Color3.fromRGB
                        temp_348 = {temp_347(0, 0, 0)}
                        temp_349 = temp_344(0.75, unpack_values(temp_348))
                        temp_352 = ColorSequenceKeypoint.new
                        temp_355 = Color3.fromRGB
                        temp_356 = {temp_355(0, 0, 0)}
                        temp_357 = {temp_352(1, unpack_values(temp_356))}
                        temp_358 = {temp_325, temp_333, temp_341, temp_349, unpack_values(temp_357)}
                        temp_359 = temp_317(temp_358)
                        temp_311.Color = temp_359
                        temp_360 = {}
                        temp_360.value = nil
                        temp_361 = q.value
                        temp_364 = temp_361.RenderStepped
                        temp_365 = bind(callbacks.callback_28, {temp_310, u, B, temp_360})
                        temp_366 = temp_364.Connect
                        temp_367 = temp_366(temp_364, temp_365)
                        temp_360.value = temp_367
                        temp_370 = bind(callbacks.callback_29, {temp_142, u, B, l, temp_84, temp_360, y, M})
                        temp_371 = temp_221.Activated
                        temp_372 = temp_371.Connect
                        temp_372(temp_371, temp_370)
                        return unpack_values(temp_314)
                    end
                end
                do
                    local temp_1, temp_10, temp_11, temp_14, temp_15, temp_22, temp_23, temp_24, temp_26,
                        temp_3, temp_4, temp_6, temp_7
                    temp_1 = {}
                    temp_1.value = n
                    temp_3 = math.random(1, 100)
                    temp_4 = {}
                    temp_4.value = temp_3
                    temp_6 = q.value(0, 255)
                    temp_7 = {}
                    temp_7.value = temp_6
                    temp_10 = q.value(1, temp_4.value)
                    temp_11 = {}
                    temp_11.value = temp_10
                    temp_14 = (q.value(1, 2) == 1)
                    temp_15 = {}
                    temp_15.value = temp_14
                    temp_22 = M.gsub(M, ":(%d*):", (":" .. (tostring(unpack_values({q.value(0, 10000)})) .. ":")))
                    temp_23 = {}
                    temp_24 = bind(callbacks.callback_42, {q, temp_1, z, l, B, y, temp_15, temp_23, temp_4, temp_11, temp_7, J})
                    temp_23.value = temp_22
                    temp_26 = {unpack_values({pcall(temp_24)})}
                    branch_result = temp_15.value
                    F, G, O, P, R, W, w = temp_11, temp_1, temp_26, temp_23, temp_7, temp_15, temp_4
                end
                if branch_result then
                    do
                        local temp_1
                        temp_1 = B.value
                        branch_result = temp_1
                        I = temp_1
                    end
                    if branch_result then
                        do
                            local temp_3
                            temp_3 = (O[1] == false)
                            branch_result = temp_3
                            hh = temp_3
                        end
                        if branch_result then
                            hh = (O[2] == P.value)
                        end
                        I = hh
                    end
                    B.value = I
                else
                    do
                        local temp_1
                        temp_1 = B.value
                        branch_result = temp_1
                        x = temp_1
                    end
                    if branch_result then
                        x = O[1]
                    end
                    B.value = x
                    A, K = ((A + O[(F.value + 1)]) % 256), ((K + R.value) % 256)
                end
            end
        end
        branch_result = (l == 0)
        q = l
        if branch_result then
            branch_result = (B.value ~= "GCk1x4aKpbKFD1c")
            if branch_result then
                while true do
                    branch_result = true
                    if not branch_result then break end
                
                end
            end
            B.value = false
        else
            branch_result = (q == 1)
            if branch_result then
                branch_result = (B.value == false)
                if branch_result then
                
                end
            end
        end
    end
end

-- callback_1; bloques originales: 3
callbacks.callback_1 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_4, temp_7
        temp_4 = game.GetService(game, "Players")
        temp_7 = temp_4.GetNameFromUserIdAsync(temp_4, captures[3].value)
        branch_result = temp_7
        X = temp_7
    end
    if branch_result then
        captures[4].value.Text = X
    end
    return unpack_values({})
end

-- callback_2; bloques originales: 1
callbacks.callback_2 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        return unpack_values({unpack_values({temp_1.GetUserThumbnailAsync(temp_1, captures[2].value, captures[3].value, captures[4].value)})})
    end
end

-- callback_3; bloques originales: 5
callbacks.callback_3 = function(captures, arguments)
    local branch_result, l
    local e7 = {}
    do
        local temp_27, temp_44
        temp_27 = math.clamp(((arguments[1].Position.X - captures[3].value.AbsolutePosition.X) / captures[3].value.AbsoluteSize.X), 0, 1)
        captures[4].value.Size = UDim2.new(temp_27, 0, 1, 0)
        temp_44 = math.floor((captures[5].value + ((captures[6].value - captures[5].value) * temp_27)))
        captures[7].value.Text = tostring(temp_44)
        branch_result = (captures[8].value[captures[9].value] ~= temp_44)
        l = temp_44
    end
    if branch_result then
        captures[8].value[captures[9].value] = l
    end
    branch_result = captures[10].value
    if branch_result then
        captures[10].value(l)
    end
    return unpack_values({})
end

-- callback_4; bloques originales: 5
callbacks.callback_4 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_11, temp_3
        temp_3 = arguments[1]
        temp_11 = (temp_3.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_11
        I, X = temp_11, temp_3
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = true
        _G.KaiserGripDragging = true
        captures[4].value(X)
    end
    return unpack_values({})
end

-- callback_5; bloques originales: 7
callbacks.callback_5 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = captures[1].value
        temp_3 = arguments[1]
        branch_result = temp_1
        I, X = temp_1, temp_3
    end
    if branch_result then
        do
            local temp_10
            temp_10 = (X.UserInputType == Enum.UserInputType.MouseMovement)
            branch_result = temp_10
            B = temp_10
        end
        if (not branch_result) then
            B = (X.UserInputType == Enum.UserInputType.Touch)
        end
        I = B
    end
    branch_result = I
    if branch_result then
        captures[4].value(X)
    end
    return unpack_values({})
end

-- callback_6; bloques originales: 5
callbacks.callback_6 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = false
        _G.KaiserGripDragging = false
        task.spawn(captures[4].value)
    end
    return unpack_values({})
end

-- callback_7; bloques originales: 8
callbacks.callback_7 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_5
        temp_5 = tonumber(captures[1].value.Text)
        branch_result = temp_5
        X = temp_5
    end
    if branch_result then
        do
            local temp_10
            temp_10 = math.clamp(math.floor(X), captures[4].value, captures[5].value)
            captures[1].value.Text = tostring(temp_10)
            branch_result = (captures[6].value[captures[7].value] ~= temp_10)
            X = temp_10
        end
        if branch_result then
            captures[6].value[captures[7].value] = X
        end
        captures[8].value.Size = UDim2.new(((X - captures[4].value) / (captures[5].value - captures[4].value)), 0, 1, 0)
        branch_result = captures[9].value
        if branch_result then
            captures[9].value(X)
        end
        task.spawn(captures[10].value)
    else
        captures[1].value.Text = tostring(captures[6].value[captures[7].value])
    end
    return unpack_values({})
end

-- callback_8; bloques originales: 1
callbacks.callback_8 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.BackgroundColor3 = captures[4].value.PanelColor
    return unpack_values({})
end

-- callback_9; bloques originales: 1
callbacks.callback_9 = function(captures, arguments)
    local branch_result
    local e7 = {}
    totouchinterest(arguments[1], arguments[2], arguments[3])
    return unpack_values({})
end

-- callback_10; bloques originales: 26
callbacks.callback_10 = function(captures, arguments)
    local B, X, branch_result, g, l, o, q
    local e7 = {}
    do
        local temp_1, temp_4
        temp_1 = captures[1].value
        temp_4 = {pairs(unpack_values({temp_1.GetDescendants(temp_1)}))}
        B, X, l = temp_4[3], temp_4[2], temp_4[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            do
                local temp_16
                captures[5].value.AssemblyLinearVelocity = Vector3.zero
                captures[5].value.AssemblyAngularVelocity = Vector3.zero
                temp_16 = captures[5].value.CFrame
                captures[6].value.PlatformStand = true
                branch_result = captures[7].value
                X = temp_16
            end
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[7].value
                    temp_1.Destroy(temp_1)
                end
            end
            do
                local temp_103, temp_104, temp_109, temp_110, temp_111, temp_114, temp_42, temp_54, temp_55, temp_98
                captures[7].value = Instance.new("Seat")
                captures[7].value.Name = "KaiserGhostSeat"
                captures[7].value.Anchored = false
                captures[7].value.CanCollide = false
                captures[7].value.CanTouch = true
                captures[7].value.Massless = true
                captures[7].value.Transparency = 1
                captures[7].value.CFrame = X
                captures[7].value.Parent = workspace
                temp_42 = Instance.new("Weld")
                temp_42.Part0 = captures[7].value
                temp_42.Part1 = captures[5].value
                temp_54 = CFrame.new()
                temp_55 = {}
                temp_42.C0 = temp_54
                temp_42.C1 = CFrame.new()
                temp_42.Parent = captures[7].value
                captures[8].value = Instance.new("BodyGyro")
                captures[8].value.P = 90000
                captures[8].value.maxTorque = Vector3.new(9000000000, 9000000000, 9000000000)
                captures[8].value.CFrame = captures[7].value.CFrame
                captures[8].value.Parent = captures[7].value
                captures[9].value = Instance.new("BodyVelocity")
                temp_98 = captures[9].value
                temp_103 = Vector3.zero
                temp_98.Velocity = temp_103
                temp_104 = captures[9].value
                temp_109 = Vector3.new
                temp_110 = temp_109(9000000000, 9000000000, 9000000000)
                temp_104.maxForce = temp_110
                temp_111 = captures[9].value
                temp_114 = captures[7].value
                temp_111.Parent = temp_114
                return unpack_values(temp_55)
            end
        end
        do
            local temp_4
            temp_4 = o.IsA(o, "BasePart")
            branch_result = temp_4
            g = temp_4
        end
        if (not branch_result) then
            do
                local temp_4
                temp_4 = o.IsA(o, "Decal")
                branch_result = temp_4
                q = temp_4
            end
            if (not branch_result) then
                q = o.IsA(o, "Texture")
            end
            g = q
        end
        branch_result = g
        if branch_result then
            do
                local temp_6
                temp_6 = (o.Name ~= "HumanoidRootPart")
                branch_result = temp_6
                g = temp_6
            end
            if branch_result then
                g = (o.Name ~= "KaiserHitboxPart")
            end
            branch_result = g
            if branch_result then
                branch_result = (captures[4].value[o] == nil)
                if branch_result then
                    captures[4].value[o] = o.Transparency
                end
                o.Transparency = 0.75
            end
            branch_result = o.IsA(o, "BasePart")
            if branch_result then
                o.CanCollide = false
            end
        else
            do
                local temp_4
                temp_4 = o.IsA(o, "ParticleEmitter")
                branch_result = temp_4
                g = temp_4
            end
            if (not branch_result) then
                do
                    local temp_4
                    temp_4 = o.IsA(o, "Trail")
                    branch_result = temp_4
                    q = temp_4
                end
                if (not branch_result) then
                    q = o.IsA(o, "BillboardGui")
                end
                g = q
            end
            branch_result = g
            if branch_result then
                o.Enabled = true
            end
        end
    end
end

-- callback_11; bloques originales: 3
callbacks.callback_11 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        captures[2].value()
    end
    return unpack_values({})
end

-- callback_12; bloques originales: 4
callbacks.callback_12 = function(captures, arguments)
    local branch_result
    local e7 = {}
    while true do
        branch_result = true
        if not branch_result then break end
        l1 = l2
        l2 = l1
        captures[1].value()
    end
    return unpack_values({})
end

-- callback_13; bloques originales: 3
callbacks.callback_13 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_14, temp_18, temp_21, temp_22
        captures[1].value = true
        captures[2].value.Text = "..."
        captures[2].value.TextColor3 = Color3.fromRGB(255, 255, 255)
        temp_14 = {}
        temp_14.value = nil
        temp_18 = captures[5].value.InputBegan
        temp_21 = temp_18.Connect(temp_18, bind(callbacks.callback_95, {captures[3], captures[4], temp_14, captures[6], captures[7], captures[2], captures[8], captures[9], captures[1]}))
        temp_22 = {}
        temp_14.value = temp_21
        return unpack_values(temp_22)
    end
end

-- callback_14; bloques originales: 5
callbacks.callback_14 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        do
            local temp_1
            temp_1 = captures[1].value
            temp_1.FireServer(temp_1)
        end
    else
        branch_result = captures[2].value
        if branch_result then
            do
                local temp_1
                temp_1 = captures[2].value
                captures[1].value = temp_1.FindFirstChild(temp_1, "RE/Events/CollectEventSpawnable")
            end
        end
    end
    return unpack_values({})
end

-- callback_15; bloques originales: 1
callbacks.callback_15 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({("rbxasset://" .. arguments[1])})
end

-- callback_16; bloques originales: 3
callbacks.callback_16 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = (captures[1].value.UserInputState == Enum.UserInputState.End)
    if branch_result then
        captures[4].value = false
    end
    return unpack_values({})
end

-- callback_17; bloques originales: 9
callbacks.callback_17 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        branch_result = temp_1
        X = temp_1
    end
    if branch_result then
        X = UDim2.new(1, -25, 0.5, -11)
    end
    branch_result = X
    I = X
    if (not branch_result) then
        I = UDim2.new(0, 3, 0.5, -11)
    end
    do
        local temp_1
        temp_1 = captures[1].value
        branch_result = temp_1
        B, X = temp_1, I
    end
    if branch_result then
        B = captures[4].value.PanelColor
    end
    branch_result = B
    I = B
    if (not branch_result) then
        I = Color3.fromRGB(50, 50, 55)
    end
    do
        local temp_1, temp_23, temp_26, temp_48
        temp_1 = captures[5].value
        temp_23 = temp_1.Create(temp_1, captures[6].value, TweenInfo.new(0.18, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {["Position"] = X})
        temp_23.Play(temp_23)
        temp_26 = captures[5].value
        temp_48 = temp_26.Create(temp_26, captures[7].value, TweenInfo.new(0.18, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {["BackgroundColor3"] = I})
        temp_48.Play(temp_48)
        return unpack_values({})
    end
end

-- callback_18; bloques originales: 3
callbacks.callback_18 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_11
        captures[1].value = true
        captures[2].value = (not captures[2].value)
        captures[3].value()
        captures[4].value(captures[2].value)
        temp_11 = {}
        task.spawn(captures[7].value)
        task.wait(0.05)
        captures[1].value = false
        return unpack_values(temp_11)
    end
end

-- callback_19; bloques originales: 1
callbacks.callback_19 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value = arguments[1]
    captures[2].value()
    return unpack_values({})
end

-- callback_20; bloques originales: 15
callbacks.callback_20 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    branch_result = (not captures[1].value(captures[2].value))
    if branch_result then
        captures[3].value(captures[2].value)
    end
    branch_result = (not captures[4].value(captures[5].value))
    if branch_result then
        do
            local temp_3
            temp_3 = game.HttpGet(game, captures[6].value)
            branch_result = temp_3
            I, X = temp_3, temp_3
        end
        if branch_result then
            I = ((# X) > 0)
        end
        branch_result = I
        if branch_result then
            captures[7].value(captures[5].value, X)
        end
    end
    branch_result = captures[4].value(captures[5].value)
    if branch_result then
        do
            local temp_3
            temp_3 = captures[8].value(captures[5].value)
            branch_result = temp_3
            I, X = temp_3, temp_3
        end
        if branch_result then
            I = captures[9].value
        end
        branch_result = I
        if branch_result then
            captures[9].value.Image = X
        end
    end
    return unpack_values({})
end

-- callback_21; bloques originales: 1
callbacks.callback_21 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        temp_1.Activate(temp_1)
        return unpack_values({})
    end
end

-- callback_22; bloques originales: 3
callbacks.callback_22 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = (not isfile(captures[1].value))
    if branch_result then
        writefile(captures[1].value, unpack_values({game.HttpGet(game, captures[2].value)}))
    end
    return unpack_values({unpack_values({getcustomasset(captures[1].value)})})
end

-- callback_23; bloques originales: 1
callbacks.callback_23 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        temp_1.FireServer(temp_1, captures[2].value, captures[3].value)
        return unpack_values({})
    end
end

-- callback_24; bloques originales: 1
callbacks.callback_24 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        temp_1.FireServer(temp_1, captures[2].value)
        return unpack_values({})
    end
end

-- callback_25; bloques originales: 1
callbacks.callback_25 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        temp_1.FireServer(temp_1, captures[2].value)
        return unpack_values({})
    end
end

-- callback_26; bloques originales: 9
callbacks.callback_26 = function(captures, arguments)
    local I, X, branch_result, l
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        branch_result = temp_1
        I = temp_1
    end
    if branch_result then
        do
            local temp_1
            temp_1 = captures[2].value
            branch_result = temp_1
            X = temp_1
        end
        if branch_result then
            do
                local temp_1
                temp_1 = captures[3].value
                branch_result = temp_1
                l = temp_1
            end
            if branch_result then
                l = captures[4].value
            end
            X = l
        end
        I = X
    end
    branch_result = I
    if branch_result then
        pcall(bind(callbacks.callback_20, {captures[5], captures[6], captures[3], captures[2], captures[7], captures[8], captures[1], captures[4], captures[9], captures[10], captures[11]}))
    end
    return unpack_values({})
end

-- callback_27; bloques originales: 6
callbacks.callback_27 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = captures[1].value
        temp_3 = arguments[1]
        branch_result = temp_1
        I, X = temp_1, temp_3
    end
    if branch_result then
        I = captures[1].value.Parent
    end
    branch_result = I
    if branch_result then
        captures[1].value.Rotation = ((captures[1].value.Rotation + (60 * X)) % 360)
    else
        do
            local temp_1
            temp_1 = captures[4].value
            temp_1.Disconnect(temp_1)
        end
    end
    return unpack_values({})
end

-- callback_28; bloques originales: 6
callbacks.callback_28 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = captures[1].value
        temp_2 = arguments[1]
        branch_result = temp_1
        I, X = temp_1, temp_2
    end
    if branch_result then
        I = captures[1].value.Parent
    end
    branch_result = I
    if branch_result then
        captures[1].value.Rotation = ((captures[1].value.Rotation - (90 * X)) % 360)
    else
        do
            local temp_1
            temp_1 = captures[4].value
            temp_1.Disconnect(temp_1)
        end
    end
    return unpack_values({})
end

-- callback_29; bloques originales: 5
callbacks.callback_29 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_4, temp_5, temp_9
        temp_4 = captures[1].value.Text
        temp_5 = {}
        temp_5.value = temp_4
        temp_9 = (temp_5.value == "")
        branch_result = temp_9
        I, X = temp_9, temp_5
    end
    if (not branch_result) then
        I = (X.value == "Pega tu key aqu铆")
    end
    branch_result = I
    if branch_result then
        captures[1].value.PlaceholderText = "隆Escribe una key v谩lida!"
        return unpack_values({})
    end
    captures[1].value.Text = ""
    captures[1].value.PlaceholderText = "Conectando al servidor..."
    task.spawn(bind(callbacks.verify_access_key, {captures[2], captures[3], captures[4], X, captures[1], captures[5], captures[6], captures[7], captures[8]}))
    return unpack_values({})
end

-- callback_30; bloques originales: 1
callbacks.callback_30 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        temp_1.Disconnect(temp_1)
        return unpack_values({})
    end
end

-- save_configuration; bloques originales: 1
callbacks.save_configuration = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_6
        temp_6 = (arguments[1].Position - captures[3].value)
        captures[5].value = UDim2.new(captures[4].value.X.Scale, (captures[4].value.X.Offset + temp_6.X), captures[4].value.Y.Scale, (captures[4].value.Y.Offset + temp_6.Y))
        return unpack_values({})
    end
end

-- callback_32; bloques originales: 7
callbacks.callback_32 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_12
        temp_1 = {}
        temp_1.value = arguments[1]
        temp_12 = (temp_1.value.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_12
        B, X = temp_12, temp_1
    end
    if (not branch_result) then
        B = (X.value.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = B
    I = B
    if branch_result then
        I = (not _G.KaiserGripDragging)
    end
    branch_result = I
    if branch_result then
        do
            local temp_14
            captures[3].value = true
            captures[4].value = X.value.Position
            captures[6].value = captures[5].value.Position
            captures[7].value = captures[6].value
            temp_14 = X.value.Changed
            temp_14.Connect(temp_14, bind(callbacks.callback_201, {X, captures[1], captures[2], captures[3]}))
        end
    end
    return unpack_values({})
end

-- callback_33; bloques originales: 5
callbacks.callback_33 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseMovement)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = X
    end
    return unpack_values({})
end

-- callback_34; bloques originales: 5
callbacks.callback_34 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = arguments[1]
        temp_3 = (temp_1 == captures[1].value)
        branch_result = temp_3
        I, X = temp_3, temp_1
    end
    if branch_result then
        I = captures[2].value
    end
    branch_result = I
    if branch_result then
        captures[3].value(X)
    end
    return unpack_values({})
end

-- callback_35; bloques originales: 3
callbacks.callback_35 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        do
            local temp_1, temp_7
            temp_1 = captures[2].value
            temp_7 = captures[2].value.Position
            temp_1.Position = temp_7.Lerp(temp_7, captures[1].value, captures[5].value)
        end
    end
    return unpack_values({})
end

-- callback_36; bloques originales: 3
callbacks.callback_36 = function(captures, arguments)
    local B, branch_result
    local e7 = {}
    do
        local temp_2, temp_3, temp_4
        captures[1].value = nil
        temp_2 = {pcall(bind(callbacks.save_configuration, {captures[2], captures[3], captures[4], captures[5], captures[6]}))}
        temp_3 = temp_2[1]
        temp_4 = temp_2[2]
        branch_result = (not temp_3)
        B = temp_4
    end
    if branch_result then
        warn(("Error al guardar la configuraci贸n: " .. tostring(B)))
    end
    return unpack_values({})
end

-- callback_37; bloques originales: 1
callbacks.callback_37 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({captures[1].value})
end

-- callback_38; bloques originales: 1
callbacks.callback_38 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = {}
        temp_1.value = arguments[1]
        task.defer(bind(callbacks.callback_194, {captures[3], temp_1}))
        return unpack_values({})
    end
end

-- callback_39; bloques originales: 17
callbacks.callback_39 = function(captures, arguments)
    local B, J, X, a, branch_result, g, l, o, q
    local e7 = {}
    do
        local temp_1, temp_4
        temp_1 = captures[1].value
        temp_4 = {ipairs(unpack_values({temp_1.GetDescendants(temp_1)}))}
        B, X, l = temp_4[3], temp_4[2], temp_4[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            return unpack_values({})
        end
        do
            local temp_1, temp_2, temp_6
            temp_1 = {}
            temp_1.value = o
            temp_2 = temp_1.value
            temp_6 = temp_2.IsA(temp_2, "RemoteEvent")
            branch_result = temp_6
            g, o = temp_6, temp_1
        end
        if (not branch_result) then
            do
                local temp_1
                temp_1 = o.value
                g = temp_1.IsA(temp_1, "UnreliableRemoteEvent")
            end
        end
        branch_result = g
        if branch_result then
            do
                local temp_2
                temp_2 = captures[4].value[1]
                branch_result = temp_2
                g = temp_2
            end
            if (not branch_result) then
                g = captures[4].value[2]
            end
            do
                local temp_1
                temp_1 = {}
                temp_1.value = g
                branch_result = temp_1.value
                q = temp_1
            end
            if branch_result then
                do
                    local temp_3
                    temp_3 = captures[5].value(q.value)
                    branch_result = temp_3
                    g = temp_3
                end
                if (not branch_result) then
                    g = q.value.Position
                end
                do
                    local temp_1
                    temp_1 = {}
                    temp_1.value = g
                    J, a = 0, temp_1
                end
                while true do
                    do
                        local temp_1
                        temp_1 = (J + 1)
                        branch_result = ((false and (4 <= temp_1)) or ((not false) and (temp_1 <= 4)))
                        J = temp_1
                    end
                    if not branch_result then break end
                    pcall(bind(callbacks.callback_23, {o, captures[6], a}))
                    pcall(bind(callbacks.callback_24, {o, q}))
                    pcall(bind(callbacks.callback_25, {o, captures[6]}))
                end
            end
        end
    end
end

-- callback_40; bloques originales: 9
callbacks.callback_40 = function(captures, arguments)
    local B, X, branch_result
    local e7 = {}
    branch_result = captures[1].value.GetNetworkPing
    if branch_result then
        do
            local temp_1
            temp_1 = captures[1].value
            captures[4].value = temp_1.GetNetworkPing(temp_1)
        end
    else
        do
            local temp_1
            temp_1 = captures[5].value
            branch_result = temp_1
            X = temp_1
        end
        if branch_result then
            do
                local temp_1, temp_5
                temp_1 = captures[5].value
                temp_5 = temp_1.FindFirstChild(temp_1, "Network")
                branch_result = temp_5
                B = temp_5
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = captures[5].value.Network
                    B = temp_4.FindFirstChild(temp_4, "ServerStatsItem")
                end
            end
            X = B
        end
        branch_result = X
        if branch_result then
            do
                local temp_10
                temp_10 = captures[5].value.Network.ServerStatsItem["Data Ping"]
                captures[4].value = (temp_10.GetValue(temp_10) / 1000)
            end
        end
    end
    return unpack_values({})
end

-- save_configuration; bloques originales: 3
callbacks.save_configuration = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = writefile
    if branch_result then
        do
            local temp_105, temp_112, temp_113, temp_116, temp_119, temp_12, temp_120, temp_123, temp_126,
                temp_129, temp_132, temp_135, temp_138, temp_141, temp_144, temp_147, temp_150, temp_153,
                temp_156, temp_159, temp_162, temp_165, temp_168, temp_171, temp_174, temp_177, temp_18,
                temp_180, temp_183, temp_186, temp_189, temp_192, temp_195, temp_198, temp_201, temp_204,
                temp_207, temp_210, temp_213, temp_216, temp_219, temp_222, temp_225, temp_228, temp_231,
                temp_234, temp_237, temp_24, temp_240, temp_243, temp_246, temp_249, temp_252, temp_255,
                temp_258, temp_261, temp_264, temp_267, temp_270, temp_273, temp_276, temp_279, temp_282,
                temp_285, temp_288, temp_291, temp_294, temp_297, temp_30, temp_300, temp_301, temp_304,
                temp_307, temp_310, temp_311, temp_314, temp_317, temp_318, temp_321, temp_324, temp_325,
                temp_326, temp_327, temp_328, temp_329, temp_330, temp_36, temp_42, temp_48, temp_6, temp_72,
                temp_96
            temp_6 = captures[3].value.Binds
            temp_12 = captures[3].value.ChamsEnabled
            temp_18 = captures[3].value.EspBoxEnabled
            temp_24 = captures[3].value.EspLineEnabled
            temp_30 = captures[3].value.EspLinePosition
            temp_36 = captures[3].value.EspHealthEnabled
            temp_42 = captures[3].value.EspNameEnabled
            temp_48 = captures[3].value.EspDistanceEnabled
            temp_72 = {captures[3].value.ChamsColor.R, captures[3].value.ChamsColor.G, captures[3].value.ChamsColor.B}
            temp_96 = {captures[3].value.EspBoxColor.R, captures[3].value.EspBoxColor.G, captures[3].value.EspBoxColor.B}
            temp_105 = captures[3].value.EspLineColor.R
            temp_112 = captures[3].value.EspLineColor.G
            temp_113 = captures[3].value
            temp_116 = temp_113.EspLineColor
            temp_119 = temp_116.B
            temp_120 = {temp_105, temp_112, temp_119}
            temp_123 = captures[3].value
            temp_126 = temp_123.NotificationsEnabled
            temp_129 = captures[3].value
            temp_132 = temp_129.FloatingButtonEnabled
            temp_135 = captures[3].value
            temp_138 = temp_135.InvisibleFloatEnabled
            temp_141 = captures[3].value
            temp_144 = temp_141.KillAuraFloatEnabled
            temp_147 = captures[3].value
            temp_150 = temp_147.AutoEquipKnifeEnabled
            temp_153 = captures[3].value
            temp_156 = temp_153.AutoFarmEnabled
            temp_159 = captures[3].value
            temp_162 = temp_159.SpeedEnabled
            temp_165 = captures[3].value
            temp_168 = temp_165.SpeedValue
            temp_171 = captures[3].value
            temp_174 = temp_171.JumpEnabled
            temp_177 = captures[3].value
            temp_180 = temp_177.JumpValue
            temp_183 = captures[3].value
            temp_186 = temp_183.NoclipEnabled
            temp_189 = captures[3].value
            temp_192 = temp_189.InvisibleEnabled
            temp_195 = captures[3].value
            temp_198 = temp_195.FlyEnabled
            temp_201 = captures[3].value
            temp_204 = temp_201.FlySpeed
            temp_207 = captures[3].value
            temp_210 = temp_207.AimbotEnabled
            temp_213 = captures[3].value
            temp_216 = temp_213.AutoShootEnabled
            temp_219 = captures[3].value
            temp_222 = temp_219.AimbotWallCheck
            temp_225 = captures[3].value
            temp_228 = temp_225.AimbotTeamCheck
            temp_231 = captures[3].value
            temp_234 = temp_231.AimbotPartIndex
            temp_237 = captures[3].value
            temp_240 = temp_237.HitboxEnabled
            temp_243 = captures[3].value
            temp_246 = temp_243.HitboxSize
            temp_249 = captures[3].value
            temp_252 = temp_249.HitboxVisible
            temp_255 = captures[3].value
            temp_258 = temp_255.KillAuraEnabled
            temp_261 = captures[3].value
            temp_264 = temp_261.AutoClickerEnabled
            temp_267 = captures[3].value
            temp_270 = temp_267.ShowFOV
            temp_273 = captures[3].value
            temp_276 = temp_273.FOVIsMobile
            temp_279 = captures[3].value
            temp_282 = temp_279.FOVRadius
            temp_285 = captures[3].value
            temp_288 = temp_285.FOVThickness
            temp_291 = captures[3].value
            temp_294 = temp_291.FOVColorIndex
            temp_297 = captures[3].value
            temp_300 = temp_297.UIScale
            temp_301 = (temp_300 or 1)
            temp_304 = captures[3].value
            temp_307 = temp_304.PanelColor
            temp_310 = temp_307.R
            temp_311 = captures[3].value
            temp_314 = temp_311.PanelColor
            temp_317 = temp_314.G
            temp_318 = captures[3].value
            temp_321 = temp_318.PanelColor
            temp_324 = temp_321.B
            temp_325 = {temp_310, temp_317, temp_324}
            temp_326 = {["Binds"] = temp_6, ["ChamsEnabled"] = temp_12, ["EspBoxEnabled"] = temp_18, ["EspLineEnabled"] = temp_24, ["EspLinePosition"] = temp_30, ["EspHealthEnabled"] = temp_36, ["EspNameEnabled"] = temp_42, ["EspDistanceEnabled"] = temp_48, ["ChamsColor"] = temp_72, ["EspBoxColor"] = temp_96, ["EspLineColor"] = temp_120, ["NotificationsEnabled"] = temp_126, ["FloatingButtonEnabled"] = temp_132, ["InvisibleFloatEnabled"] = temp_138, ["KillAuraFloatEnabled"] = temp_144, ["AutoEquipKnifeEnabled"] = temp_150, ["AutoFarmEnabled"] = temp_156, ["SpeedEnabled"] = temp_162, ["SpeedValue"] = temp_168, ["JumpEnabled"] = temp_174, ["JumpValue"] = temp_180, ["NoclipEnabled"] = temp_186, ["InvisibleEnabled"] = temp_192, ["FlyEnabled"] = temp_198, ["FlySpeed"] = temp_204, ["AimbotEnabled"] = temp_210, ["AutoShootEnabled"] = temp_216, ["AimbotWallCheck"] = temp_222, ["AimbotTeamCheck"] = temp_228, ["AimbotPartIndex"] = temp_234, ["HitboxEnabled"] = temp_240, ["HitboxSize"] = temp_246, ["HitboxVisible"] = temp_252, ["KillAuraEnabled"] = temp_258, ["AutoClickerEnabled"] = temp_264, ["ShowFOV"] = temp_270, ["FOVIsMobile"] = temp_276, ["FOVRadius"] = temp_282, ["FOVThickness"] = temp_288, ["FOVColorIndex"] = temp_294, ["UIScale"] = temp_301, ["PanelColor"] = temp_325}
            temp_327 = captures[4].value
            temp_328 = captures[5].value
            temp_329 = temp_328.JSONEncode
            temp_330 = {temp_329(temp_328, temp_326)}
            writefile(temp_327, unpack_values(temp_330))
        end
    end
    return unpack_values({})
end

-- callback_42; bloques originales: 12
callbacks.callback_42 = function(captures, arguments)
    local I, X, branch_result, l, u
    local e7 = {}
    do
        local temp_3
        temp_3 = (captures[1].value(1, 2) == 1)
        branch_result = temp_3
        I = temp_3
    end
    if (not branch_result) then
        I = (captures[2].value == captures[3].value)
    end
    branch_result = I
    if branch_result then
        do
            local temp_10, temp_9
            temp_9 = tonumber(unpack_values({captures[4].value(tostring(({unpack_values({pcall(bind(callbacks.callback_100, {}))})})[2]), ":(%d*):")()}))
            temp_10 = captures[5].value
            branch_result = temp_10
            I, X = temp_10, temp_9
        end
        if branch_result then
            I = (captures[6].value == X)
        end
        captures[5].value = I
    end
    branch_result = captures[7].value
    if branch_result then
        error(captures[8].value, 0)
    end
    X, l, u = {}, 0, captures[9].value
    while true do
        do
            local temp_1, temp_2
            temp_1 = (not false)
            temp_2 = (l + 1)
            branch_result = ((false and (temp_2 >= u)) or (temp_1 and (u >= temp_2)))
            l = temp_2
        end
        if not branch_result then break end
        X[l] = captures[1].value(0, 255)
    end
    X[captures[10].value] = captures[11].value
    return unpack_values({unpack_values({captures[12].value(X)})})
end

-- callback_43; bloques originales: 1
callbacks.callback_43 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({pcall(readfile, arguments[1])})
end

-- callback_44; bloques originales: 13
callbacks.callback_44 = function(captures, arguments)
    local B, a, branch_result, g, l, o, q, u
    local e7 = {}
    local steps = {}
    steps.entry = function()
        do
            local temp_12, temp_13, temp_2
            temp_2 = captures[1].value()
            temp_12 = {{["Name"] = "Ninguno", ["Display"] = "Ninguno"}}
            temp_13 = {ipairs(temp_2)}
            B, l, o, u = temp_12, temp_13[2], temp_13[1], temp_13[3]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = o(l, u)
                branch_result = temp_1
                q, u = temp_2, temp_1
            end
            if not branch_result then break end
            table.insert(B, {["Name"] = q.Name, ["Display"] = q.Name})
        end
        do
            local temp_1
            temp_1 = {ipairs(B)}
            g, l, o, u = temp_1[3], 1, temp_1[2], temp_1[1]
        end
        return "step_2"
    end
    steps.step_2 = function()
        do
            local temp_1, temp_2
            temp_1, temp_2 = u(o, g)
            branch_result = temp_1
            a, g = temp_2, temp_1
        end
        if branch_result then
            return "step_3"
        else
            return "step_5"
        end
    end
    steps.step_3 = function()
        branch_result = (a.Name == captures[4].value.SelectedTargetName)
        q = g
        if branch_result then
            return "step_4"
        else
            return "step_6"
        end
    end
    steps.step_4 = function()
        l = q
        return "step_5"
    end
    steps.step_5 = function()
        do
            local temp_1
            temp_1 = (l + 1)
            branch_result = (temp_1 > (# B))
            l = temp_1
        end
        if branch_result then
            l = 1
        end
        do
            local temp_18, temp_22
            captures[4].value.SelectedTargetName = B[l].Name
            captures[4].value.SelectedTargetName = B[l].Display
            temp_18 = captures[5].value.S_TargetSelect
            temp_22 = temp_18.FindFirstChildOfClass(temp_18, "TextLabel")
            branch_result = temp_22
            q = temp_22
        end
        if branch_result then
            q.Text = ("Objetivo Prioritario: " .. captures[4].value.SelectedTargetName)
        end
        do
            local temp_1, temp_5
            temp_1 = captures[6].value
            temp_5 = {}
            temp_1("KaiserHub", ("Jugador Seleccionado: " .. captures[4].value.SelectedTargetName))
            captures[7].value()
            return nil, pack_values(unpack_values(temp_5))
        end
    end
    steps.step_6 = function()

        return "step_2"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_45; bloques originales: 5
callbacks.callback_45 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_7
        temp_1 = arguments[1]
        captures[1].value.InvisibleEnabled = temp_1
        captures[4].value(temp_1)
        temp_7 = captures[5].value
        branch_result = temp_1
        g, o, u = temp_7, temp_1, temp_7
    end
    if branch_result then
        o = "Invisible Activada"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Invisible Desactivada"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_46; bloques originales: 1
callbacks.callback_46 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = captures[1].value
        temp_2 = arguments[1]
        temp_1.InvisibleFloatEnabled = temp_2
        captures[4].value.Visible = temp_2
        captures[5].value()
        return unpack_values({})
    end
end

-- callback_47; bloques originales: 3
callbacks.callback_47 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = arguments[1]
        captures[1].value.AntiLagEnabled = temp_1
        captures[4].value(temp_1)
        captures[5].value()
        branch_result = temp_1
    end
    if branch_result then
        task.delay(0.5, bind(callbacks.callback_78, {captures[1], captures[2], captures[3], captures[6], captures[7], captures[5]}))
    end
    return unpack_values({})
end

-- callback_48; bloques originales: 5
callbacks.callback_48 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.AutoClickerEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Autoclicker Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Autoclicker Desactivado"
    end
    u("KaiserHub", l)
    captures[5].value()
    return unpack_values({})
end

-- callback_49; bloques originales: 14
callbacks.callback_49 = function(captures, arguments)
    local B, X, branch_result, g, l, o, q, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.KillAuraEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        X, g, o, u = temp_1, temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Kill Aura Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Kill Aura Desactivado"
    end
    u("KaiserHub", l)
    branch_result = (not X)
    if branch_result then
        do
            local temp_1, temp_4
            temp_1 = captures[5].value
            temp_4 = {ipairs(unpack_values({temp_1.GetPlayers(temp_1)}))}
            B, l, u = temp_4[2], temp_4[3], temp_4[1]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = u(B, l)
                branch_result = temp_1
                g, l = temp_2, temp_1
            end
            if not branch_result then break end
            branch_result = g.Character
            if branch_result then
                do
                    local temp_3, temp_7
                    temp_3 = g.Character
                    temp_7 = temp_3.FindFirstChild(temp_3, "CustomHitbox")
                    branch_result = temp_7
                    q = temp_7
                end
                if branch_result then
                    q.Destroy(q)
                end
            end
        end
    end
    return unpack_values({})
end

-- callback_50; bloques originales: 1
callbacks.callback_50 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = captures[1].value
        temp_3 = arguments[1]
        temp_1.KillAuraFloatEnabled = temp_3
        captures[4].value.Visible = temp_3
        captures[5].value()
        return unpack_values({})
    end
end

-- callback_51; bloques originales: 5
callbacks.callback_51 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_4, temp_5
        temp_1 = captures[1].value
        temp_4 = arguments[1]
        temp_1.AutoFarmEnabled = temp_4
        temp_5 = captures[4].value
        branch_result = temp_4
        g, o, u = temp_5, temp_4, temp_5
    end
    if branch_result then
        o = "Autofarm Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Autofarm Desactivado"
    end
    u("KaiserHub", l)
    captures[5].value()
    return unpack_values({})
end

-- callback_52; bloques originales: 1
callbacks.callback_52 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.ShowFOV = arguments[1]
    return unpack_values({})
end

-- callback_53; bloques originales: 5
callbacks.callback_53 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.FOVIsMobile = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "FOV Modo M贸vil (Centro)"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "FOV Modo PC (Cursor)"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_54; bloques originales: 3
callbacks.callback_54 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.FOVColorIndex = (captures[1].value.FOVColorIndex + 1)
    branch_result = (captures[1].value.FOVColorIndex > (# captures[4].value))
    if branch_result then
        captures[1].value.FOVColorIndex = 1
    end
    do
        local temp_6
        temp_6 = captures[4].value[captures[1].value.FOVColorIndex]
        captures[1].value.FOVColor = temp_6.Color
        captures[5].value.BackgroundColor3 = temp_6.Color
        captures[6].value("KaiserHub", ("Color del FOV cambiado a: " .. temp_6.Name))
        captures[7].value()
        return unpack_values({})
    end
end

-- callback_55; bloques originales: 19
callbacks.callback_55 = function(captures, arguments)
    local B, I, X, branch_result, l
    local e7 = {}
    do
        local temp_1
        temp_1 = arguments[1]
        branch_result = (not temp_1)
        X = temp_1
    end
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_4
        temp_4 = captures[1].value.AimbotPartIndex
        branch_result = (temp_4 == 1)
        B = temp_4
    end
    if (not branch_result) then
        branch_result = (B == 2)
        if (not branch_result) then
            branch_result = (B == 3)
            if (not branch_result) then
                return unpack_values({unpack_values({X.FindFirstChild(X, "HumanoidRootPart")})})
            end
            do
                local temp_4
                temp_4 = X.FindFirstChild(X, "LowerTorso")
                branch_result = temp_4
                I = temp_4
            end
            if (not branch_result) then
                do
                    local temp_4
                    temp_4 = X.FindFirstChild(X, "Torso")
                    branch_result = temp_4
                    l = temp_4
                end
                if (not branch_result) then
                    l = X.FindFirstChild(X, "HumanoidRootPart")
                end
                I = l
            end
            return unpack_values({I})
        end
        do
            local temp_4
            temp_4 = X.FindFirstChild(X, "UpperTorso")
            branch_result = temp_4
            I = temp_4
        end
        if (not branch_result) then
            do
                local temp_4
                temp_4 = X.FindFirstChild(X, "Torso")
                branch_result = temp_4
                l = temp_4
            end
            if (not branch_result) then
                l = X.FindFirstChild(X, "Head")
            end
            I = l
        end
        return unpack_values({I})
    end
    do
        local temp_4
        temp_4 = X.FindFirstChild(X, "Head")
        branch_result = temp_4
        I = temp_4
    end
    if (not branch_result) then
        I = X.FindFirstChild(X, "HumanoidRootPart")
    end
    return unpack_values({I})
end

-- callback_56; bloques originales: 31
callbacks.callback_56 = function(captures, arguments)
    local A, B, J, K, Q, X, a, branch_result, g, l, n, o, u, y
    local e7 = {}
    local steps = {}
    steps.entry = function()
        do
            local temp_1, temp_2, temp_5, temp_6, temp_9
            temp_1 = captures[1].value
            temp_2 = arguments[1]
            temp_5 = temp_1.FOVRadius
            temp_6 = captures[4].value
            temp_9 = {ipairs(unpack_values({temp_6.GetPlayers(temp_6)}))}
            B, X, g, l, o, u = nil, temp_2, temp_9[1], temp_5, temp_9[3], temp_9[2]
        end
        return "step_2"
    end
    steps.step_2 = function()
        do
            local temp_1, temp_2
            temp_1, temp_2 = g(u, o)
            branch_result = temp_1
            a, o = temp_2, temp_1
        end
        if (not branch_result) then
            return nil, pack_values(unpack_values({B}))
        end
        do
            local temp_2
            temp_2 = (a ~= captures[5].value)
            branch_result = temp_2
            J = temp_2
        end
        if branch_result then
            do
                local temp_3
                temp_3 = a.Character
                branch_result = temp_3
                A = temp_3
            end
            if branch_result then
                do
                    local temp_3, temp_7
                    temp_3 = a.Character
                    temp_7 = temp_3.FindFirstChild(temp_3, "Humanoid")
                    branch_result = temp_7
                    K = temp_7
                end
                if branch_result then
                    K = (a.Character.Humanoid.Health > 0)
                end
                A = K
            end
            J = A
        end
        branch_result = J
        if branch_result then
            return "step_3"
        else
            return "step_8"
        end
    end
    steps.step_3 = function()
        do
            local temp_5
            temp_5 = captures[6].value(a.Character)
            branch_result = temp_5
            J = temp_5
        end
        if branch_result then
            return "step_4"
        else
            return "step_7"
        end
    end
    steps.step_4 = function()
        do
            local temp_4
            temp_4 = captures[1].value.AimbotTeamCheck
            branch_result = temp_4
            A = temp_4
        end
        if branch_result then
            A = (not captures[7].value(a))
        end
        branch_result = A
        if branch_result then
            return "step_5"
        else
            return "step_6"
        end
    end
    steps.step_5 = function()

        return "step_2"
    end
    steps.step_6 = function()
        do
            local temp_1, temp_6, temp_7
            temp_1 = captures[8].value
            temp_6 = {temp_1.WorldToViewportPoint(temp_1, J.Position)}
            temp_7 = temp_6[1]
            branch_result = temp_6[2]
            A = temp_7
        end
        if branch_result then
            do
                local temp_14
                temp_14 = (Vector2.new(A.X, A.Y) - X).Magnitude
                branch_result = (temp_14 < l)
                K = temp_14
            end
            if branch_result then
                branch_result = captures[1].value.AimbotWallCheck
                if branch_result then
                    do
                        local temp_4, temp_44
                        temp_4 = RaycastParams.new()
                        temp_4.FilterDescendantsInstances = {captures[5].value.Character, captures[9].value}
                        temp_4.FilterType = Enum.RaycastFilterType.Exclude
                        temp_44 = workspace.Raycast(workspace, captures[8].value.CFrame.Position, ((J.Position - captures[8].value.CFrame.Position).Unit * 1000), temp_4)
                        branch_result = temp_44
                        n, y = temp_44, temp_44
                    end
                    if branch_result then
                        do
                            local temp_3
                            temp_3 = n.Instance
                            branch_result = temp_3
                            Q = temp_3
                        end
                        if branch_result then
                            do
                                local temp_3
                                temp_3 = n.Instance
                                Q = temp_3.IsDescendantOf(temp_3, a.Character)
                            end
                        end
                        y = Q
                    end
                    branch_result = y
                    if branch_result then
                        B, l = a, K
                    end
                else
                    B, l = a, K
                end
            end
        end
        return "step_7"
    end
    steps.step_7 = function()

        return "step_8"
    end
    steps.step_8 = function()

        return "step_2"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_57; bloques originales: 60
callbacks.callback_57 = function(captures, arguments)
    local B, I, J, X, a, branch_result, g, l, o, q, u
    local e7 = {}
    branch_result = (not captures[1].value.ScriptActive)
    if (not branch_result) then
        branch_result = captures[1].value.FlyEnabled
        if branch_result then
            do
                local temp_4
                temp_4 = captures[5].value.Character
                branch_result = temp_4
                X = temp_4
            end
            if branch_result then
                do
                    local temp_4, temp_8
                    temp_4 = X.FindFirstChild(X, "HumanoidRootPart")
                    temp_8 = X.FindFirstChildOfClass(X, "Humanoid")
                    branch_result = temp_4
                    B, I, l = temp_4, temp_4, temp_8
                end
                if branch_result then
                    I = l
                end
                branch_result = I
                if branch_result then
                    do
                        local temp_4
                        temp_4 = B.FindFirstChild(B, "KaiserFlyBV")
                        branch_result = (not temp_4)
                        u = temp_4
                    end
                    if branch_result then
                        do
                            local temp_6
                            temp_6 = Instance.new("BodyVelocity")
                            temp_6.Name = "KaiserFlyBV"
                            temp_6.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
                            temp_6.Velocity = Vector3.zero
                            temp_6.Parent = B
                            u = temp_6
                        end
                    end
                    do
                        local temp_3
                        temp_3 = l.MoveDirection
                        branch_result = (temp_3.Magnitude > 0)
                        o = temp_3
                    end
                    if branch_result then
                        u.Velocity = (Vector3.new(o.X, workspace.CurrentCamera.CFrame.LookVector.Y, o.Z).Unit * captures[1].value.FlySpeed)
                    else
                        u.Velocity = Vector3.zero
                    end
                end
            end
        end
        do
            local temp_1, temp_4
            temp_1 = captures[7].value
            temp_4 = {ipairs(unpack_values({temp_1.GetPlayers(temp_1)}))}
            B, X, l = temp_4[2], temp_4[1], temp_4[3]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = X(B, l)
                branch_result = temp_1
                l, o = temp_1, temp_2
            end
            if (not branch_result) then
                do
                    local temp_58
                    captures[4].value.Visible = captures[1].value.ShowFOV
                    captures[9].value.Color = captures[1].value.FOVColor
                    captures[9].value.Thickness = captures[1].value.FOVThickness
                    captures[4].value.Size = UDim2.new(0, (captures[1].value.FOVRadius * 2), 0, (captures[1].value.FOVRadius * 2))
                    temp_58 = Vector2.new((captures[10].value.ViewportSize.X / 2), (captures[10].value.ViewportSize.Y / 2))
                    branch_result = captures[1].value.FOVIsMobile
                    B, X = temp_58, temp_58
                end
                if branch_result then
                    do
                        local temp_1
                        temp_1 = captures[11].value
                        captures[4].value.Position = UDim2.new(0, B.X, 0, (B.Y - temp_1.GetGuiInset(temp_1).Y))
                    end
                else
                    do
                        local temp_1, temp_3, temp_4
                        temp_1 = captures[12].value
                        temp_3 = temp_1.GetMouseLocation(temp_1)
                        temp_4 = captures[11].value
                        captures[4].value.Position = UDim2.new(0, temp_3.X, 0, (temp_3.Y - temp_4.GetGuiInset(temp_4).Y))
                        X = temp_3
                    end
                end
                branch_result = captures[1].value.AimbotEnabled
                if branch_result then
                    do
                        local temp_2
                        temp_2 = captures[13].value(X)
                        branch_result = temp_2
                        o, u = temp_2, temp_2
                    end
                    if branch_result then
                        u = o.Character
                    end
                    branch_result = u
                    if branch_result then
                        do
                            local temp_5
                            temp_5 = captures[14].value(o.Character)
                            branch_result = temp_5
                            g = temp_5
                        end
                        if branch_result then
                            captures[10].value.CFrame = CFrame.new(captures[10].value.CFrame.Position, g.Position)
                        end
                    end
                end
                return unpack_values({})
            end
            do
                local temp_2
                temp_2 = (o ~= captures[5].value)
                branch_result = temp_2
                g = temp_2
            end
            if branch_result then
                g = o.Character
            end
            branch_result = g
            if branch_result then
                do
                    local temp_10, temp_14, temp_3, temp_7
                    temp_3 = o.Character
                    temp_7 = temp_3.FindFirstChild(temp_3, "HumanoidRootPart")
                    temp_10 = o.Character
                    temp_14 = temp_10.FindFirstChildOfClass(temp_10, "Humanoid")
                    branch_result = temp_7
                    a, g, q = temp_7, temp_7, temp_14
                end
                if branch_result then
                    branch_result = q
                    J = q
                    if branch_result then
                        J = (q.Health > 0)
                    end
                    a = J
                end
                branch_result = a
                if branch_result then
                    do
                        local temp_4
                        temp_4 = captures[1].value.HitboxEnabled
                        branch_result = temp_4
                        a = temp_4
                    end
                    if branch_result then
                        do
                            local temp_5
                            temp_5 = (not captures[1].value.AimbotTeamCheck)
                            branch_result = temp_5
                            J = temp_5
                        end
                        if (not branch_result) then
                            J = captures[8].value(o)
                        end
                        a = J
                    end
                    do
                        local temp_3, temp_7
                        temp_3 = o.Character
                        temp_7 = temp_3.FindFirstChild(temp_3, "KaiserHitboxPart")
                        branch_result = a
                        J = temp_7
                    end
                    if branch_result then
                        branch_result = (not J)
                        if branch_result then
                            do
                                local temp_49, temp_6
                                temp_6 = Instance.new("Part")
                                temp_6.Name = "KaiserHitboxPart"
                                temp_6.Shape = Enum.PartType.Block
                                temp_6.CanCollide = false
                                temp_6.Massless = true
                                existingPartCastShadow = false
                                temp_6.Material = Enum.Material.ForceField
                                temp_6.CFrame = g.CFrame
                                temp_6.Parent = o.Character
                                temp_49 = Instance.new("WeldConstraint")
                                temp_49.Name = "KaiserHitboxWeld"
                                temp_49.Part0 = g
                                temp_49.Part1 = temp_6
                                temp_49.Parent = temp_6
                                J = temp_6
                            end
                        end
                        J.Size = Vector3.new(captures[1].value.HitboxSize, captures[1].value.HitboxSize, captures[1].value.HitboxSize)
                        J.Transparency = ((captures[1].value.HitboxVisible and 0.6) or 1)
                        J.Color = captures[1].value.ChamsColor
                    else
                        branch_result = J
                        if branch_result then
                            J.Destroy(J)
                        end
                    end
                else
                    do
                        local temp_3, temp_7
                        temp_3 = o.Character
                        temp_7 = temp_3.FindFirstChild(temp_3, "KaiserHitboxPart")
                        branch_result = temp_7
                        J = temp_7
                    end
                    if branch_result then
                        J.Destroy(J)
                    end
                end
            end
        end
    end
    do
        local temp_8
        captures[4].value.Visible = false
        temp_8 = captures[5].value.Character
        branch_result = temp_8
        X = temp_8
    end
    if branch_result then
        do
            local temp_4
            temp_4 = X.FindFirstChild(X, "HumanoidRootPart")
            branch_result = temp_4
            B = temp_4
        end
        if branch_result then
            do
                local temp_4
                temp_4 = B.FindFirstChild(B, "KaiserFlyBV")
                branch_result = temp_4
                l = temp_4
            end
            if branch_result then
                l.Destroy(l)
            end
        end
    end
    captures[6].value()
    return unpack_values({})
end

-- callback_58; bloques originales: 7
callbacks.callback_58 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = arguments[1]
    if branch_result then
        captures[1].value.UIScale = 1
        branch_result = captures[4].value
        if branch_result then
            captures[4].value.Scale = 1
        end
        branch_result = captures[5].value
        if branch_result then
            captures[5].value()
        end
        task.delay(0.3, bind(callbacks.callback_129, {}))
    end
    return unpack_values({})
end

-- callback_59; bloques originales: 1
callbacks.callback_59 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.NotificationsEnabled = arguments[1]
    return unpack_values({})
end

-- callback_60; bloques originales: 1
callbacks.callback_60 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value((not captures[2].value.Visible))
    return unpack_values({})
end

-- callback_61; bloques originales: 1
callbacks.callback_61 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_4
        temp_1 = captures[1].value
        temp_4 = arguments[1]
        temp_1.FloatingButtonEnabled = temp_4
        captures[4].value.Visible = temp_4
        return unpack_values({})
    end
end

-- callback_62; bloques originales: 5
callbacks.callback_62 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_2, temp_28, temp_31, temp_57, temp_70, temp_75, temp_79, temp_84, temp_85
        captures[1].value = true
        temp_2 = captures[2].value
        temp_28 = temp_2.Create(temp_2, captures[3].value, TweenInfo.new(0.18, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {["Position"] = UDim2.new(1, -21, 0.5, -9)})
        temp_28.Play(temp_28)
        temp_31 = captures[2].value
        temp_57 = temp_31.Create(temp_31, captures[6].value, TweenInfo.new(0.18, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {["BackgroundColor3"] = captures[7].value.PanelColor})
        temp_57.Play(temp_57)
        task.wait(0.25)
        captures[7].value.UIScale = 1
        captures[8].value.Scale = 1
        temp_70 = captures[9].value
        temp_75 = UDim2.new
        temp_79 = captures[10].value.X
        temp_84 = temp_75(0, temp_79, 0, captures[10].value.Y)
        temp_70.Size = temp_84
        temp_85 = captures[11].value
        branch_result = temp_85
    end
    if branch_result then
        captures[11].value.Text = "1.00x"
    end
    captures[12].value.Visible = false
    captures[13].value()
    captures[14].value("KaiserHub", "Tama帽o del panel reiniciado")
    captures[3].value.Position = UDim2.new(0, 3, 0.5, -9)
    captures[6].value.BackgroundColor3 = Color3.fromRGB(50, 50, 55)
    captures[1].value = false
    return unpack_values({})
end

-- callback_63; bloques originales: 4
callbacks.callback_63 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_29
        temp_1 = captures[1].value
        temp_29 = (math.round((math.clamp(((temp_1.GetMouseLocation(temp_1).X - captures[4].value.AbsolutePosition.X) / captures[5].value.X), 0.5, 1.5) * 100)) / 100)
        captures[6].value.UIScale = temp_29
        captures[7].value.Scale = temp_29
        captures[4].value.Size = UDim2.new(0, (captures[5].value.X * temp_29), 0, (captures[5].value.Y * temp_29))
        captures[8].value.Text = string.format("%.2fx", temp_29)
        branch_result = (temp_29 <= 0.6)
    end
    if branch_result then
        ResetSizeBtn.Visible = true
    else
        ResetSizeBtn.Visible = false
    end
    return unpack_values({})
end

-- callback_64; bloques originales: 7
callbacks.callback_64 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = true
        _G.KaiserGripDragging = true
        branch_result = captures[4].value
        if branch_result then
            do
                local temp_1
                temp_1 = captures[4].value
                temp_1.Disconnect(temp_1)
            end
        end
        do
            local temp_4
            temp_4 = captures[5].value.RenderStepped
            captures[4].value = temp_4.Connect(temp_4, bind(callbacks.callback_11, {captures[3], captures[6]}))
        end
    end
    return unpack_values({})
end

-- callback_65; bloques originales: 9
callbacks.callback_65 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        branch_result = (captures[3].value == true)
        if branch_result then
            captures[3].value = false
            _G.KaiserGripDragging = false
            branch_result = captures[4].value
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[4].value
                    temp_1.Disconnect(temp_1)
                    captures[4].value = nil
                end
            end
            captures[5].value()
        end
    end
    return unpack_values({})
end

-- callback_66; bloques originales: 21
callbacks.callback_66 = function(captures, arguments)
    local B, X, branch_result, l, o, u
    local e7 = {}
    do
        local temp_31
        captures[1].value.UIScale = 1
        captures[4].value.Scale = 1
        captures[5].value.Size = UDim2.new(0, captures[6].value.X, 0, captures[6].value.Y)
        captures[7].value.Text = "1.0x"
        temp_31 = {pairs(captures[1].value.Binds)}
        B, X, l = temp_31[3], temp_31[2], temp_31[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B = temp_1
        end
        if (not branch_result) then
            do
                local temp_101, temp_103, temp_107, temp_110, temp_113, temp_116, temp_119, temp_120,
                    temp_123, temp_124, temp_128, temp_132, temp_134, temp_137
                captures[1].value.ChamsEnabled = true
                captures[1].value.EspBoxEnabled = false
                captures[1].value.EspLineEnabled = false
                captures[1].value.EspHealthEnabled = false
                captures[1].value.ChamsColor = Color3.fromRGB(160, 32, 240)
                captures[1].value.EspBoxColor = Color3.fromRGB(0, 255, 0)
                captures[1].value.EspLineColor = Color3.fromRGB(255, 0, 0)
                captures[1].value.SpeedEnabled = false
                captures[1].value.SpeedValue = 50
                captures[1].value.JumpEnabled = false
                captures[1].value.JumpValue = 100
                captures[1].value.NoclipEnabled = false
                captures[1].value.InvisibleEnabled = false
                captures[1].value.InvisibleFloatEnabled = false
                captures[1].value.KillAuraFloatEnabled = false
                captures[1].value.AutoFarmEnabled = false
                captures[1].value.FlyEnabled = false
                captures[1].value.FlySpeed = 150
                captures[1].value.AimbotEnabled = false
                captures[1].value.AimbotPartIndex = 1
                captures[1].value.HitboxEnabled = false
                captures[1].value.HitboxSize = 8
                captures[1].value.HitboxVisible = true
                captures[1].value.KillAuraEnabled = false
                temp_101 = captures[9].value
                temp_101()
                temp_103 = captures[1].value
                temp_103.ShowFOV = false
                temp_107 = captures[1].value
                temp_107.FOVRadius = 150
                temp_110 = captures[1].value
                temp_110.FOVThickness = 3
                temp_113 = captures[1].value
                temp_113.FOVColorIndex = 1
                temp_116 = captures[1].value
                temp_119 = captures[10].value
                temp_120 = temp_119[1]
                temp_123 = temp_120.Color
                temp_116.FOVColor = temp_123
                temp_124 = captures[1].value
                temp_124.NotificationsEnabled = true
                temp_128 = captures[1].value
                temp_128.FloatingButtonEnabled = true
                temp_132 = captures[11].value
                temp_132()
                temp_134 = captures[12].value
                temp_137 = temp_134.Character
                branch_result = temp_137
                X = temp_137
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = captures[12].value.Character
                    X = temp_4.FindFirstChild(temp_4, "Humanoid")
                end
            end
            branch_result = X
            if branch_result then
                do
                    local temp_32, temp_36
                    captures[12].value.Character.Humanoid.WalkSpeed = 16
                    captures[12].value.Character.Humanoid.UseJumpPower = true
                    captures[12].value.Character.Humanoid.JumpPower = 50
                    temp_32 = captures[12].value.Character
                    temp_36 = temp_32.FindFirstChild(temp_32, "HumanoidRootPart")
                    branch_result = temp_36
                    B, X = temp_36, temp_36
                end
                if branch_result then
                    B = X.FindFirstChild(X, "KaiserFlyBV")
                end
                branch_result = B
                if branch_result then
                    do
                        local temp_3
                        temp_3 = X.KaiserFlyBV
                        temp_3.Destroy(temp_3)
                    end
                end
            end
            do
                local temp_2
                temp_2 = {pairs(captures[13].value)}
                B, X, l = temp_2[2], temp_2[1], temp_2[3]
            end
            while true do
                do
                    local temp_1, temp_2
                    temp_1, temp_2 = X(B, l)
                    branch_result = temp_1
                    l, o = temp_1, temp_2
                end
                if (not branch_result) then
                    captures[14].value(false)
                    UpdateGhostButtonColor()
                    captures[15].value.Visible = false
                    bind(callbacks.callback_99, {captures[1], captures[2], captures[3]})
                    captures[16].value.Visible = false
                    captures[17].value.Visible = true
                    branch_result = captures[18].value
                    if branch_result then
                        captures[18].value.BackgroundColor3 = captures[1].value.FOVColor
                    end
                    do
                        local temp_12, temp_8
                        SetActivePanelColor(unpack_values({Color3.fromRGB(255, 60, 60)}))
                        captures[19].value()
                        temp_8 = captures[20].value
                        temp_12 = {}
                        temp_8("KaiserHub", "Script Reseteado Con Exito")
                        return unpack_values(temp_12)
                    end
                end
                branch_result = (captures[1].value[l] ~= nil)
                u = l
                if branch_result then
                    o(captures[1].value[u])
                end
            end
        end
        captures[1].value.Binds[B] = ""
        branch_result = captures[8].value[B]
        u = B
        if branch_result then
            captures[8].value[u].Text = "NONE"
            captures[8].value[u].TextColor3 = Color3.fromRGB(255, 200, 0)
        end
    end
end

-- callback_67; bloques originales: 11
callbacks.callback_67 = function(captures, arguments)
    local B, X, branch_result, g, l, o, q, u
    local e7 = {}
    do
        local temp_1, temp_100, temp_101, temp_102, temp_103, temp_11, temp_16, temp_20, temp_52, temp_72,
            temp_75, temp_78, temp_82, temp_86, temp_89, temp_90, temp_91, temp_92, temp_95, temp_96,
            temp_97, temp_98, temp_99
        temp_1 = arguments[1]
        captures[1].value.PanelColor = temp_1
        captures[4].value.BackgroundColor3 = temp_1
        captures[5].value.Color = temp_1
        temp_11 = captures[6].value
        temp_16 = ColorSequence.new
        temp_20 = ColorSequenceKeypoint.new(0, temp_1)
        temp_52 = ColorSequenceKeypoint.new(0.25, unpack_values({Color3.new(math.clamp((temp_1.R + 0.2), 0, 1), math.clamp((temp_1.G + 0.2), 0, 1), unpack_values({math.clamp((temp_1.B + 0.2), 0, 1)}))}))
        temp_72 = ColorSequenceKeypoint.new(0.5, unpack_values({Color3.new((temp_1.R * 0.12), (temp_1.G * 0.12), (temp_1.B * 0.12))}))
        temp_75 = ColorSequenceKeypoint.new
        temp_78 = Color3.new
        temp_82 = (temp_1.R * 0.06)
        temp_86 = (temp_1.G * 0.06)
        temp_89 = temp_1.B
        temp_90 = (temp_89 * 0.06)
        temp_91 = {temp_78(temp_82, temp_86, temp_90)}
        temp_92 = temp_75(0.75, unpack_values(temp_91))
        temp_95 = ColorSequenceKeypoint.new
        temp_96 = {temp_95(1, temp_1)}
        temp_97 = {temp_20, temp_52, temp_72, temp_92, unpack_values(temp_96)}
        temp_98 = temp_16(temp_97)
        temp_11.Color = temp_98
        temp_99 = captures[7].value
        temp_100 = {ipairs(temp_99)}
        temp_101 = temp_100[3]
        temp_102 = temp_100[1]
        temp_103 = temp_100[2]
        B, X, l, u = temp_103, temp_1, temp_101, temp_102
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = u(B, l)
            branch_result = temp_1
            g, l = temp_2, temp_1
        end
        if not branch_result then break end
        g.Update()
    end
    do
        local temp_2
        temp_2 = {pairs(captures[8].value)}
        B, l, u = temp_2[1], temp_2[2], temp_2[3]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = B(l, u)
            branch_result = temp_1
            g, u = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({})
        end
        do
            local temp_2
            temp_2 = captures[9].value[u]
            branch_result = temp_2
            o, q = u, temp_2
        end
        if branch_result then
            q = captures[9].value[o].Visible
        end
        branch_result = q
        if branch_result then
            g.BackgroundColor3 = X
        end
    end
end

-- callback_68; bloques originales: 1
callbacks.callback_68 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({})
end

-- build_modern_interface; bloques originales: 25
callbacks.build_modern_interface = function(captures, arguments)
    local A, Ah, B, B7, Bh, Ch, D, Dh, E7, F, Fh, G, Gh, H7, I, I7, J, Jh, K, Kh, L7, M, Mh, O, Oh, P, Ph, Q,
        Qh, R, Rh, S, Sh, Th, U7, Uh, V, Vh, Wh, X, X7, Xh, Yh, a, ah, b, branch_result, c7, dh, eh, fh, gh,
        h7, hh, i7, jh, k7, l, l7, m, mh, n, nh, o, o7, p7, ph, q, qh, rh, scratch_1, scratch_101,
        scratch_103, scratch_106, scratch_107, scratch_108, scratch_109, scratch_11, scratch_114,
        scratch_116, scratch_12, scratch_120, scratch_121, scratch_122, scratch_123, scratch_124,
        scratch_125, scratch_13, scratch_15, scratch_16, scratch_17, scratch_18, scratch_2, scratch_20,
        scratch_25, scratch_26, scratch_27, scratch_3, scratch_35, scratch_37, scratch_4, scratch_43,
        scratch_45, scratch_47, scratch_5, scratch_52, scratch_54, scratch_58, scratch_59, scratch_60,
        scratch_63, scratch_64, scratch_65, scratch_66, scratch_67, scratch_68, scratch_69, scratch_7,
        scratch_70, scratch_72, scratch_73, scratch_75, scratch_76, scratch_77, scratch_79, scratch_80,
        scratch_81, scratch_82, scratch_85, scratch_9, scratch_92, scratch_93, scratch_95, scratch_97, sh,
        th, u, u7, uh, v7, w, wh, x, yh, z, zh
    local e7 = {}
    do
        local temp_12, temp_13, temp_17, temp_18, temp_22, temp_23, temp_27, temp_28, temp_32, temp_36,
            temp_37, temp_41, temp_42, temp_46, temp_47, temp_51, temp_52, temp_56, temp_7, temp_8
        print("隆Ejecutando Kaiser Modern Gui!")
        temp_7 = game.GetService(game, "Players")
        temp_8 = {}
        temp_8.value = temp_7
        temp_12 = game.GetService(game, "RunService")
        temp_13 = {}
        temp_13.value = temp_12
        temp_17 = game.GetService(game, "CoreGui")
        temp_18 = {}
        temp_18.value = temp_17
        temp_22 = game.GetService(game, "UserInputService")
        temp_23 = {}
        temp_23.value = temp_22
        temp_27 = game.GetService(game, "TweenService")
        temp_28 = {}
        temp_28.value = temp_27
        temp_32 = game.GetService(game, "ReplicatedStorage")
        temp_36 = game.GetService(game, "TeleportService")
        temp_37 = {}
        temp_37.value = temp_36
        temp_41 = game.GetService(game, "HttpService")
        temp_42 = {}
        temp_42.value = temp_41
        temp_46 = temp_8.value.LocalPlayer
        temp_47 = {}
        temp_47.value = temp_46
        temp_51 = game.GetService(game, "Stats")
        temp_52 = {}
        temp_52.value = temp_51
        temp_56 = temp_32.FindFirstChild(temp_32, "Packages")
        branch_result = temp_56
        A, B, D, J, K, X, a, l, o, q, u, z = temp_52, temp_13, temp_56, temp_47, temp_56, temp_8, temp_42, temp_18, temp_28, temp_37, temp_23, temp_56
    end
    if branch_result then
        K = z.FindFirstChild(z, "Net")
    end
    do
        local temp_10, temp_11, temp_13, temp_6
        temp_6 = {}
        temp_6.value = "KaiserHub_ConfigB"
        temp_10 = (temp_6.value .. "/KaiserHub_Config.json")
        temp_11 = {}
        temp_11.value = temp_10
        bind(callbacks.callback_104, {temp_6})
        temp_13 = {}
        temp_13.value = {}
        branch_result = firetouchinterest
        I, M, Q, V, n = firetouchinterest, temp_6, temp_13, D, temp_11
    end
    if (not branch_result) then
        branch_result = totouchinterest
        S = totouchinterest
        if branch_result then
            S = bind(callbacks.callback_9, {})
        end
        I = S
    end
    do
        local temp_1, temp_2
        temp_1 = {}
        temp_1.value = I
        temp_2 = l.value
        branch_result = temp_2.FindFirstChild(temp_2, "KaiserUniversalGUI")
        V = temp_1
    end
    if branch_result then
        do
            local temp_4
            temp_4 = l.value.KaiserUniversalGUI
            temp_4.Destroy(temp_4)
        end
    end
    do
        local temp_1
        temp_1 = l.value
        branch_result = temp_1.FindFirstChild(temp_1, "KaiserESP2D")
    end
    if branch_result then
        do
            local temp_4
            temp_4 = l.value.KaiserESP2D
            temp_4.Destroy(temp_4)
        end
    end
    do
        local temporary = {}
        temporary[6] = Instance.new("ScreenGui")
        temporary[7] = {}
        temporary[7].value = temporary[6]
        temporary[7].value.Name = "KaiserESP2D"
        temporary[7].value.Parent = l.value
        temporary[7].value.IgnoreGuiInset = true
        temporary[87] = {{["Name"] = "Blanco", ["Color"] = Color3.fromRGB(255, 255, 255)}, {["Name"] = "Rojo", ["Color"] = Color3.fromRGB(255, 0, 0)}, {["Name"] = "Azul Fuerte", ["Color"] = Color3.fromRGB(0, 85, 255)}, {["Name"] = "Verde Aqua", ["Color"] = Color3.fromRGB(0, 255, 255)}, {["Name"] = "Verde Claro", ["Color"] = Color3.fromRGB(0, 255, 0)}, {["Name"] = "Morado", ["Color"] = Color3.fromRGB(180, 100, 255)}}
        temporary[88] = {}
        temporary[88].value = temporary[87]
        temporary[116] = Color3.fromRGB(255, 255, 255)
        temporary[122] = Color3.fromRGB(255, 255, 255)
        temporary[128] = Color3.fromRGB(255, 255, 255)
        temporary[212] = temporary[88].value[1].Color
        temporary[229] = Color3.fromRGB(200, 200, 180)
        temporary[259] = {["ChamsEnabled"] = true, ["EspBoxEnabled"] = true, ["EspLineEnabled"] = true, ["EspLinePosition"] = "Arriba", ["EspHealthEnabled"] = true, ["EspNameEnabled"] = true, ["EspDistanceEnabled"] = true, ["ChamsColor"] = temporary[116], ["EspBoxColor"] = temporary[122], ["EspLineColor"] = temporary[128], ["SpeedEnabled"] = false, ["SpeedValue"] = 50, ["JumpEnabled"] = false, ["JumpValue"] = 100, ["NoclipEnabled"] = false, ["InvisibleEnabled"] = false, ["InvisibleFloatEnabled"] = false, ["FlyEnabled"] = false, ["FlySpeed"] = 50, ["AimbotEnabled"] = false, ["AutoShootEnabled"] = false, ["AimbotWallCheck"] = true, ["AimbotTeamCheck"] = true, ["AimbotPartIndex"] = 1, ["HitboxEnabled"] = false, ["HitboxSize"] = 38, ["HitboxVisible"] = false, ["KillAuraEnabled"] = false, ["AutoEquipKnifeEnabled"] = false, ["KillAuraFloatEnabled"] = false, ["AntiLagEnabled"] = false, ["SelectedTargetName"] = "Ninguno", ["AutoFarmEnabled"] = true, ["ShowFOV"] = false, ["FOVIsMobile"] = false, ["FOVRadius"] = 150, ["FOVThickness"] = 3, ["FOVColorIndex"] = 1, ["FOVColor"] = temporary[212], ["NotificationsEnabled"] = true, ["NotificationDuration"] = 2, ["ScriptActive"] = true, ["FloatingButtonEnabled"] = true, ["PanelColor"] = temporary[229], ["UIScale"] = 1, ["Binds"] = {["ToggleUI"] = "", ["ToggleAimbot"] = "", ["ToggleHitbox"] = "", ["ToggleHitboxVisible"] = "", ["ToggleKillAura"] = "", ["ToggleInvisible"] = ""}}
        temporary[260] = {}
        temporary[260].value = temporary[259]
        temporary[261] = {}
        temporary[262] = {}
        temporary[263] = {}
        temporary[262].value = temporary[261]
        temporary[266] = {}
        temporary[267] = Vector2.new
        temporary[268] = {}
        temporary[269] = temporary[267](600, 360)
        temporary[270] = {}
        temporary[270].value = temporary[269]
        temporary[271] = {}
        temporary[272] = {}
        temporary[273] = {}
        temporary[274] = {}
        temporary[275] = bind(callbacks.callback_132, {J, captures[1], captures[2], B})
        temporary[276] = {}
        temporary[274].value = temporary[273]
        temporary[277] = {}
        temporary[276].value = temporary[277]
        temporary[278] = {}
        temporary[272].value = nil
        temporary[279] = {}
        temporary[278].value = nil
        temporary[271].value = nil
        temporary[280] = {}
        temporary[281] = bind(callbacks.callback_133, {temporary[260], captures[1], captures[2], Q, temporary[272], temporary[278], J, temporary[271], temporary[7], l})
        temporary[266].value = temporary[281]
        temporary[286] = {}
        temporary[293] = {}
        temporary[295] = {}
        temporary[297] = {}
        temporary[302] = bind(callbacks.callback_134, {})
        temporary[303] = temporary[302]("https://files.catbox.moe/54lm4f.jpg", "KaiserHub_Background_Custom.jpg116")
        temporary[304] = temporary[302]("https://files.catbox.moe/rw57oe.jpg", "KaiserHub_FloatingButton_Custom.jpg23")
        temporary[305] = temporary[302]("https://files.catbox.moe/jdq3rw.jpeg", "Kaiser_KillAura_Custom3.jpeg")
        temporary[306] = temporary[302]("https://files.catbox.moe/1d36pv.jpeg", "Kaiser_GhostButton_Custom3.jpeg")
        temporary[307] = {}
        temporary[308] = bind(callbacks.callback_135, {captures[1], captures[2], Q, u, B})
        temporary[268].value = nil
        temporary[309] = bind(callbacks.callback_136, {temporary[268], captures[1], captures[2], temporary[260], n, a})
        temporary[293].value = temporary[309]
        temporary[310] = {}
        temporary[311] = bind(callbacks.callback_137, {n, a, captures[1], captures[2], temporary[260], temporary[88]})
        temporary[312] = {}
        temporary[311]()
        temporary[279].value = false
        temporary[297].value = nil
        temporary[310].value = nil
        temporary[280].value = nil
        temporary[315] = {}
        temporary[263].value = temporary[315]
        temporary[286].value = nil
        temporary[316] = bind(callbacks.callback_138, {J, captures[1], captures[2], temporary[297], temporary[310], temporary[280], temporary[263]})
        temporary[295].value = temporary[316]
        temporary[317] = bind(callbacks.callback_139, {temporary[260], captures[1], captures[2], temporary[279], J, temporary[263], temporary[297], temporary[310], temporary[280], temporary[295]})
        temporary[307].value = temporary[317]
        temporary[320] = table.insert
        temporary[321] = Q.value
        temporary[322] = B.value
        temporary[325] = temporary[322].Stepped
        temporary[326] = temporary[325].Connect
        temporary[327] = bind(callbacks.callback_140, {temporary[260], captures[1], captures[2], J})
        temporary[328] = {temporary[326](temporary[325], temporary[327])}
        temporary[320](temporary[321], unpack_values(temporary[328]))
        temporary[332] = table.insert
        temporary[333] = Q.value
        temporary[334] = B.value
        temporary[337] = bind(callbacks.callback_141, {captures[1], captures[2]})
        temporary[338] = temporary[334].RenderStepped
        temporary[339] = temporary[338].Connect
        temporary[340] = bind(callbacks.callback_142, {temporary[260], captures[1], captures[2], temporary[297], temporary[280], temporary[310], J, temporary[286]})
        temporary[341] = {temporary[339](temporary[338], temporary[340])}
        temporary[332](temporary[333], unpack_values(temporary[341]))
        temporary[343] = {}
        bind(callbacks.callback_143, {captures[1], captures[2], J})
        temporary[345] = {}
        temporary[346] = {}
        temporary[347] = {}
        temporary[348] = {}
        temporary[349] = {}
        temporary[345].value = temporary[349]
        temporary[350] = {}
        temporary[351] = bind(callbacks.callback_144, {captures[1], captures[2], J, A, temporary[345]})
        temporary[347].value = temporary[351]
        temporary[352] = {}
        temporary[348].value = temporary[352]
        temporary[350].value = 0.5
        temporary[353] = bind(callbacks.callback_145, {J, temporary[260], captures[1], captures[2], temporary[348], temporary[350]})
        temporary[343].value = temporary[353]
        temporary[354] = {}
        temporary[355] = bind(callbacks.callback_146, {temporary[260], captures[1], captures[2]})
        temporary[346].value = temporary[355]
        temporary[356] = bind(callbacks.callback_147, {X, captures[1], captures[2]})
        temporary[278].value = temporary[356]
        temporary[354].value = nil
        temporary[357] = {}
        temporary[357].value = temporary[337]
        temporary[358] = bind(callbacks.callback_148, {temporary[354], temporary[346], captures[1], captures[2], temporary[357]})
        temporary[359] = {}
        temporary[359].value = temporary[358]
        temporary[360] = {}
        temporary[360].value = temporary[275]
        temporary[365] = Vector3.new
        temporary[366] = temporary[365](-320.5, 280.82, 16)
        temporary[369] = {["Centro"] = temporary[366], ["Radio"] = 500}
        temporary[374] = Vector3.new
        temporary[375] = temporary[374](1564.14, -155.45, 40.04)
        temporary[378] = {["Centro"] = temporary[375], ["Radio"] = 300}
        temporary[379] = {temporary[369], temporary[378]}
        temporary[380] = {}
        temporary[381] = bind(callbacks.callback_149, {temporary[343]})
        temporary[382] = {}
        temporary[382].value = temporary[379]
        temporary[383] = {}
        temporary[384] = bind(callbacks.callback_150, {J, captures[1], captures[2], temporary[382]})
        temporary[385] = bind(callbacks.callback_151, {X, captures[1], captures[2]})
        temporary[386] = bind(callbacks.callback_152, {captures[1], captures[2]})
        temporary[383].value = temporary[381]
        temporary[387] = bind(callbacks.callback_153, {captures[1], captures[2]})
        temporary[388] = {}
        temporary[389] = {}
        temporary[389].value = temporary[387]
        temporary[390] = {}
        temporary[391] = bind(callbacks.callback_154, {J, captures[1], captures[2], temporary[389]})
        temporary[390].value = temporary[384]
        temporary[392] = {}
        temporary[392].value = temporary[386]
        temporary[393] = {}
        temporary[393].value = temporary[385]
        temporary[394] = bind(callbacks.callback_155, {captures[1], captures[2], J, temporary[393], temporary[380], X, temporary[383], temporary[392]})
        temporary[395] = {}
        temporary[380].value = nil
        temporary[396] = {}
        temporary[396].value = temporary[394]
        temporary[388].value = 1.2
        temporary[395].value = 0
        temporary[397] = {}
        temporary[397].value = temporary[391]
        temporary[398] = {}
        temporary[399] = bind(callbacks.callback_156, {J, captures[1], captures[2]})
        temporary[398].value = temporary[399]
        temporary[402] = {}
        temporary[403] = task.spawn
        temporary[404] = bind(callbacks.callback_157, {captures[1], captures[2], temporary[260], temporary[390], temporary[395], temporary[388], temporary[398], J, temporary[396], temporary[397], temporary[347], u, B})
        temporary[403](temporary[404])
        temporary[406] = {}
        temporary[407] = {}
        temporary[406].value = 250
        temporary[407].value = 0.01
        temporary[402].value = false
        temporary[411] = Vector3.new
        temporary[411](60, 60, 60)
        temporary[428] = {}
        temporary[429] = bind(callbacks.callback_158, {captures[1], captures[2], J, A})
        temporary[430] = bind(callbacks.callback_159, {J, captures[1], captures[2], V, temporary[428]})
        temporary[428].value = temporary[429]
        temporary[431] = {}
        temporary[432] = bind(callbacks.callback_160, {captures[1], captures[2]})
        temporary[433] = bind(callbacks.callback_161, {J, captures[1], captures[2], temporary[428]})
        temporary[431].value = temporary[433]
        temporary[434] = {}
        temporary[434].value = temporary[432]
        temporary[435] = bind(callbacks.callback_162, {X, temporary[343], captures[1], captures[2]})
        temporary[436] = bind(callbacks.callback_163, {captures[1], captures[2]})
        temporary[437] = {}
        temporary[438] = bind(callbacks.callback_164, {J, captures[1], captures[2], temporary[389], temporary[434]})
        temporary[437].value = temporary[438]
        temporary[439] = bind(callbacks.callback_165, {temporary[390], J, captures[1], captures[2], temporary[437], temporary[434]})
        temporary[440] = {}
        temporary[440].value = temporary[439]
        temporary[441] = {}
        temporary[441].value = temporary[430]
        temporary[442] = {}
        temporary[442].value = temporary[435]
        temporary[443] = {}
        temporary[443].value = temporary[436]
        temporary[444] = bind(callbacks.callback_166, {temporary[431], temporary[442], temporary[443], captures[1], captures[2], temporary[428], temporary[406]})
        temporary[445] = {}
        temporary[445].value = temporary[444]
        temporary[446] = {}
        temporary[447] = bind(callbacks.callback_167, {J, captures[1], captures[2], temporary[406], temporary[260], temporary[360], temporary[443], X, temporary[441]})
        temporary[446].value = temporary[447]
        temporary[448] = bind(callbacks.callback_168, {temporary[402], temporary[260], captures[1], captures[2], J, temporary[389], temporary[445], temporary[437], temporary[440], temporary[443], temporary[446], temporary[407]})
        temporary[449] = {}
        temporary[449].value = temporary[448]
        temporary[452] = task.spawn
        temporary[453] = bind(callbacks.callback_169, {temporary[260], captures[1], captures[2], B, temporary[402], J, temporary[389], temporary[445], temporary[437], temporary[440], temporary[449]})
        temporary[452](temporary[453])
        temporary[457] = task.spawn
        temporary[458] = bind(callbacks.callback_170, {captures[1], captures[2], temporary[260], o, temporary[293], Q, temporary[276], temporary[262]})
        temporary[459] = bind(callbacks.callback_171, {captures[1], captures[2], temporary[260], Q, u, temporary[293], temporary[262]})
        temporary[460] = bind(callbacks.callback_172, {captures[1], captures[2], temporary[260]})
        temporary[457](temporary[460])
        temporary[462] = bind(callbacks.callback_173, {temporary[312], captures[1], captures[2], temporary[7]})
        temporary[463] = bind(callbacks.callback_174, {captures[1], captures[2], temporary[260], temporary[274], Q, u, temporary[346], temporary[293]})
        temporary[464] = bind(callbacks.callback_175, {captures[1], captures[2]})
        temporary[465] = {}
        temporary[465].value = temporary[464]
        temporary[466] = bind(callbacks.callback_176, {captures[1], captures[2], temporary[260]})
        temporary[467] = bind(callbacks.callback_177, {captures[1], captures[2], o})
        temporary[468] = bind(callbacks.callback_178, {temporary[465], captures[1], captures[2], Q, temporary[260], temporary[293], temporary[346]})
        temporary[469] = {}
        temporary[312].value = temporary[469]
        temporary[470] = {}
        temporary[470].value = temporary[462]
        temporary[471] = bind(callbacks.callback_179, {temporary[260], captures[1], captures[2], temporary[390], temporary[312], X, J, temporary[343], temporary[470]})
        temporary[474] = table.insert
        temporary[475] = Q.value
        temporary[476] = B.value
        temporary[479] = temporary[476].RenderStepped
        temporary[480] = temporary[479].Connect
        temporary[481] = {temporary[480](temporary[479], temporary[471])}
        temporary[474](temporary[475], unpack_values(temporary[481]))
        temporary[485] = Instance.new
        temporary[488] = temporary[485]("ScreenGui")
        temporary[271].value = temporary[488]
        temporary[489] = temporary[271].value
        temporary[489].Name = "KaiserUniversalGUI"
        temporary[494] = temporary[271].value
        temporary[497] = l.value
        temporary[494].Parent = temporary[497]
        temporary[498] = temporary[271].value
        temporary[498].ResetOnSpawn = false
        temporary[504] = Instance.new
        temporary[507] = temporary[504]("ImageButton")
        temporary[508] = {}
        temporary[508].value = temporary[507]
        temporary[509] = temporary[508].value
        temporary[509].Name = "KaiserGhostButton"
        temporary[514] = temporary[508].value
        temporary[519] = UDim2.new
        temporary[520] = temporary[519](0, 55, 0, 55)
        temporary[514].Size = temporary[520]
        temporary[521] = temporary[508].value
        temporary[526] = UDim2.new
        temporary[527] = temporary[526](0.02, 0, 0.35, 0)
        temporary[521].Position = temporary[527]
        temporary[528] = temporary[508].value
        temporary[528].BackgroundTransparency = 1
        temporary[531] = temporary[508].value
        temporary[531].Image = temporary[306]
        temporary[534] = temporary[508].value
        temporary[534].Active = true
        temporary[538] = temporary[508].value
        temporary[538].AutoButtonColor = false
        temporary[542] = temporary[508].value
        temporary[545] = temporary[260].value
        temporary[548] = temporary[545].InvisibleFloatEnabled
        temporary[542].Visible = temporary[548]
        temporary[549] = temporary[508].value
        temporary[552] = temporary[271].value
        temporary[549].Parent = temporary[552]
        temporary[555] = Instance.new
        temporary[558] = temporary[555]("UICorner")
        temporary[563] = UDim.new
        temporary[564] = temporary[563](1, 0)
        temporary[558].CornerRadius = temporary[564]
        temporary[567] = temporary[508].value
        temporary[558].Parent = temporary[567]
        temporary[568] = temporary[508].value
        temporary[308](temporary[568])
        temporary[570] = {}
        temporary[572] = {}
        temporary[570].value = false
        temporary[572].value = nil
        temporary[575] = table.insert
        temporary[576] = Q.value
        temporary[577] = temporary[508].value
        temporary[580] = temporary[577].InputBegan
        temporary[581] = bind(callbacks.callback_180, {captures[1], captures[2], temporary[570], temporary[572]})
        temporary[582] = temporary[580].Connect
        temporary[583] = {temporary[582](temporary[580], temporary[581])}
        temporary[575](temporary[576], unpack_values(temporary[583]))
        temporary[587] = table.insert
        temporary[588] = Q.value
        temporary[589] = temporary[508].value
        temporary[592] = temporary[589].InputChanged
        temporary[593] = bind(callbacks.callback_181, {captures[1], captures[2], temporary[572], temporary[570]})
        temporary[594] = temporary[592].Connect
        temporary[595] = {temporary[594](temporary[592], temporary[593])}
        temporary[587](temporary[588], unpack_values(temporary[595]))
        temporary[599] = table.insert
        temporary[600] = Q.value
        temporary[601] = temporary[508].value
        temporary[604] = temporary[601].Activated
        temporary[605] = bind(callbacks.callback_182, {temporary[570], temporary[260], captures[1], captures[2], temporary[307], temporary[276], temporary[346], temporary[293]})
        temporary[606] = temporary[604].Connect
        temporary[607] = {temporary[606](temporary[604], temporary[605])}
        temporary[599](temporary[600], unpack_values(temporary[607]))
        temporary[611] = Instance.new
        temporary[614] = temporary[611]("ImageButton")
        temporary[615] = {}
        temporary[615].value = temporary[614]
        temporary[616] = temporary[615].value
        temporary[616].Name = "KaiserKillAuraButton"
        temporary[621] = temporary[615].value
        temporary[626] = UDim2.new
        temporary[627] = temporary[626](0, 55, 0, 55)
        temporary[621].Size = temporary[627]
        temporary[628] = temporary[615].value
        temporary[633] = UDim2.new
        temporary[634] = temporary[633](0.02, 0, 0.45, 0)
        temporary[628].Position = temporary[634]
        temporary[635] = temporary[615].value
        temporary[635].BackgroundTransparency = 1
        temporary[638] = temporary[615].value
        temporary[638].Image = temporary[305]
        temporary[641] = temporary[615].value
        temporary[641].Active = true
        temporary[645] = temporary[615].value
        temporary[645].AutoButtonColor = false
        temporary[649] = temporary[615].value
        temporary[652] = temporary[260].value
        temporary[655] = temporary[652].KillAuraFloatEnabled
        temporary[649].Visible = temporary[655]
        temporary[656] = temporary[615].value
        temporary[659] = temporary[271].value
        temporary[656].Parent = temporary[659]
        temporary[662] = Instance.new
        temporary[665] = temporary[662]("UICorner")
        temporary[670] = UDim.new
        temporary[671] = temporary[670](1, 0)
        temporary[665].CornerRadius = temporary[671]
        temporary[674] = temporary[615].value
        temporary[665].Parent = temporary[674]
        temporary[675] = temporary[615].value
        temporary[676] = {}
        temporary[308](temporary[675])
        temporary[678] = {}
        temporary[678].value = false
        temporary[676].value = nil
        temporary[682] = table.insert
        temporary[683] = Q.value
        temporary[684] = temporary[615].value
        temporary[687] = temporary[684].InputBegan
        temporary[688] = bind(callbacks.callback_183, {captures[1], captures[2], temporary[678], temporary[676]})
        temporary[689] = temporary[687].Connect
        temporary[690] = {temporary[689](temporary[687], temporary[688])}
        temporary[682](temporary[683], unpack_values(temporary[690]))
        temporary[694] = table.insert
        temporary[695] = Q.value
        temporary[696] = temporary[615].value
        temporary[699] = temporary[696].InputChanged
        temporary[700] = bind(callbacks.callback_184, {captures[1], captures[2], temporary[676], temporary[678]})
        temporary[701] = temporary[699].Connect
        temporary[702] = {temporary[701](temporary[699], temporary[700])}
        temporary[694](temporary[695], unpack_values(temporary[702]))
        temporary[706] = table.insert
        temporary[707] = Q.value
        temporary[708] = temporary[615].value
        temporary[711] = temporary[708].Activated
        temporary[712] = bind(callbacks.callback_185, {temporary[678], temporary[260], captures[1], captures[2], temporary[276], temporary[346], temporary[293], X})
        temporary[713] = temporary[711].Connect
        temporary[714] = {temporary[713](temporary[711], temporary[712])}
        temporary[706](temporary[707], unpack_values(temporary[714]))
        temporary[718] = Instance.new
        temporary[721] = temporary[718]("CanvasGroup")
        temporary[722] = {}
        temporary[722].value = temporary[721]
        temporary[723] = temporary[722].value
        temporary[723].Name = "MainFrame"
        temporary[728] = temporary[722].value
        temporary[733] = UDim2.new
        temporary[734] = temporary[270].value
        temporary[737] = temporary[734].X
        temporary[738] = temporary[260].value
        temporary[741] = temporary[738].UIScale
        temporary[742] = (temporary[737] * temporary[741])
        temporary[743] = temporary[270].value
        temporary[746] = temporary[743].Y
        temporary[747] = temporary[260].value
        temporary[750] = temporary[747].UIScale
        temporary[751] = (temporary[746] * temporary[750])
        temporary[752] = temporary[733](0, temporary[742], 0, temporary[751])
        temporary[728].Size = temporary[752]
        temporary[753] = temporary[722].value
        temporary[758] = UDim2.new
        temporary[759] = temporary[270].value
        temporary[762] = temporary[759].X
        temporary[763] = temporary[260].value
        temporary[766] = temporary[763].UIScale
        temporary[767] = (temporary[762] * temporary[766])
        temporary[768] = (- temporary[767])
        temporary[769] = (temporary[768] / 2)
        temporary[770] = temporary[270].value
        temporary[773] = temporary[770].Y
        temporary[774] = temporary[260].value
        temporary[777] = temporary[774].UIScale
        temporary[778] = (temporary[773] * temporary[777])
        temporary[779] = (- temporary[778])
        temporary[780] = (temporary[779] / 2)
        temporary[781] = temporary[758](0.5, temporary[769], 0.5, temporary[780])
        temporary[753].Position = temporary[781]
        temporary[782] = temporary[722].value
        temporary[787] = Color3.fromRGB
        temporary[788] = temporary[787](15, 15, 18)
        temporary[782].BackgroundColor3 = temporary[788]
        temporary[789] = temporary[722].value
        temporary[789].BackgroundTransparency = 0
        temporary[792] = temporary[722].value
        temporary[792].BorderSizePixel = 0
        temporary[795] = temporary[722].value
        temporary[795].Active = true
        temporary[799] = temporary[722].value
        temporary[802] = temporary[271].value
        temporary[799].Parent = temporary[802]
        temporary[803] = temporary[722].value
        temporary[308](temporary[803])
        temporary[807] = Instance.new
        temporary[810] = temporary[807]("UIScale")
        temporary[811] = {}
        temporary[811].value = temporary[810]
        temporary[812] = temporary[811].value
        temporary[815] = temporary[260].value
        temporary[818] = temporary[815].UIScale
        temporary[812].Scale = temporary[818]
        temporary[819] = temporary[811].value
        temporary[822] = temporary[722].value
        temporary[819].Parent = temporary[822]
        temporary[825] = Instance.new
        temporary[828] = temporary[825]("UICorner")
        temporary[833] = UDim.new
        temporary[834] = temporary[833](0, 16)
        temporary[828].CornerRadius = temporary[834]
        temporary[837] = temporary[722].value
        temporary[828].Parent = temporary[837]
        temporary[838] = {}
        temporary[838].value = false
        temporary[840] = temporary[722].value
        temporary[840].Visible = true
        temporary[844] = bind(callbacks.callback_186, {temporary[838], temporary[722], captures[1], captures[2], temporary[811], temporary[260], o})
        temporary[845] = {}
        temporary[846] = bind(callbacks.callback_187, {captures[1], captures[2], B, temporary[260], Q})
        temporary[845].value = temporary[844]
        bind(callbacks.callback_188, {temporary[260], captures[1], captures[2], temporary[811], temporary[722], temporary[270], temporary[293], temporary[346]})
        temporary[848] = temporary[722].value
        temporary[846](temporary[848])
        temporary[852] = Instance.new
        temporary[855] = temporary[852]("Frame")
        temporary[855].Name = "KaiserHub_NeonBorder"
        temporary[864] = UDim2.new
        temporary[865] = temporary[864](1, 4, 1, 4)
        temporary[855].Size = temporary[865]
        temporary[870] = UDim2.new
        temporary[871] = temporary[870](0, -2, 0, -2)
        temporary[855].Position = temporary[871]
        temporary[855].BackgroundTransparency = 1
        temporary[876] = temporary[722].value
        temporary[879] = temporary[876].ZIndex
        temporary[880] = (temporary[879] - 1)
        temporary[855].ZIndex = temporary[880]
        temporary[855].Active = false
        temporary[886] = temporary[722].value
        temporary[855].Parent = temporary[886]
        temporary[887] = temporary[828].Clone
        temporary[888] = temporary[887](temporary[828])
        temporary[888].Parent = temporary[855]
        temporary[893] = Instance.new
        temporary[896] = temporary[893]("UIStroke")
        temporary[897] = {}
        temporary[897].value = temporary[896]
        temporary[898] = temporary[897].value
        temporary[898].Thickness = 3.5
        temporary[901] = temporary[897].value
        temporary[906] = Enum.ApplyStrokeMode
        temporary[909] = temporary[906].Border
        temporary[901].ApplyStrokeMode = temporary[909]
        temporary[910] = temporary[897].value
        temporary[915] = Enum.LineJoinMode
        temporary[918] = temporary[915].Round
        temporary[910].LineJoinMode = temporary[918]
        temporary[919] = temporary[897].value
        temporary[922] = temporary[260].value
        temporary[925] = temporary[922].PanelColor
        temporary[919].Color = temporary[925]
        temporary[926] = temporary[897].value
        temporary[926].Parent = temporary[855]
        temporary[931] = Instance.new
        temporary[934] = temporary[931]("UIGradient")
        temporary[935] = {}
        temporary[935].value = temporary[934]
        temporary[936] = temporary[935].value
        temporary[941] = ColorSequence.new
        temporary[944] = ColorSequenceKeypoint.new
        temporary[945] = temporary[260].value
        temporary[948] = temporary[945].PanelColor
        temporary[949] = temporary[944](0, temporary[948])
        temporary[952] = ColorSequenceKeypoint.new
        temporary[955] = Color3.new
        temporary[958] = math.clamp
        temporary[959] = temporary[260].value
        temporary[962] = temporary[959].PanelColor
        temporary[965] = temporary[962].R
        temporary[966] = (temporary[965] + 0.2)
        temporary[967] = temporary[958](temporary[966], 0, 1)
        temporary[970] = math.clamp
        temporary[971] = temporary[260].value
        temporary[974] = temporary[971].PanelColor
        temporary[977] = temporary[974].G
        temporary[978] = (temporary[977] + 0.2)
        temporary[979] = temporary[970](temporary[978], 0, 1)
        temporary[982] = math.clamp
        temporary[983] = temporary[260].value
        temporary[986] = temporary[983].PanelColor
        temporary[989] = temporary[986].B
        temporary[990] = (temporary[989] + 0.2)
        temporary[991] = {temporary[982](temporary[990], 0, 1)}
        temporary[992] = {temporary[955](temporary[967], temporary[979], unpack_values(temporary[991]))}
        temporary[993] = temporary[952](0.25, unpack_values(temporary[992]))
        temporary[996] = ColorSequenceKeypoint.new
        temporary[999] = Color3.new
        temporary[1000] = temporary[260].value
        temporary[1003] = temporary[1000].PanelColor
        temporary[1006] = temporary[1003].R
        temporary[1007] = (temporary[1006] * 0.12)
        temporary[1008] = temporary[260].value
        temporary[1011] = temporary[1008].PanelColor
        temporary[1014] = temporary[1011].G
        temporary[1015] = (temporary[1014] * 0.12)
        temporary[1016] = temporary[260].value
        temporary[1019] = temporary[1016].PanelColor
        temporary[1022] = temporary[1019].B
        temporary[1023] = (temporary[1022] * 0.12)
        temporary[1024] = {temporary[999](temporary[1007], temporary[1015], temporary[1023])}
        temporary[1025] = temporary[996](0.5, unpack_values(temporary[1024]))
        temporary[1028] = ColorSequenceKeypoint.new
        temporary[1031] = Color3.new
        temporary[1032] = temporary[260].value
        temporary[1035] = temporary[1032].PanelColor
        temporary[1038] = temporary[1035].R
        temporary[1039] = (temporary[1038] * 0.06)
        temporary[1040] = temporary[260].value
        temporary[1043] = temporary[1040].PanelColor
        temporary[1046] = temporary[1043].G
        temporary[1047] = (temporary[1046] * 0.06)
        temporary[1048] = temporary[260].value
        temporary[1051] = temporary[1048].PanelColor
        temporary[1054] = temporary[1051].B
        temporary[1055] = (temporary[1054] * 0.06)
        temporary[1056] = {temporary[1031](temporary[1039], temporary[1047], temporary[1055])}
        temporary[1057] = temporary[1028](0.75, unpack_values(temporary[1056]))
        temporary[1060] = ColorSequenceKeypoint.new
        temporary[1061] = temporary[260].value
        temporary[1064] = temporary[1061].PanelColor
        temporary[1065] = {temporary[1060](1, temporary[1064])}
        temporary[1066] = {temporary[949], temporary[993], temporary[1025], temporary[1057], unpack_values(temporary[1065])}
        temporary[1067] = temporary[941](temporary[1066])
        temporary[936].Color = temporary[1067]
        temporary[1068] = temporary[935].value
        temporary[1071] = temporary[897].value
        temporary[1068].Parent = temporary[1071]
        temporary[1074] = TweenInfo.new
        temporary[1077] = Enum.EasingStyle
        temporary[1080] = temporary[1077].Linear
        temporary[1083] = Enum.EasingDirection
        temporary[1086] = temporary[1083].InOut
        temporary[1088] = temporary[1074](4.5, temporary[1080], temporary[1086], -1, false)
        temporary[1089] = o.value
        temporary[1090] = temporary[935].value
        temporary[1093] = temporary[1089].Create
        temporary[1094] = {["Rotation"] = 360}
        temporary[1095] = temporary[1093](temporary[1089], temporary[1090], temporary[1088], temporary[1094])
        temporary[1096] = temporary[1095].Play
        temporary[1096](temporary[1095])
        temporary[1100] = Instance.new
        temporary[1103] = temporary[1100]("UIStroke")
        temporary[1103].Thickness = 2.5
        temporary[1110] = Color3.fromRGB
        temporary[1111] = temporary[1110](0, 0, 0)
        temporary[1103].Color = temporary[1111]
        temporary[1103].Transparency = 0.65
        temporary[1116] = temporary[722].value
        temporary[1103].Parent = temporary[1116]
        temporary[1119] = Instance.new
        temporary[1122] = temporary[1119]("UIStroke")
        temporary[1122].Thickness = 1.2
        temporary[1129] = Color3.fromRGB
        temporary[1130] = temporary[1129](45, 45, 52)
        temporary[1122].Color = temporary[1130]
        temporary[1122].Transparency = 0
        temporary[1135] = temporary[722].value
        temporary[1122].Parent = temporary[1135]
        temporary[1138] = Instance.new
        temporary[1141] = temporary[1138]("Frame")
        temporary[1141].Name = "Header"
        temporary[1150] = UDim2.new
        temporary[1151] = temporary[1150](1, 0, 0, 45)
        temporary[1141].Size = temporary[1151]
        temporary[1141].BackgroundTransparency = 1
        temporary[1141].ZIndex = 2
        temporary[1158] = temporary[722].value
        temporary[1141].Parent = temporary[1158]
        temporary[1161] = Instance.new
        temporary[1164] = temporary[1161]("TextLabel")
        temporary[1169] = UDim2.new
        temporary[1170] = temporary[1169](0.6, 0, 0, 20)
        temporary[1164].Size = temporary[1170]
        temporary[1175] = UDim2.new
        temporary[1176] = temporary[1175](0, 16, 0, 6)
        temporary[1164].Position = temporary[1176]
        temporary[1164].BackgroundTransparency = 1
        temporary[1164].Text = "KaiserHub   v10.6.1"
        temporary[1187] = Color3.fromRGB
        temporary[1188] = temporary[1187](255, 255, 255)
        temporary[1164].TextColor3 = temporary[1188]
        temporary[1164].TextSize = 16
        temporary[1195] = Enum.Font
        temporary[1198] = temporary[1195].GothamBold
        temporary[1164].Font = temporary[1198]
        temporary[1203] = Enum.TextXAlignment
        temporary[1206] = temporary[1203].Left
        temporary[1164].TextXAlignment = temporary[1206]
        temporary[1164].ZIndex = 3
        temporary[1164].Parent = temporary[1141]
        temporary[1213] = Instance.new
        temporary[1216] = temporary[1213]("Frame")
        temporary[1216].Name = "CreatorProfileHeader"
        temporary[1225] = UDim2.new
        temporary[1226] = temporary[1225](0.5, 0, 0, 18)
        temporary[1216].Size = temporary[1226]
        temporary[1231] = UDim2.new
        temporary[1232] = temporary[1231](0, 16, 0, 25)
        temporary[1216].Position = temporary[1232]
        temporary[1216].BackgroundTransparency = 1
        temporary[1216].ZIndex = 3
        temporary[1216].Parent = temporary[1141]
        temporary[1241] = Instance.new
        temporary[1244] = temporary[1241]("ImageLabel")
        temporary[1245] = {}
        temporary[1245].value = temporary[1244]
        temporary[1246] = temporary[1245].value
        temporary[1246].Name = "HeaderAvatarImage"
        temporary[1251] = temporary[1245].value
        temporary[1256] = UDim2.new
        temporary[1257] = temporary[1256](0, 16, 0, 16)
        temporary[1251].Size = temporary[1257]
        temporary[1258] = temporary[1245].value
        temporary[1263] = UDim2.new
        temporary[1264] = temporary[1263](0, 0, 0.5, -8)
        temporary[1258].Position = temporary[1264]
        temporary[1265] = temporary[1245].value
        temporary[1270] = Color3.fromRGB
        temporary[1271] = temporary[1270](30, 30, 35)
        temporary[1265].BackgroundColor3 = temporary[1271]
        temporary[1272] = temporary[1245].value
        temporary[1272].ZIndex = 4
        temporary[1275] = temporary[1245].value
        temporary[1275].Parent = temporary[1216]
        temporary[1280] = Instance.new
        temporary[1283] = temporary[1280]("UICorner")
        temporary[1288] = UDim.new
        temporary[1289] = temporary[1288](1, 0)
        temporary[1283].CornerRadius = temporary[1289]
        temporary[1292] = temporary[1245].value
        temporary[1283].Parent = temporary[1292]
        temporary[1295] = Instance.new
        temporary[1298] = temporary[1295]("TextLabel")
        temporary[1299] = {}
        temporary[1299].value = temporary[1298]
        temporary[1300] = temporary[1299].value
        temporary[1300].Name = "HeaderUserLabel"
        temporary[1305] = temporary[1299].value
        temporary[1310] = UDim2.new
        temporary[1311] = temporary[1310](1, -22, 1, 0)
        temporary[1305].Size = temporary[1311]
        temporary[1312] = temporary[1299].value
        temporary[1317] = UDim2.new
        temporary[1318] = temporary[1317](0, 20, 0, 0)
        temporary[1312].Position = temporary[1318]
        temporary[1319] = temporary[1299].value
        temporary[1319].BackgroundTransparency = 1
        temporary[1322] = temporary[1299].value
        temporary[1322].Text = "Kaiser"
        temporary[1327] = temporary[1299].value
        temporary[1332] = Color3.fromRGB
        temporary[1333] = temporary[1332](200, 200, 205)
        temporary[1327].TextColor3 = temporary[1333]
        temporary[1334] = temporary[1299].value
        temporary[1339] = Enum.Font
        temporary[1342] = temporary[1339].GothamSemibold
        temporary[1334].Font = temporary[1342]
        temporary[1343] = temporary[1299].value
        temporary[1343].TextSize = 10
        temporary[1346] = temporary[1299].value
        temporary[1351] = Enum.TextXAlignment
        temporary[1354] = temporary[1351].Left
        temporary[1346].TextXAlignment = temporary[1354]
        temporary[1355] = temporary[1299].value
        temporary[1355].ClipsDescendants = true
        temporary[1359] = temporary[1299].value
        temporary[1359].ZIndex = 4
        temporary[1362] = temporary[1299].value
        temporary[1362].Parent = temporary[1216]
        temporary[1367] = task.spawn
        temporary[1368] = bind(callbacks.callback_189, {captures[1], captures[2], temporary[1299], X, temporary[1245]})
        temporary[1367](temporary[1368])
        temporary[1372] = Instance.new
        temporary[1375] = temporary[1372]("Frame")
        temporary[1380] = UDim2.new
        temporary[1381] = temporary[1380](0, 70, 0, 30)
        temporary[1375].Size = temporary[1381]
        temporary[1386] = UDim2.new
        temporary[1387] = temporary[1386](1, -80, 0, 7)
        temporary[1375].Position = temporary[1387]
        temporary[1375].BackgroundTransparency = 1
        temporary[1375].ZIndex = 3
        temporary[1375].Parent = temporary[1141]
        temporary[1396] = Instance.new
        temporary[1399] = temporary[1396]("TextButton")
        temporary[1404] = UDim2.new
        temporary[1405] = temporary[1404](0, 24, 0, 24)
        temporary[1399].Size = temporary[1405]
        temporary[1410] = UDim2.new
        temporary[1411] = temporary[1410](1, -24, 0, 3)
        temporary[1399].Position = temporary[1411]
        temporary[1416] = Color3.fromRGB
        temporary[1417] = temporary[1416](35, 22, 22)
        temporary[1399].BackgroundColor3 = temporary[1417]
        temporary[1399].Text = "脳"
        temporary[1426] = Color3.fromRGB
        temporary[1427] = temporary[1426](255, 95, 95)
        temporary[1399].TextColor3 = temporary[1427]
        temporary[1432] = Enum.Font
        temporary[1435] = temporary[1432].GothamBold
        temporary[1399].Font = temporary[1435]
        temporary[1399].TextSize = 16
        temporary[1399].ZIndex = 4
        temporary[1399].Active = true
        temporary[1399].AutoButtonColor = false
        temporary[1399].Parent = temporary[1375]
        temporary[1450] = Instance.new
        temporary[1453] = temporary[1450]("UICorner")
        temporary[1458] = UDim.new
        temporary[1459] = temporary[1458](1, 0)
        temporary[1453].CornerRadius = temporary[1459]
        temporary[1453].Parent = temporary[1399]
        temporary[1464] = table.insert
        temporary[1465] = Q.value
        temporary[1468] = bind(callbacks.callback_190, {temporary[266]})
        temporary[1469] = temporary[1399].Activated
        temporary[1470] = temporary[1469].Connect
        temporary[1471] = {temporary[1470](temporary[1469], temporary[1468])}
        temporary[1464](temporary[1465], unpack_values(temporary[1471]))
        temporary[1475] = Instance.new
        temporary[1478] = temporary[1475]("TextButton")
        temporary[1483] = UDim2.new
        temporary[1484] = temporary[1483](0, 24, 0, 24)
        temporary[1478].Size = temporary[1484]
        temporary[1489] = UDim2.new
        temporary[1490] = temporary[1489](1, -54, 0, 3)
        temporary[1478].Position = temporary[1490]
        temporary[1495] = Color3.fromRGB
        temporary[1496] = temporary[1495](255, 255, 255)
        temporary[1478].BackgroundColor3 = temporary[1496]
        temporary[1478].BackgroundTransparency = 0.9
        temporary[1478].Text = "-"
        temporary[1507] = Color3.fromRGB
        temporary[1508] = temporary[1507](210, 210, 215)
        temporary[1478].TextColor3 = temporary[1508]
        temporary[1513] = Enum.Font
        temporary[1516] = temporary[1513].GothamBold
        temporary[1478].Font = temporary[1516]
        temporary[1478].TextSize = 16
        temporary[1478].ZIndex = 4
        temporary[1478].Active = true
        temporary[1478].AutoButtonColor = false
        temporary[1478].Parent = temporary[1375]
        temporary[1531] = Instance.new
        temporary[1534] = temporary[1531]("UICorner")
        temporary[1539] = UDim.new
        temporary[1540] = temporary[1539](1, 0)
        temporary[1534].CornerRadius = temporary[1540]
        temporary[1534].Parent = temporary[1478]
        temporary[1545] = table.insert
        temporary[1546] = Q.value
        temporary[1549] = temporary[1478].Activated
        temporary[1550] = bind(callbacks.callback_191, {temporary[845]})
        temporary[1551] = temporary[1549].Connect
        temporary[1552] = {temporary[1551](temporary[1549], temporary[1550])}
        temporary[1545](temporary[1546], unpack_values(temporary[1552]))
        temporary[1556] = Instance.new
        temporary[1559] = temporary[1556]("Frame")
        temporary[1559].Name = "Sidebar"
        temporary[1568] = UDim2.new
        temporary[1569] = temporary[1568](0, 115, 1, -45)
        temporary[1559].Size = temporary[1569]
        temporary[1574] = UDim2.new
        temporary[1575] = temporary[1574](0, 0, 0, 45)
        temporary[1559].Position = temporary[1575]
        temporary[1580] = Color3.fromRGB
        temporary[1581] = temporary[1580](15, 15, 18)
        temporary[1559].BackgroundColor3 = temporary[1581]
        temporary[1559].BackgroundTransparency = 0.45
        temporary[1559].BorderSizePixel = 0
        temporary[1559].ZIndex = 2
        temporary[1590] = temporary[722].value
        temporary[1559].Parent = temporary[1590]
        temporary[1593] = Instance.new
        temporary[1596] = temporary[1593]("ScrollingFrame")
        temporary[1596].Name = "TabScrollContainer"
        temporary[1605] = UDim2.new
        temporary[1606] = temporary[1605](1, 0, 1, -55)
        temporary[1596].Size = temporary[1606]
        temporary[1611] = UDim2.new
        temporary[1612] = temporary[1611](0, 0, 0, 0)
        temporary[1596].Position = temporary[1612]
        temporary[1596].BackgroundTransparency = 1
        temporary[1596].BorderSizePixel = 0
        temporary[1596].ScrollBarThickness = 2
        temporary[1623] = Color3.fromRGB
        temporary[1624] = temporary[1623](255, 255, 255)
        temporary[1596].ScrollBarImageColor3 = temporary[1624]
        temporary[1629] = Enum.ScrollingDirection
        temporary[1632] = temporary[1629].Y
        temporary[1596].ScrollingDirection = temporary[1632]
        temporary[1596].Parent = temporary[1559]
        temporary[1637] = Instance.new
        temporary[1640] = temporary[1637]("ScrollingFrame")
        temporary[1641] = {}
        temporary[1641].value = temporary[1640]
        temporary[1642] = temporary[1641].value
        temporary[1642].Name = "TabScrollContainer"
        temporary[1647] = temporary[1641].value
        temporary[1652] = UDim2.new
        temporary[1653] = temporary[1652](1, 0, 1, -55)
        temporary[1647].Size = temporary[1653]
        temporary[1654] = temporary[1641].value
        temporary[1659] = UDim2.new
        temporary[1660] = temporary[1659](0, 0, 0, 0)
        temporary[1654].Position = temporary[1660]
        temporary[1661] = temporary[1641].value
        temporary[1661].BackgroundTransparency = 1
        temporary[1664] = temporary[1641].value
        temporary[1664].BorderSizePixel = 0
        temporary[1667] = temporary[1641].value
        temporary[1667].ScrollBarThickness = 2
        temporary[1670] = temporary[1641].value
        temporary[1675] = Enum.AutomaticSize
        temporary[1678] = temporary[1675].Y
        temporary[1670].AutomaticCanvasSize = temporary[1678]
        temporary[1679] = temporary[1641].value
        temporary[1684] = UDim2.new
        temporary[1685] = temporary[1684](0, 0, 0, 0)
        temporary[1679].CanvasSize = temporary[1685]
        temporary[1686] = temporary[1641].value
        temporary[1686].Parent = temporary[1559]
        temporary[1691] = Instance.new
        temporary[1694] = temporary[1691]("UIListLayout")
        temporary[1699] = Enum.SortOrder
        temporary[1702] = temporary[1699].LayoutOrder
        temporary[1694].SortOrder = temporary[1702]
        temporary[1707] = UDim.new
        temporary[1708] = temporary[1707](0, 4)
        temporary[1694].Padding = temporary[1708]
        temporary[1713] = Enum.HorizontalAlignment
        temporary[1716] = temporary[1713].Center
        temporary[1694].HorizontalAlignment = temporary[1716]
        temporary[1719] = temporary[1641].value
        temporary[1694].Parent = temporary[1719]
        temporary[1722] = workspace.CurrentCamera
        branch_result = temporary[1722]
        Ah, B7, Bh, Ch, Dh, E7, F, Fh, G, Gh, H7, I7, Jh, Kh, L7, Mh, O, Oh, P, Ph, Qh, R, Rh, S, Sh, Th, U7, Uh, Vh, Wh, X7, Xh, Yh, ah, b, c7, dh, eh, fh, gh, h7, hh, i7, jh, k7, l7, m, mh, nh, o7, p7, ph, qh, rh, scratch_1, scratch_11, scratch_12, scratch_13, scratch_15, scratch_16, scratch_17, scratch_18, scratch_2, scratch_20, scratch_25, scratch_26, scratch_27, scratch_3, scratch_35, scratch_37, scratch_4, scratch_43, scratch_45, scratch_47, scratch_5, scratch_7, scratch_9, sh, th, u7, uh, v7, w, wh, x, yh, zh = temporary[359], temporary[449], temporary[308], temporary[280], temporary[357], temporary[440], temporary[274], temporary[388], temporary[7], temporary[393], temporary[428], temporary[442], temporary[343], temporary[354], temporary[446], temporary[360], temporary[276], temporary[398], temporary[270], temporary[395], temporary[392], temporary[262], temporary[397], temporary[88], temporary[389], temporary[286], temporary[443], temporary[303], temporary[390], temporary[380], temporary[445], temporary[304], temporary[297], temporary[350], temporary[271], temporary[437], temporary[407], temporary[279], temporary[307], temporary[347], temporary[431], temporary[278], temporary[402], temporary[345], temporary[434], temporary[465], temporary[266], temporary[406], temporary[383], temporary[458], temporary[468], temporary[293], temporary[348], temporary[295], temporary[459], temporary[570], temporary[572], temporary[722], temporary[678], temporary[676], temporary[811], temporary[845], temporary[466], temporary[838], temporary[897], temporary[935], temporary[1245], temporary[463], temporary[1299], temporary[1641], temporary[470], temporary[1559], temporary[1722], temporary[1722], temporary[312], temporary[508], temporary[615], temporary[263], temporary[310], temporary[467], temporary[268], temporary[441], temporary[260], temporary[396], temporary[272], temporary[382], temporary[346]
    end
    if branch_result then
        scratch_47 = (scratch_45.ViewportSize.Y < 450)
    end
    branch_result = scratch_47
    if branch_result then
        w.value.UIScale = math.clamp((scratch_45.ViewportSize.Y / 480), 0.55, 0.85)
        scratch_17.value.Scale = w.value.UIScale
    end
    do
        local temporary = {}
        temporary[6] = Instance.new("Frame")
        temporary[6].Size = UDim2.new(0, 1, 1, 0)
        temporary[6].Position = UDim2.new(1, -1, 0, 0)
        temporary[6].BackgroundColor3 = Color3.fromRGB(40, 40, 48)
        temporary[6].BorderSizePixel = 0
        temporary[6].ZIndex = 3
        temporary[6].Parent = scratch_43
        temporary[36] = Instance.new("Frame")
        temporary[36].Name = "UserProfileFrame"
        temporary[36].Size = UDim2.new(1, 0, 0, 50)
        temporary[36].Position = UDim2.new(0, 0, 1, -55)
        temporary[36].BackgroundTransparency = 1
        temporary[36].ZIndex = 4
        temporary[36].Parent = scratch_43
        temporary[64] = Instance.new("UIStroke")
        temporary[64].Thickness = 1
        temporary[64].Color = Color3.fromRGB(80, 80, 90)
        temporary[64].Transparency = 0.55
        temporary[64].Parent = temporary[36]
        temporary[82] = Instance.new("UICorner")
        temporary[82].CornerRadius = UDim.new(0, 6)
        temporary[82].Parent = temporary[36]
        temporary[96] = Instance.new("ImageLabel")
        temporary[97] = {}
        temporary[97].value = temporary[96]
        temporary[97].value.Name = "AvatarImage"
        temporary[97].value.Size = UDim2.new(0, 34, 0, 34)
        temporary[97].value.Position = UDim2.new(0, 10, 0.5, -17)
        temporary[97].value.BackgroundColor3 = Color3.fromRGB(30, 30, 35)
        temporary[97].value.BackgroundTransparency = 0.2
        temporary[127] = temporary[97].value
        temporary[127].ZIndex = 5
        temporary[130] = temporary[97].value
        temporary[130].Parent = temporary[36]
        temporary[135] = Instance.new
        temporary[138] = temporary[135]("UICorner")
        temporary[143] = UDim.new
        temporary[144] = temporary[143](1, 0)
        temporary[138].CornerRadius = temporary[144]
        temporary[147] = temporary[97].value
        temporary[138].Parent = temporary[147]
        temporary[150] = Instance.new
        temporary[153] = temporary[150]("TextLabel")
        temporary[154] = {}
        temporary[154].value = temporary[153]
        temporary[155] = temporary[154].value
        temporary[155].Name = "UserLabel"
        temporary[160] = temporary[154].value
        temporary[165] = UDim2.new
        temporary[166] = temporary[165](1, -52, 1, 0)
        temporary[160].Size = temporary[166]
        temporary[167] = temporary[154].value
        temporary[172] = UDim2.new
        temporary[173] = temporary[172](0, 48, 0, 0)
        temporary[167].Position = temporary[173]
        temporary[174] = temporary[154].value
        temporary[174].BackgroundTransparency = 1
        temporary[177] = temporary[154].value
        temporary[177].Text = "Cargando..."
        temporary[182] = temporary[154].value
        temporary[187] = Color3.fromRGB
        temporary[188] = temporary[187](240, 240, 245)
        temporary[182].TextColor3 = temporary[188]
        temporary[189] = temporary[154].value
        temporary[194] = Enum.Font
        temporary[197] = temporary[194].GothamBold
        temporary[189].Font = temporary[197]
        temporary[198] = temporary[154].value
        temporary[198].TextSize = 10
        temporary[201] = temporary[154].value
        temporary[206] = Enum.TextXAlignment
        temporary[209] = temporary[206].Left
        temporary[201].TextXAlignment = temporary[209]
        temporary[210] = temporary[154].value
        temporary[210].ClipsDescendants = true
        temporary[214] = temporary[154].value
        temporary[214].ZIndex = 5
        temporary[217] = temporary[154].value
        temporary[217].Parent = temporary[36]
        temporary[222] = task.spawn
        temporary[223] = bind(callbacks.callback_90, {J, captures[1], captures[2], temporary[154], X, temporary[97]})
        temporary[222](temporary[223])
        temporary[227] = Instance.new
        temporary[230] = temporary[227]("Frame")
        temporary[231] = {}
        temporary[231].value = temporary[230]
        temporary[232] = temporary[231].value
        temporary[232].Name = "PageContainer"
        temporary[237] = temporary[231].value
        temporary[242] = UDim2.new
        temporary[243] = temporary[242](1, -130, 1, -60)
        temporary[237].Size = temporary[243]
        temporary[244] = temporary[231].value
        temporary[249] = UDim2.new
        temporary[250] = temporary[249](0, 125, 0, 50)
        temporary[244].Position = temporary[250]
        temporary[251] = temporary[231].value
        temporary[251].BackgroundTransparency = 1
        temporary[254] = temporary[231].value
        temporary[254].ZIndex = 2
        temporary[257] = temporary[231].value
        temporary[257].ClipsDescendants = true
        temporary[261] = temporary[231].value
        temporary[261].Active = true
        temporary[265] = temporary[231].value
        temporary[268] = scratch_13.value
        temporary[265].Parent = temporary[268]
        temporary[271] = Instance.new
        temporary[274] = temporary[271]("ImageLabel")
        temporary[274].Name = "OptionsBackgroundImage"
        temporary[283] = UDim2.new
        temporary[284] = temporary[283](1, 0, 1, 0)
        temporary[274].Size = temporary[284]
        temporary[289] = UDim2.new
        temporary[290] = temporary[289](0, 0, 0, 0)
        temporary[274].Position = temporary[290]
        temporary[274].BackgroundTransparency = 1
        temporary[274].Image = Uh
        temporary[299] = Enum.ScaleType
        temporary[302] = temporary[299].Crop
        temporary[274].ScaleType = temporary[302]
        temporary[274].ImageTransparency = 0
        temporary[274].ZIndex = 1
        temporary[309] = temporary[231].value
        temporary[274].Parent = temporary[309]
        temporary[312] = Instance.new
        temporary[315] = temporary[312]("UICorner")
        temporary[320] = UDim.new
        temporary[321] = temporary[320](0, 8)
        temporary[315].CornerRadius = temporary[321]
        temporary[324] = {}
        temporary[325] = {}
        temporary[315].Parent = temporary[274]
        temporary[326] = {}
        temporary[327] = {}
        temporary[328] = bind(callbacks.callback_91, {captures[1], captures[2], temporary[231], Q, temporary[325], temporary[327]})
        temporary[327].value = temporary[326]
        temporary[329] = {}
        temporary[324].value = temporary[329]
        temporary[330] = {}
        temporary[325].value = temporary[330]
        temporary[333] = temporary[328]("ESP")
        temporary[336] = temporary[328]("Aimbot")
        temporary[339] = temporary[328]("Hitbox")
        temporary[342] = temporary[328]("KillAura")
        temporary[345] = temporary[328]("AutoFarm")
        temporary[348] = temporary[328]("Settings")
        temporary[349] = {}
        temporary[350] = {}
        temporary[349].value = temporary[350]
        u7(temporary[333], "WallCheck")
        temporary[354] = temporary[349].value
        temporary[357] = l7.value
        temporary[360] = temporary[357](temporary[333], "Esp Chams")
        temporary[354].S_EspToggle = temporary[360]
        temporary[361] = temporary[349].value
        temporary[364] = temporary[361].S_EspToggle
        temporary[367] = w.value
        temporary[370] = temporary[367].ChamsEnabled
        temporary[371] = bind(callbacks.callback_92, {w, captures[1], captures[2], zh})
        o7(temporary[364], "ChamsEnabled", temporary[370], temporary[371])
        p7(temporary[333], "Color Chams", "ChamsColor")
        u7(temporary[333], "Box y Lineas")
        temporary[381] = temporary[349].value
        temporary[384] = l7.value
        temporary[387] = temporary[384](temporary[333], "Esp Box")
        temporary[381].S_EspBox = temporary[387]
        temporary[388] = temporary[349].value
        temporary[391] = temporary[388].S_EspBox
        temporary[394] = w.value
        temporary[397] = temporary[394].EspBoxEnabled
        temporary[398] = bind(callbacks.callback_93, {w, captures[1], captures[2], zh})
        o7(temporary[391], "EspBoxEnabled", temporary[397], temporary[398])
        p7(temporary[333], " Color Box", "EspBoxColor")
        temporary[405] = temporary[349].value
        temporary[408] = l7.value
        temporary[411] = temporary[408](temporary[333], "Esp Lineas")
        temporary[405].S_EspLine = temporary[411]
        temporary[412] = temporary[349].value
        temporary[415] = temporary[412].S_EspLine
        temporary[418] = w.value
        temporary[421] = temporary[418].EspLineEnabled
        temporary[422] = bind(callbacks.callback_94, {w, captures[1], captures[2], zh})
        o7(temporary[415], "EspLineEnabled", temporary[421], temporary[422])
        p7(temporary[333], " Color Lineas", "EspLineColor")
        temporary[429] = temporary[349].value
        temporary[432] = l7.value
        temporary[435] = w.value
        temporary[438] = temporary[435].EspLinePosition
        branch_result = temporary[438]
        scratch_47, scratch_52, scratch_54, scratch_58, scratch_59, scratch_60, scratch_63, scratch_64, scratch_65, scratch_66, scratch_67, scratch_68, scratch_69, scratch_70, scratch_72, scratch_76 = temporary[97], temporary[154], temporary[231], temporary[327], temporary[324], temporary[325], temporary[333], temporary[336], temporary[339], temporary[342], temporary[345], temporary[348], temporary[429], temporary[349], temporary[432], temporary[438]
    end
    if (not branch_result) then
        scratch_76 = "Abajo"
    end
    do
        local temporary = {}
        scratch_69.S_EspLinePos = scratch_72(scratch_63, ("Posici贸n L铆neas: " .. scratch_76))
        temporary[8] = Instance.new("TextButton")
        temporary[8].Size = UDim2.new(1, 0, 1, 0)
        temporary[8].BackgroundTransparency = 1
        temporary[8].Text = ""
        temporary[8].ZIndex = 6
        temporary[8].Active = true
        temporary[8].AutoButtonColor = false
        temporary[8].Parent = scratch_70.value.S_EspLinePos
        temporary[37] = table.insert
        temporary[38] = Q.value
        temporary[41] = bind(callbacks.callback_113, {w, captures[1], captures[2], scratch_70, ph})
        temporary[42] = temporary[8].Activated
        temporary[37](temporary[38], unpack_values({temporary[42].Connect(temporary[42], temporary[41])}))
        u7(scratch_63, "Adicional")
        scratch_70.value.S_EspHealth = l7.value(scratch_63, "Esp Vida")
        o7(scratch_70.value.S_EspHealth, "EspHealthEnabled", w.value.EspHealthEnabled, bind(callbacks.callback_114, {w, captures[1], captures[2], zh}))
        scratch_70.value.S_EspName = l7.value(scratch_63, "Esp Nombres")
        o7(scratch_70.value.S_EspName, "EspNameEnabled", w.value.EspNameEnabled, bind(callbacks.callback_115, {w, captures[1], captures[2], zh}))
        scratch_70.value.S_EspDist = l7.value(scratch_63, "Esp Distancia")
        temporary[97] = scratch_70.value.S_EspDist
        temporary[103] = w.value.EspDistanceEnabled
        temporary[104] = bind(callbacks.callback_116, {w, captures[1], captures[2], zh})
        o7(temporary[97], "EspDistanceEnabled", temporary[103], temporary[104])
        u7(scratch_64, "Aimbot & AutoShoot")
        temporary[109] = scratch_70.value
        temporary[112] = l7.value
        temporary[117] = temporary[112](scratch_64, "Autoshoot", "Con Macro")
        temporary[109].S_AutoShoot = temporary[117]
        temporary[118] = scratch_70.value
        temporary[121] = l7.value
        temporary[124] = temporary[121](scratch_64, "Aimbot C谩mara")
        temporary[118].S_Aimbot = temporary[124]
        temporary[125] = scratch_70.value
        temporary[128] = l7.value
        temporary[131] = temporary[128](scratch_64, "Posici贸n Aimbot: Head")
        temporary[125].S_AimbotPart = temporary[131]
        temporary[132] = scratch_70.value
        temporary[135] = l7.value
        temporary[138] = temporary[135](scratch_64, "Wall Check")
        temporary[132].S_WallCheck = temporary[138]
        temporary[139] = scratch_70.value
        temporary[142] = l7.value
        temporary[145] = temporary[142](scratch_64, "Team Check")
        temporary[139].S_TeamCheck = temporary[145]
        u7(scratch_64, "Fov")
        temporary[149] = scratch_70.value
        temporary[152] = l7.value
        temporary[155] = temporary[152](scratch_64, "Mostrar C铆rculo FOV")
        temporary[149].S_ShowFOV = temporary[155]
        temporary[156] = scratch_70.value
        temporary[159] = l7.value
        temporary[164] = temporary[159](scratch_64, "FOV", "M贸vil")
        temporary[156].S_FOVType = temporary[164]
        temporary[165] = scratch_70.value
        temporary[168] = l7.value
        temporary[171] = temporary[168](scratch_64, "Color del FOV")
        temporary[165].S_FOVColor = temporary[171]
        temporary[172] = scratch_70.value
        temporary[175] = l7.value
        temporary[178] = temporary[175](scratch_64, "Tama帽o del FOV")
        temporary[172].S_FOVSize = temporary[178]
        temporary[179] = scratch_70.value
        temporary[182] = l7.value
        temporary[185] = temporary[182](scratch_64, "Grosor del FOV")
        temporary[179].S_FOVThick = temporary[185]
        u7(scratch_64, "Atajos PC")
        temporary[189] = scratch_70.value
        temporary[192] = l7.value
        temporary[197] = temporary[192](scratch_64, "Tecla Para Activar Aimbot", "PC")
        temporary[189].S_AimbotBind = temporary[197]
        temporary[198] = scratch_70.value
        temporary[201] = temporary[198].S_AutoShoot
        temporary[204] = w.value
        temporary[207] = temporary[204].AutoShootEnabled
        temporary[208] = bind(callbacks.callback_117, {w, captures[1], captures[2], zh})
        o7(temporary[201], "AutoShootEnabled", temporary[207], temporary[208])
        temporary[210] = scratch_70.value
        temporary[213] = temporary[210].S_Aimbot
        temporary[216] = w.value
        temporary[219] = temporary[216].AimbotEnabled
        temporary[220] = bind(callbacks.callback_118, {w, captures[1], captures[2], zh})
        o7(temporary[213], "AimbotEnabled", temporary[219], temporary[220])
        temporary[224] = Instance.new
        temporary[227] = temporary[224]("TextButton")
        temporary[232] = UDim2.new
        temporary[233] = temporary[232](1, 0, 1, 0)
        temporary[227].Size = temporary[233]
        temporary[227].BackgroundTransparency = 1
        temporary[227].Text = ""
        temporary[227].ZIndex = 6
        temporary[227].Active = true
        temporary[227].AutoButtonColor = false
        temporary[250] = scratch_70.value
        temporary[253] = temporary[250].S_AimbotPart
        temporary[227].Parent = temporary[253]
        temporary[254] = {}
        temporary[255] = bind(callbacks.callback_119, {scratch_70, captures[1], captures[2], w})
        temporary[254].value = temporary[255]
        temporary[258] = table.insert
        temporary[259] = Q.value
        temporary[262] = temporary[227].Activated
        temporary[263] = bind(callbacks.callback_120, {w, captures[1], captures[2], temporary[254], zh, ph})
        temporary[264] = temporary[262].Connect
        temporary[265] = {temporary[264](temporary[262], temporary[263])}
        temporary[258](temporary[259], unpack_values(temporary[265]))
        temporary[267] = temporary[254].value
        temporary[267]()
        temporary[269] = scratch_70.value
        temporary[272] = temporary[269].S_WallCheck
        temporary[275] = w.value
        temporary[278] = temporary[275].AimbotWallCheck
        temporary[279] = bind(callbacks.callback_121, {w, captures[1], captures[2], zh})
        o7(temporary[272], "AimbotWallCheck", temporary[278], temporary[279])
        temporary[281] = scratch_70.value
        temporary[284] = temporary[281].S_TeamCheck
        temporary[287] = w.value
        temporary[290] = temporary[287].AimbotTeamCheck
        temporary[291] = bind(callbacks.callback_122, {w, captures[1], captures[2], zh})
        o7(temporary[284], "AimbotTeamCheck", temporary[290], temporary[291])
        u7(scratch_65, "Objetivo")
        temporary[296] = scratch_70.value
        temporary[299] = l7.value
        temporary[302] = temporary[299](scratch_65, "Hitbox")
        temporary[296].S_Hitbox = temporary[302]
        temporary[303] = scratch_70.value
        temporary[306] = l7.value
        temporary[309] = temporary[306](scratch_65, "Hitbox Visible")
        temporary[303].S_HitboxVisible = temporary[309]
        temporary[310] = scratch_70.value
        temporary[313] = l7.value
        temporary[316] = temporary[313](scratch_65, "Tama帽o de Hitbox")
        temporary[310].S_HitboxSize = temporary[316]
        u7(scratch_65, "Atajos PC (Hitbox)")
        temporary[320] = scratch_70.value
        temporary[323] = l7.value
        temporary[328] = temporary[323](scratch_65, "Tecla Para Activar Hitbox", "PC")
        temporary[320].S_HitboxBind = temporary[328]
        temporary[329] = scratch_70.value
        temporary[332] = l7.value
        temporary[337] = temporary[332](scratch_65, "Tecla Para Hitbox Visible", "PC")
        temporary[329].S_HitboxVisibleBind = temporary[337]
        temporary[338] = scratch_70.value
        temporary[341] = temporary[338].S_Hitbox
        temporary[344] = w.value
        temporary[347] = temporary[344].HitboxEnabled
        temporary[348] = bind(callbacks.callback_123, {w, captures[1], captures[2], zh, hh})
        o7(temporary[341], "HitboxEnabled", temporary[347], temporary[348])
        temporary[350] = scratch_70.value
        temporary[353] = temporary[350].S_HitboxBind
        scratch_3(temporary[353], "ToggleHitbox")
        temporary[357] = scratch_70.value
        temporary[360] = temporary[357].S_HitboxVisibleBind
        scratch_3(temporary[360], "ToggleHitboxVisible")
        temporary[364] = scratch_70.value
        temporary[367] = temporary[364].S_HitboxSize
        temporary[370] = w.value
        temporary[373] = temporary[370].HitboxSize
        scratch_1(temporary[367], "HitboxSize", 2, 50, temporary[373])
        temporary[375] = scratch_70.value
        temporary[378] = temporary[375].S_HitboxVisible
        temporary[381] = w.value
        temporary[384] = temporary[381].HitboxVisible
        temporary[385] = bind(callbacks.callback_124, {w, captures[1], captures[2], zh, ph})
        o7(temporary[378], "HitboxVisible", temporary[384], temporary[385])
        temporary[389] = table.insert
        temporary[390] = Q.value
        temporary[391] = u.value
        temporary[394] = temporary[391].InputBegan
        temporary[395] = bind(callbacks.callback_125, {captures[1], captures[2], w, O, zh, ph})
        temporary[396] = temporary[394].Connect
        temporary[397] = {temporary[396](temporary[394], temporary[395])}
        temporary[389](temporary[390], unpack_values(temporary[397]))
        u7(scratch_66, "Agresivo")
        temporary[402] = scratch_70.value
        temporary[405] = l7.value
        temporary[408] = temporary[405](scratch_66, "Kill Aura")
        temporary[402].S_KillAuraToggle = temporary[408]
        temporary[409] = scratch_70.value
        temporary[412] = l7.value
        temporary[415] = temporary[412](scratch_66, "Auto Equipar Cuchillo")
        temporary[409].S_AutoEquipKnife = temporary[415]
        temporary[416] = scratch_70.value
        temporary[419] = temporary[416].S_AutoEquipKnife
        temporary[422] = w.value
        temporary[425] = temporary[422].AutoEquipKnifeEnabled
        temporary[426] = bind(callbacks.callback_126, {w, captures[1], captures[2], zh})
        o7(temporary[419], "AutoEquipKnifeEnabled", temporary[425], temporary[426])
        temporary[428] = scratch_70.value
        temporary[431] = l7.value
        temporary[434] = w.value
        temporary[437] = temporary[434].SelectedTargetName
        branch_result = temporary[437]
        scratch_69, scratch_73, scratch_75, scratch_79 = temporary[254], temporary[428], temporary[431], temporary[437]
    end
    if (not branch_result) then
        scratch_79 = "Ninguno"
    end
    do
        local temporary = {}
        scratch_73.S_TargetSelect = scratch_75(scratch_66, ("Matar Objetivo Espec铆fico: " .. scratch_79))
        scratch_70.value.S_KillAuraFloat = l7.value(scratch_66, "Bot贸n Flotante Kill Aura", "M贸vil")
        scratch_70.value.S_KillAuraBind = l7.value(scratch_66, "Tecla Para Activar Kill Aura", "PC")
        temporary[26] = Instance.new("TextButton")
        temporary[26].Size = UDim2.new(1, 0, 1, 0)
        temporary[26].BackgroundTransparency = 1
        temporary[26].Text = ""
        temporary[26].ZIndex = 6
        temporary[26].Active = true
        temporary[26].AutoButtonColor = false
        temporary[26].Parent = scratch_70.value.S_TargetSelect
        temporary[55] = table.insert
        temporary[56] = Q.value
        temporary[59] = temporary[26].Activated
        temporary[55](temporary[56], unpack_values({temporary[59].Connect(temporary[59], bind(callbacks.callback_44, {I7, captures[1], captures[2], w, scratch_70, zh, ph}))}))
        u7(scratch_66, "Ayuda Kill Aura")
        scratch_70.value.S_Invisible = l7.value(scratch_66, "Invisible")
        scratch_70.value.S_InvisibleFloat = l7.value(scratch_66, "Bot贸n Flotante Invisible", "M贸vil")
        scratch_70.value.S_InvisibleBind = l7.value(scratch_66, "Tecla Para Activar Invisible (PC)")
        o7(scratch_70.value.S_Invisible, "InvisibleEnabled", w.value.InvisibleEnabled, bind(callbacks.callback_45, {w, captures[1], captures[2], fh, zh}))
        temporary[102] = scratch_70.value
        temporary[105] = temporary[102].S_InvisibleBind
        scratch_3(temporary[105], "ToggleInvisible")
        temporary[109] = scratch_70.value
        temporary[112] = temporary[109].S_InvisibleFloat
        temporary[115] = w.value
        temporary[118] = temporary[115].InvisibleFloatEnabled
        temporary[119] = bind(callbacks.callback_46, {w, captures[1], captures[2], scratch_7, ph})
        o7(temporary[112], "InvisibleFloatEnabled", temporary[118], temporary[119])
        u7(scratch_66, "Rendimiento")
        temporary[124] = scratch_70.value
        temporary[127] = l7.value
        temporary[132] = temporary[127](scratch_66, "Optimizar FPS", "Mejora el rendimiento Si Vas Lag")
        temporary[124].S_AntiLagSection = temporary[132]
        temporary[133] = scratch_70.value
        temporary[136] = temporary[133].S_AntiLagSection
        temporary[139] = w.value
        temporary[142] = temporary[139].AntiLagEnabled
        temporary[143] = bind(callbacks.callback_47, {w, captures[1], captures[2], Ah, ph, O, Kh})
        o7(temporary[136], "AntiLagEnabled", temporary[142], temporary[143])
        temporary[145] = scratch_70.value
        temporary[148] = temporary[145].S_AutoClickerToggle
        temporary[151] = w.value
        temporary[154] = temporary[151].AutoClickerEnabled
        temporary[155] = bind(callbacks.callback_48, {w, captures[1], captures[2], zh, ph})
        o7(temporary[148], "AutoClickerEnabled", temporary[154], temporary[155])
        temporary[157] = scratch_70.value
        temporary[160] = temporary[157].S_KillAuraToggle
        temporary[163] = w.value
        temporary[166] = temporary[163].KillAuraEnabled
        temporary[167] = bind(callbacks.callback_49, {w, captures[1], captures[2], zh, X})
        o7(temporary[160], "KillAuraEnabled", temporary[166], temporary[167])
        temporary[169] = scratch_70.value
        temporary[172] = temporary[169].S_KillAuraBind
        scratch_3(temporary[172], "ToggleKillAura")
        temporary[176] = scratch_70.value
        temporary[179] = temporary[176].S_KillAuraFloat
        temporary[182] = w.value
        temporary[185] = temporary[182].KillAuraFloatEnabled
        temporary[186] = bind(callbacks.callback_50, {w, captures[1], captures[2], scratch_9, ph})
        o7(temporary[179], "KillAuraFloatEnabled", temporary[185], temporary[186])
        temporary[188] = scratch_70.value
        temporary[191] = l7.value
        temporary[194] = temporary[191](scratch_67, "Autofarm Evento")
        temporary[188].S_AutoFarmToggle = temporary[194]
        temporary[195] = scratch_70.value
        temporary[198] = temporary[195].S_AutoFarmToggle
        temporary[201] = w.value
        temporary[204] = temporary[201].AutoFarmEnabled
        temporary[205] = bind(callbacks.callback_51, {w, captures[1], captures[2], zh, ph})
        o7(temporary[198], "AutoFarmEnabled", temporary[204], temporary[205])
        temporary[207] = scratch_70.value
        temporary[210] = temporary[207].S_ShowFOV
        temporary[213] = w.value
        temporary[216] = temporary[213].ShowFOV
        temporary[217] = bind(callbacks.callback_52, {w, captures[1], captures[2]})
        o7(temporary[210], "ShowFOV", temporary[216], temporary[217])
        temporary[219] = scratch_70.value
        temporary[222] = temporary[219].S_FOVType
        temporary[225] = w.value
        temporary[228] = temporary[225].FOVIsMobile
        temporary[229] = bind(callbacks.callback_53, {w, captures[1], captures[2], zh})
        o7(temporary[222], "FOVIsMobile", temporary[228], temporary[229])
        temporary[231] = scratch_70.value
        temporary[234] = temporary[231].S_FOVColor
        temporary[235] = scratch_2(temporary[234])
        temporary[236] = {}
        temporary[236].value = temporary[235]
        temporary[239] = Instance.new
        temporary[242] = temporary[239]("TextButton")
        temporary[247] = UDim2.new
        temporary[248] = temporary[247](1, 0, 1, 0)
        temporary[242].Size = temporary[248]
        temporary[242].BackgroundTransparency = 1
        temporary[242].Text = ""
        temporary[242].ZIndex = 6
        temporary[242].Active = true
        temporary[242].AutoButtonColor = false
        temporary[265] = scratch_70.value
        temporary[268] = temporary[265].S_FOVColor
        temporary[242].Parent = temporary[268]
        temporary[271] = table.insert
        temporary[272] = Q.value
        temporary[275] = bind(callbacks.callback_54, {w, captures[1], captures[2], S, temporary[236], zh, ph})
        temporary[276] = temporary[242].Activated
        temporary[277] = temporary[276].Connect
        temporary[278] = {temporary[277](temporary[276], temporary[275])}
        temporary[271](temporary[272], unpack_values(temporary[278]))
        temporary[280] = temporary[236].value
        temporary[283] = w.value
        temporary[286] = temporary[283].FOVColor
        temporary[280].BackgroundColor3 = temporary[286]
        temporary[287] = scratch_70.value
        temporary[290] = temporary[287].S_FOVSize
        temporary[293] = w.value
        temporary[296] = temporary[293].FOVRadius
        scratch_1(temporary[290], "FOVRadius", 10, 1000, temporary[296])
        temporary[298] = scratch_70.value
        temporary[301] = temporary[298].S_FOVThick
        temporary[304] = w.value
        temporary[307] = temporary[304].FOVThickness
        scratch_1(temporary[301], "FOVThickness", 1, 20, temporary[307])
        temporary[309] = scratch_70.value
        temporary[312] = temporary[309].S_AimbotBind
        scratch_3(temporary[312], "ToggleAimbot")
        temporary[318] = Instance.new
        temporary[321] = temporary[318]("Frame")
        temporary[322] = {}
        temporary[322].value = temporary[321]
        temporary[323] = temporary[322].value
        temporary[323].Name = "AimbotFOVCircle"
        temporary[328] = temporary[322].value
        temporary[328].BackgroundTransparency = 1
        temporary[331] = temporary[322].value
        temporary[331].ZIndex = 50
        temporary[334] = temporary[322].value
        temporary[337] = w.value
        temporary[340] = temporary[337].ShowFOV
        temporary[334].Visible = temporary[340]
        temporary[341] = temporary[322].value
        temporary[346] = Vector2.new
        temporary[347] = temporary[346](0.5, 0.5)
        temporary[341].AnchorPoint = temporary[347]
        temporary[350] = Instance.new
        temporary[353] = temporary[350]("UICorner")
        temporary[358] = UDim.new
        temporary[359] = temporary[358](1, 0)
        temporary[353].CornerRadius = temporary[359]
        temporary[362] = temporary[322].value
        temporary[353].Parent = temporary[362]
        temporary[365] = Instance.new
        temporary[368] = temporary[365]("UIStroke")
        temporary[369] = {}
        temporary[369].value = temporary[368]
        temporary[370] = temporary[369].value
        temporary[373] = w.value
        temporary[376] = temporary[373].FOVThickness
        temporary[370].Thickness = temporary[376]
        temporary[377] = temporary[369].value
        temporary[380] = w.value
        temporary[383] = temporary[380].FOVColor
        temporary[377].Color = temporary[383]
        temporary[384] = temporary[369].value
        temporary[387] = temporary[322].value
        temporary[384].Parent = temporary[387]
        temporary[388] = temporary[322].value
        temporary[391] = b.value
        temporary[388].Parent = temporary[391]
        temporary[394] = workspace.CurrentCamera
        temporary[395] = {}
        temporary[395].value = temporary[394]
        temporary[398] = game.GetService
        temporary[399] = temporary[398](game, "GuiService")
        temporary[400] = bind(callbacks.callback_55, {w, captures[1], captures[2]})
        temporary[401] = {}
        temporary[401].value = temporary[399]
        temporary[402] = {}
        temporary[403] = bind(callbacks.callback_56, {w, captures[1], captures[2], X, J, temporary[402], Jh, temporary[395], temporary[322]})
        temporary[402].value = temporary[400]
        temporary[404] = {}
        temporary[404].value = temporary[403]
        temporary[407] = table.insert
        temporary[408] = Q.value
        temporary[409] = B.value
        temporary[412] = temporary[409].RenderStepped
        temporary[413] = temporary[412].Connect
        temporary[414] = bind(callbacks.callback_57, {w, captures[1], captures[2], temporary[322], J, hh, X, Jh, temporary[369], temporary[395], temporary[401], u, temporary[404], temporary[402]})
        temporary[415] = {temporary[413](temporary[412], temporary[414])}
        temporary[407](temporary[408], unpack_values(temporary[415]))
        temporary[417] = l7.value
        temporary[420] = temporary[417](scratch_68, "Tecla Menu UI")
        temporary[421] = l7.value
        temporary[424] = temporary[421](scratch_68, "Rejoin")
        temporary[425] = l7.value
        temporary[430] = temporary[425](scratch_68, "Tama帽o del Panel", "Ajusta El Tama帽o Recomendado En Movil")
        temporary[431] = l7.value
        temporary[434] = temporary[431](scratch_68, "Color del Panel")
        temporary[435] = l7.value
        temporary[438] = temporary[435](scratch_68, "Restaurar Teclas y Configuraciones")
        temporary[439] = l7.value
        temporary[442] = temporary[439](scratch_68, "Mostrar Notificaciones")
        temporary[443] = l7.value
        temporary[446] = temporary[443](scratch_68, "Mostrar Bot贸n Flotante")
        temporary[449] = bind(callbacks.callback_58, {w, captures[1], captures[2], scratch_17, ph})
        o7(temporary[430], "Restablecer Tama帽o (100%)", false, temporary[449])
        scratch_3(temporary[420], "ToggleUI")
        temporary[457] = w.value
        temporary[460] = temporary[457].NotificationsEnabled
        temporary[461] = bind(callbacks.callback_59, {w, captures[1], captures[2]})
        o7(temporary[442], "NotificationsEnabled", temporary[460], temporary[461])
        temporary[465] = Instance.new
        temporary[468] = temporary[465]("ImageButton")
        temporary[469] = {}
        temporary[469].value = temporary[468]
        temporary[470] = temporary[469].value
        temporary[470].Name = "KaiserFloatingButton"
        temporary[475] = temporary[469].value
        temporary[480] = UDim2.new
        temporary[481] = temporary[480](0, 60, 0, 60)
        temporary[475].Size = temporary[481]
        temporary[482] = temporary[469].value
        temporary[487] = UDim2.new
        temporary[488] = temporary[487](0.02, 0, 0.2, 0)
        temporary[482].Position = temporary[488]
        temporary[489] = temporary[469].value
        temporary[489].BackgroundTransparency = 1
        temporary[492] = temporary[469].value
        temporary[492].Image = Xh
        temporary[495] = temporary[469].value
        temporary[500] = Enum.ScaleType
        temporary[503] = temporary[500].Crop
        temporary[495].ScaleType = temporary[503]
        temporary[504] = temporary[469].value
        temporary[504].Active = true
        temporary[508] = temporary[469].value
        temporary[508].AutoButtonColor = false
        temporary[512] = temporary[469].value
        temporary[515] = w.value
        temporary[518] = temporary[515].FloatingButtonEnabled
        temporary[512].Visible = temporary[518]
        temporary[519] = temporary[469].value
        temporary[522] = b.value
        temporary[519].Parent = temporary[522]
        temporary[525] = Instance.new
        temporary[528] = temporary[525]("UICorner")
        temporary[533] = UDim.new
        temporary[534] = temporary[533](1, 0)
        temporary[528].CornerRadius = temporary[534]
        temporary[537] = temporary[469].value
        temporary[528].Parent = temporary[537]
        temporary[538] = temporary[469].value
        Bh(temporary[538])
        temporary[542] = table.insert
        temporary[543] = Q.value
        temporary[544] = temporary[469].value
        temporary[547] = temporary[544].Activated
        temporary[548] = bind(callbacks.callback_60, {scratch_18, scratch_13, captures[1], captures[2]})
        temporary[549] = temporary[547].Connect
        temporary[550] = {temporary[549](temporary[547], temporary[548])}
        temporary[542](temporary[543], unpack_values(temporary[550]))
        temporary[554] = w.value
        temporary[557] = temporary[554].FloatingButtonEnabled
        temporary[558] = bind(callbacks.callback_61, {w, captures[1], captures[2], temporary[469]})
        o7(temporary[446], "FloatingButtonEnabled", temporary[557], temporary[558])
        temporary[562] = Instance.new
        temporary[565] = temporary[562]("TextLabel")
        temporary[566] = {}
        temporary[566].value = temporary[565]
        temporary[567] = temporary[566].value
        temporary[572] = UDim2.new
        temporary[573] = temporary[572](0, 50, 1, 0)
        temporary[567].Size = temporary[573]
        temporary[574] = temporary[566].value
        temporary[579] = UDim2.new
        temporary[580] = temporary[579](1, -62, 0, 0)
        temporary[574].Position = temporary[580]
        temporary[581] = temporary[566].value
        temporary[581].BackgroundTransparency = 1
        temporary[584] = temporary[566].value
        temporary[589] = string.format
        temporary[592] = w.value
        temporary[595] = temporary[592].UIScale
        temporary[596] = temporary[589]("%.1fx", temporary[595])
        temporary[584].Text = temporary[596]
        temporary[597] = temporary[566].value
        temporary[602] = Color3.fromRGB
        temporary[603] = temporary[602](255, 200, 0)
        temporary[597].TextColor3 = temporary[603]
        temporary[604] = temporary[566].value
        temporary[609] = Enum.Font
        temporary[612] = temporary[609].GothamBold
        temporary[604].Font = temporary[612]
        temporary[613] = temporary[566].value
        temporary[613].TextSize = 13
        temporary[616] = temporary[566].value
        temporary[621] = Enum.TextXAlignment
        temporary[624] = temporary[621].Right
        temporary[616].TextXAlignment = temporary[624]
        temporary[625] = temporary[566].value
        temporary[625].ZIndex = 4
        temporary[628] = temporary[566].value
        temporary[628].Active = false
        temporary[632] = temporary[566].value
        temporary[632].Parent = temporary[430]
        temporary[637] = Instance.new
        temporary[640] = temporary[637]("TextButton")
        temporary[640].Name = "ResizeGrip"
        temporary[649] = UDim2.new
        temporary[650] = temporary[649](0, 20, 0, 20)
        temporary[640].Size = temporary[650]
        temporary[655] = UDim2.new
        temporary[656] = temporary[655](1, -20, 1, -20)
        temporary[640].Position = temporary[656]
        temporary[640].BackgroundTransparency = 1
        temporary[640].Text = "鈼�"
        temporary[667] = Color3.fromRGB
        temporary[668] = temporary[667](255, 255, 255)
        temporary[640].TextColor3 = temporary[668]
        temporary[640].TextTransparency = 0.65
        temporary[675] = Enum.Font
        temporary[678] = temporary[675].GothamBold
        temporary[640].Font = temporary[678]
        temporary[640].TextSize = 14
        temporary[640].ZIndex = 8
        temporary[640].Active = true
        temporary[640].AutoButtonColor = false
        temporary[691] = scratch_13.value
        temporary[640].Parent = temporary[691]
        temporary[694] = Instance.new
        temporary[697] = temporary[694]("Frame")
        temporary[698] = {}
        temporary[698].value = temporary[697]
        temporary[699] = temporary[698].value
        temporary[699].Name = "ResetContainer"
        temporary[704] = temporary[698].value
        temporary[709] = UDim2.new
        temporary[710] = temporary[709](0, 170, 0, 42)
        temporary[704].Size = temporary[710]
        temporary[711] = temporary[698].value
        temporary[716] = UDim2.new
        temporary[717] = temporary[716](1, -180, 1, -55)
        temporary[711].Position = temporary[717]
        temporary[718] = temporary[698].value
        temporary[723] = Color3.fromRGB
        temporary[724] = temporary[723](30, 30, 35)
        temporary[718].BackgroundColor3 = temporary[724]
        temporary[725] = temporary[698].value
        temporary[728] = w.value
        temporary[731] = temporary[728].UIScale
        temporary[732] = (temporary[731] <= 0.6)
        temporary[725].Visible = temporary[732]
        temporary[733] = temporary[698].value
        temporary[733].ZIndex = 10
        temporary[736] = temporary[698].value
        temporary[739] = b.value
        temporary[736].Parent = temporary[739]
        temporary[742] = Instance.new
        temporary[745] = temporary[742]("UICorner")
        temporary[750] = UDim.new
        temporary[751] = temporary[750](0, 8)
        temporary[745].CornerRadius = temporary[751]
        temporary[754] = temporary[698].value
        temporary[745].Parent = temporary[754]
        temporary[757] = Instance.new
        temporary[760] = temporary[757]("UIStroke")
        temporary[760].Thickness = 1.5
        temporary[767] = Color3.fromRGB
        temporary[768] = temporary[767](60, 60, 68)
        temporary[760].Color = temporary[768]
        temporary[771] = temporary[698].value
        temporary[760].Parent = temporary[771]
        temporary[774] = Instance.new
        temporary[777] = temporary[774]("TextLabel")
        temporary[782] = UDim2.new
        temporary[783] = temporary[782](0, 100, 1, 0)
        temporary[777].Size = temporary[783]
        temporary[788] = UDim2.new
        temporary[789] = temporary[788](0, 12, 0, 0)
        temporary[777].Position = temporary[789]
        temporary[777].BackgroundTransparency = 1
        temporary[777].Text = "Reiniciar Tama帽o"
        temporary[800] = Color3.fromRGB
        temporary[801] = temporary[800](255, 255, 255)
        temporary[777].TextColor3 = temporary[801]
        temporary[806] = Enum.Font
        temporary[809] = temporary[806].GothamMedium
        temporary[777].Font = temporary[809]
        temporary[777].TextSize = 13
        temporary[816] = Enum.TextXAlignment
        temporary[819] = temporary[816].Left
        temporary[777].TextXAlignment = temporary[819]
        temporary[777].ZIndex = 11
        temporary[824] = temporary[698].value
        temporary[777].Parent = temporary[824]
        temporary[827] = Instance.new
        temporary[830] = temporary[827]("TextButton")
        temporary[831] = {}
        temporary[831].value = temporary[830]
        temporary[832] = temporary[831].value
        temporary[837] = UDim2.new
        temporary[838] = temporary[837](0, 42, 0, 24)
        temporary[832].Size = temporary[838]
        temporary[839] = temporary[831].value
        temporary[844] = UDim2.new
        temporary[845] = temporary[844](1, -52, 0.5, -12)
        temporary[839].Position = temporary[845]
        temporary[846] = temporary[831].value
        temporary[851] = Color3.fromRGB
        temporary[852] = temporary[851](50, 50, 55)
        temporary[846].BackgroundColor3 = temporary[852]
        temporary[853] = temporary[831].value
        temporary[853].Text = ""
        temporary[858] = temporary[831].value
        temporary[858].AutoButtonColor = false
        temporary[862] = temporary[831].value
        temporary[862].ZIndex = 11
        temporary[865] = temporary[831].value
        temporary[868] = temporary[698].value
        temporary[865].Parent = temporary[868]
        temporary[871] = Instance.new
        temporary[874] = temporary[871]("UICorner")
        temporary[879] = UDim.new
        temporary[880] = temporary[879](1, 0)
        temporary[874].CornerRadius = temporary[880]
        temporary[883] = temporary[831].value
        temporary[874].Parent = temporary[883]
        temporary[886] = Instance.new
        temporary[889] = temporary[886]("Frame")
        temporary[890] = {}
        temporary[890].value = temporary[889]
        temporary[891] = temporary[890].value
        temporary[896] = UDim2.new
        temporary[897] = temporary[896](0, 18, 0, 18)
        temporary[891].Size = temporary[897]
        temporary[898] = temporary[890].value
        temporary[903] = UDim2.new
        temporary[904] = temporary[903](0, 3, 0.5, -9)
        temporary[898].Position = temporary[904]
        temporary[905] = temporary[890].value
        temporary[910] = Color3.fromRGB
        temporary[911] = temporary[910](255, 255, 255)
        temporary[905].BackgroundColor3 = temporary[911]
        temporary[912] = temporary[890].value
        temporary[912].ZIndex = 12
        temporary[915] = temporary[890].value
        temporary[918] = temporary[831].value
        temporary[915].Parent = temporary[918]
        temporary[921] = Instance.new
        temporary[924] = temporary[921]("UICorner")
        temporary[929] = UDim.new
        temporary[930] = temporary[929](1, 0)
        temporary[924].CornerRadius = temporary[930]
        temporary[933] = temporary[890].value
        temporary[924].Parent = temporary[933]
        temporary[936] = Instance.new
        temporary[939] = temporary[936]("UIStroke")
        temporary[939].Thickness = 1
        temporary[946] = Color3.fromRGB
        temporary[947] = temporary[946](0, 0, 0)
        temporary[939].Color = temporary[947]
        temporary[939].Transparency = 0.8
        temporary[952] = temporary[890].value
        temporary[939].Parent = temporary[952]
        temporary[954] = {}
        temporary[954].value = false
        temporary[957] = table.insert
        temporary[958] = Q.value
        temporary[959] = temporary[831].value
        temporary[962] = temporary[959].Activated
        temporary[963] = bind(callbacks.callback_62, {temporary[954], o, temporary[890], captures[1], captures[2], temporary[831], w, scratch_17, scratch_13, P, temporary[566], temporary[698], ph, zh})
        temporary[964] = temporary[962].Connect
        temporary[965] = {temporary[964](temporary[962], temporary[963])}
        temporary[957](temporary[958], unpack_values(temporary[965]))
        temporary[968] = {}
        temporary[969] = {}
        temporary[969].value = false
        temporary[970] = bind(callbacks.callback_63, {u, captures[1], captures[2], scratch_13, P, w, scratch_17, temporary[566]})
        temporary[968].value = nil
        temporary[971] = {}
        temporary[971].value = temporary[970]
        temporary[974] = table.insert
        temporary[975] = Q.value
        temporary[978] = temporary[640].InputBegan
        temporary[979] = temporary[978].Connect
        temporary[980] = bind(callbacks.callback_64, {captures[1], captures[2], temporary[969], temporary[968], B, temporary[971]})
        temporary[981] = {temporary[979](temporary[978], temporary[980])}
        temporary[974](temporary[975], unpack_values(temporary[981]))
        temporary[985] = table.insert
        temporary[986] = Q.value
        temporary[987] = u.value
        temporary[990] = temporary[987].InputEnded
        temporary[991] = temporary[990].Connect
        temporary[992] = bind(callbacks.callback_65, {captures[1], captures[2], temporary[969], temporary[968], ph})
        temporary[993] = {temporary[991](temporary[990], temporary[992])}
        temporary[985](temporary[986], unpack_values(temporary[993]))
        temporary[997] = Instance.new
        temporary[1000] = temporary[997]("TextButton")
        temporary[1005] = UDim2.new
        temporary[1006] = temporary[1005](1, 0, 1, 0)
        temporary[1000].Size = temporary[1006]
        temporary[1000].BackgroundTransparency = 1
        temporary[1000].Text = ""
        temporary[1000].ZIndex = 6
        temporary[1000].Active = true
        temporary[1000].AutoButtonColor = false
        temporary[1000].Parent = temporary[438]
        temporary[1025] = table.insert
        temporary[1026] = Q.value
        temporary[1029] = temporary[1000].Activated
        temporary[1030] = bind(callbacks.callback_66, {w, captures[1], captures[2], scratch_17, scratch_13, P, temporary[566], F, scratch_69, S, hh, J, O, fh, scratch_7, scratch_9, temporary[469], temporary[236], ph, zh})
        temporary[1031] = temporary[1029].Connect
        temporary[1032] = {temporary[1031](temporary[1029], temporary[1030])}
        temporary[1025](temporary[1026], unpack_values(temporary[1032]))
        temporary[1036] = Instance.new
        temporary[1039] = temporary[1036]("Frame")
        temporary[1040] = {}
        temporary[1040].value = temporary[1039]
        temporary[1041] = temporary[1040].value
        temporary[1046] = UDim2.new
        temporary[1047] = temporary[1046](0, 180, 0, 115)
        temporary[1041].Size = temporary[1047]
        temporary[1048] = temporary[1040].value
        temporary[1053] = UDim2.new
        temporary[1054] = temporary[1053](0.5, -90, 0.5, -57)
        temporary[1048].Position = temporary[1054]
        temporary[1055] = temporary[1040].value
        temporary[1060] = Color3.fromRGB
        temporary[1061] = temporary[1060](20, 20, 25)
        temporary[1055].BackgroundColor3 = temporary[1061]
        temporary[1062] = temporary[1040].value
        temporary[1062].Visible = false
        temporary[1066] = temporary[1040].value
        temporary[1066].ZIndex = 10
        temporary[1069] = temporary[1040].value
        temporary[1069].Active = false
        temporary[1073] = temporary[1040].value
        temporary[1076] = scratch_13.value
        temporary[1073].Parent = temporary[1076]
        temporary[1079] = Instance.new
        temporary[1082] = temporary[1079]("UICorner")
        temporary[1087] = UDim.new
        temporary[1088] = temporary[1087](0, 10)
        temporary[1082].CornerRadius = temporary[1088]
        temporary[1091] = temporary[1040].value
        temporary[1082].Parent = temporary[1091]
        temporary[1094] = Instance.new
        temporary[1097] = temporary[1094]("UIStroke")
        temporary[1097].Thickness = 1.5
        temporary[1104] = Color3.fromRGB
        temporary[1105] = temporary[1104](45, 45, 52)
        temporary[1097].Color = temporary[1105]
        temporary[1108] = temporary[1040].value
        temporary[1097].Parent = temporary[1108]
        temporary[1111] = Instance.new
        temporary[1114] = temporary[1111]("Frame")
        temporary[1119] = UDim2.new
        temporary[1120] = temporary[1119](1, -20, 0, 55)
        temporary[1114].Size = temporary[1120]
        temporary[1125] = UDim2.new
        temporary[1126] = temporary[1125](0, 10, 0, 12)
        temporary[1114].Position = temporary[1126]
        temporary[1114].BackgroundTransparency = 1
        temporary[1114].ZIndex = 11
        temporary[1114].Active = false
        temporary[1136] = temporary[1040].value
        temporary[1114].Parent = temporary[1136]
        temporary[1139] = Instance.new
        temporary[1142] = temporary[1139]("UIGridLayout")
        temporary[1147] = UDim2.new
        temporary[1148] = temporary[1147](0, 26, 0, 24)
        temporary[1142].CellSize = temporary[1148]
        temporary[1153] = UDim2.new
        temporary[1154] = temporary[1153](0, 7, 0, 7)
        temporary[1142].CellPadding = temporary[1154]
        temporary[1142].Parent = temporary[1114]
        temporary[1159] = Color3.fromRGB
        temporary[1160] = temporary[1159](255, 0, 0)
        temporary[1163] = Color3.fromRGB
        temporary[1164] = temporary[1163](160, 100, 255)
        temporary[1167] = Color3.fromRGB
        temporary[1168] = temporary[1167](60, 150, 255)
        temporary[1171] = Color3.fromRGB
        temporary[1172] = temporary[1171](0, 240, 180)
        temporary[1175] = Color3.fromRGB
        temporary[1176] = temporary[1175](100, 255, 100)
        temporary[1179] = Color3.fromRGB
        temporary[1180] = temporary[1179](255, 200, 0)
        temporary[1183] = Color3.fromRGB
        temporary[1184] = temporary[1183](255, 110, 180)
        temporary[1187] = Color3.fromRGB
        temporary[1188] = temporary[1187](240, 240, 245)
        temporary[1191] = Color3.fromRGB
        temporary[1192] = temporary[1191](200, 200, 180)
        temporary[1195] = Color3.fromRGB
        temporary[1196] = {temporary[1195](156, 163, 168)}
        temporary[1197] = {temporary[1160], temporary[1164], temporary[1168], temporary[1172], temporary[1176], temporary[1180], temporary[1184], temporary[1188], temporary[1192], unpack_values(temporary[1196])}
        temporary[1200] = Instance.new
        temporary[1203] = temporary[1200]("TextButton")
        temporary[1204] = {}
        temporary[1204].value = temporary[1203]
        temporary[1205] = temporary[1204].value
        temporary[1210] = UDim2.new
        temporary[1211] = temporary[1210](0, 45, 0, 24)
        temporary[1205].Size = temporary[1211]
        temporary[1212] = temporary[1204].value
        temporary[1217] = UDim2.new
        temporary[1218] = temporary[1217](1, -57, 0.5, -12)
        temporary[1212].Position = temporary[1218]
        temporary[1219] = temporary[1204].value
        temporary[1222] = w.value
        temporary[1225] = temporary[1222].PanelColor
        temporary[1219].BackgroundColor3 = temporary[1225]
        temporary[1226] = temporary[1204].value
        temporary[1226].Text = ""
        temporary[1231] = temporary[1204].value
        temporary[1231].ZIndex = 6
        temporary[1234] = temporary[1204].value
        temporary[1234].Active = true
        temporary[1238] = temporary[1204].value
        temporary[1238].AutoButtonColor = false
        temporary[1242] = temporary[1204].value
        temporary[1242].Parent = temporary[434]
        temporary[1247] = Instance.new
        temporary[1250] = temporary[1247]("UICorner")
        temporary[1255] = UDim.new
        temporary[1256] = temporary[1255](0, 4)
        temporary[1250].CornerRadius = temporary[1256]
        temporary[1259] = temporary[1204].value
        temporary[1250].Parent = temporary[1259]
        temporary[1262] = Instance.new
        temporary[1265] = temporary[1262]("UIStroke")
        temporary[1265].Thickness = 1
        temporary[1272] = Color3.fromRGB
        temporary[1273] = temporary[1272](255, 255, 255)
        temporary[1265].Color = temporary[1273]
        temporary[1276] = temporary[1204].value
        temporary[1265].Parent = temporary[1276]
        temporary[1277] = bind(callbacks.callback_67, {w, captures[1], captures[2], temporary[1204], scratch_25, scratch_26, R, scratch_59, scratch_58})
        SetActivePanelColor = temporary[1277]
        temporary[1278] = {ipairs(temporary[1197])}
        temporary[1279] = temporary[1278][2]
        temporary[1280] = temporary[1278][1]
        temporary[1281] = temporary[1278][3]
        scratch_101, scratch_103, scratch_106, scratch_107, scratch_108, scratch_109, scratch_114, scratch_116, scratch_120, scratch_121, scratch_122, scratch_73, scratch_75, scratch_77, scratch_79, scratch_80, scratch_81, scratch_82, scratch_85, scratch_92, scratch_93, scratch_95, scratch_97 = temporary[890], temporary[971], temporary[954], temporary[969], temporary[968], temporary[1040], temporary[1114], temporary[1204], temporary[1280], temporary[1279], temporary[1281], temporary[322], temporary[236], temporary[369], temporary[401], temporary[395], temporary[402], temporary[404], temporary[424], temporary[469], temporary[566], temporary[698], temporary[831]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = scratch_120(scratch_121, scratch_122)
            branch_result = temp_1
            scratch_122, scratch_123 = temp_1, temp_2
        end
        if not branch_result then break end
        do
            local temp_1, temp_30, temp_44, temp_59, temp_60, temp_63, temp_64, temp_7
            temp_1 = {}
            temp_1.value = scratch_123
            temp_7 = Instance.new("TextButton")
            temp_7.BackgroundColor3 = temp_1.value
            temp_7.Text = ""
            temp_7.ZIndex = 12
            temp_7.Active = true
            temp_7.AutoButtonColor = false
            temp_7.Parent = scratch_114
            temp_30 = Instance.new("UICorner")
            temp_30.CornerRadius = UDim.new(0, 5)
            temp_30.Parent = temp_7
            temp_44 = Instance.new("UIStroke")
            temp_44.Thickness = 1
            temp_44.Color = Color3.fromRGB(0, 0, 0)
            temp_44.Transparency = 0.4
            temp_44.Parent = temp_7
            temp_59 = table.insert
            temp_60 = Q.value
            temp_63 = bind(callbacks.callback_111, {temp_1})
            temp_64 = temp_7.Activated
            temp_59(temp_60, unpack_values({temp_64.Connect(temp_64, temp_63)}))
        end
    end
    do
        local temp_6, temp_61, temp_72, temp_73, temp_77, temp_84, temp_85, temp_88, temp_94
        temp_6 = Instance.new("TextButton")
        temp_6.Size = UDim2.new(1, -20, 0, 24)
        temp_6.Position = UDim2.new(0, 10, 1, -34)
        temp_6.BackgroundColor3 = Color3.fromRGB(30, 30, 35)
        temp_6.Text = "Listo"
        temp_6.TextColor3 = Color3.fromRGB(240, 240, 245)
        temp_6.Font = Enum.Font.GothamMedium
        temp_6.TextSize = 12
        temp_6.ZIndex = 11
        temp_6.Active = true
        temp_6.AutoButtonColor = false
        temp_6.Parent = scratch_109.value
        temp_61 = Instance.new("UICorner")
        temp_61.CornerRadius = UDim.new(0, 5)
        temp_61.Parent = temp_6
        temp_72 = table.insert
        temp_73 = Q.value
        temp_77 = scratch_116.value.Activated
        temp_72(temp_73, unpack_values({temp_77.Connect(temp_77, bind(callbacks.callback_130, {scratch_109, captures[1], captures[2]}))}))
        temp_84 = table.insert
        temp_85 = Q.value
        temp_88 = temp_6.Activated
        temp_84(temp_85, unpack_values({temp_88.Connect(temp_88, bind(callbacks.callback_131, {scratch_109, captures[1], captures[2], ph}))}))
        temp_94 = {ipairs(R.value)}
        scratch_122, scratch_123, scratch_124 = temp_94[1], temp_94[2], temp_94[3]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = scratch_122(scratch_123, scratch_124)
            branch_result = temp_1
            scratch_124, scratch_125 = temp_1, temp_2
        end
        if not branch_result then break end
        scratch_125.Update()
    end
    do
        local temp_21, temp_32, temp_33, temp_36, temp_45, temp_46, temp_50, temp_6
        temp_6 = Instance.new("TextButton")
        temp_6.Size = UDim2.new(1, 0, 1, 0)
        temp_6.BackgroundTransparency = 1
        temp_6.Text = ""
        temp_21 = {}
        temp_6.ZIndex = 6
        temp_6.Active = true
        temp_6.AutoButtonColor = false
        temp_6.Parent = scratch_85
        temp_32 = table.insert
        temp_33 = Q.value
        temp_36 = temp_6.Activated
        temp_32(temp_33, unpack_values({temp_36.Connect(temp_36, bind(callbacks.callback_105, {zh, captures[1], captures[2], X, q, J}))}))
        bind(callbacks.callback_106, {scratch_37, captures[1], captures[2], scratch_58, scratch_59, w, Q})()
        temp_45 = table.insert
        temp_46 = Q.value
        temp_50 = u.value.InputBegan
        temp_45(temp_46, unpack_values({temp_50.Connect(temp_50, bind(callbacks.callback_107, {w, captures[1], captures[2], scratch_18, scratch_13, O, zh, ph, hh, fh}))}))
        scratch_18.value(true)
        return unpack_values(temp_21)
    end
end

-- callback_70; bloques originales: 1
callbacks.callback_70 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({pcall(readfile, arguments[1])})
end

-- next_decryption_byte; bloques originales: 5
callbacks.next_decryption_byte = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = ((# captures[1].value) == 0)
    if branch_result then
        captures[2].value = (((captures[2].value * 213) + 27552854471197) % 35184372088832)
        while true do
            captures[3].value = ((captures[3].value * 201) % 257)
            branch_result = (captures[3].value ~= 1)
            if not (not branch_result) then break end
        end
        do
            local temp_14, temp_2, temp_21, temp_22, temp_24
            temp_2 = (captures[3].value % 32)
            temp_14 = ((captures[4].value((captures[2].value / (2 ^ (13 - ((captures[3].value - temp_2) / 32))))) % 4294967296) / (2 ^ temp_2))
            temp_21 = (captures[4].value(((temp_14 % 1) * 4294967296)) + captures[4].value(temp_14))
            temp_22 = (temp_21 % 65536)
            temp_24 = ((temp_21 - temp_22) / 65536)
            captures[1].value = {(temp_22 % 256), ((temp_22 - (temp_22 % 256)) / 256), (temp_24 % 256), ((temp_24 - (temp_24 % 256)) / 256)}
        end
    end
    do
        local temp_2, temp_4
        temp_2 = (# captures[1].value)
        temp_4 = captures[1].value[temp_2]
        captures[1].value[temp_2] = nil
        return unpack_values({temp_4})
    end
end

-- decode_cached_string; bloques originales: 7
callbacks.decode_cached_string = function(captures, arguments)
    local A, B, X, a, branch_result, l, q, u, z
    local e7 = {}
    do
        local temp_1, temp_2, temp_3
        temp_1 = arguments[1]
        temp_2 = arguments[2]
        temp_3 = captures[1].value
        branch_result = temp_3[temp_2]
        B, X, l = temp_2, temp_1, temp_3
    end
    if branch_result then
        return unpack_values({B})
    end
    do
        local temp_2, temp_6
        captures[2].value = {}
        temp_2 = captures[3].value
        captures[4].value = (B % 35184372088832)
        captures[5].value = ((B % 255) + 2)
        temp_6 = (# X)
        l[B] = ""
        A, a, q, u, z = temp_6, "", 204, temp_2, 0
    end
    while true do
        do
            local temp_1
            temp_1 = (1 + z)
            branch_result = ((false and (temp_1 >= A)) or ((not false) and (A >= temp_1)))
            z = temp_1
        end
        if not branch_result then break end
        do
            local temp_7
            temp_7 = (((string.byte(X, z) + captures[6].value()) + q) % 256)
            a, q = (a .. u[(temp_7 + 1)]), temp_7
        end
    end
    l[B] = a
    return unpack_values({B})
end

-- callback_73; bloques originales: 4
callbacks.callback_73 = function(captures, arguments)
    local B, X, a, branch_result, g, o, u
    local e7 = {}
    do
        local temp_1, temp_39, temp_43, temp_44, temp_45, temp_46, temp_47, temp_7, temp_8
        temp_1 = {}
        temp_1.value = arguments[1]
        temp_7 = Instance.new("Frame")
        temp_8 = {}
        temp_8.value = temp_7
        temp_8.value.Name = "ContenedorEstrellas"
        temp_8.value.Size = UDim2.new(1, 0, 1, 0)
        temp_8.value.BackgroundTransparency = 1
        temp_8.value.ClipsDescendants = true
        temp_8.value.ZIndex = 2
        temp_8.value.Active = false
        temp_8.value.Parent = temp_1.value
        temp_39 = {}
        temp_39.value = {}
        temp_43 = {}
        temp_44 = Random.new
        temp_45 = {}
        temp_46 = temp_44()
        temp_47 = bind(callbacks.callback_198, {captures[1], captures[2], temp_8, temp_45})
        temp_45.value = temp_46
        temp_43.value = temp_47
        B, X, a, g, o, u = temp_8, temp_1, 0, temp_43, temp_45, temp_39
    end
    while true do
        do
            local temp_1, temp_2
            temp_1 = (not false)
            temp_2 = (a + 1)
            branch_result = ((false and (temp_2 >= 60)) or (temp_1 and (60 >= temp_2)))
            a = temp_2
        end
        if not branch_result then break end
        table.insert(u.value, unpack_values({g.value(false)}))
    end
    do
        local temp_1, temp_5
        temp_1 = {}
        temp_1.value = nil
        temp_5 = captures[3].value.RenderStepped
        temp_1.value = temp_5.Connect(temp_5, bind(callbacks.callback_112, {X, captures[1], captures[2], temp_1, u, g}))
        return unpack_values({})
    end
end

-- callback_74; bloques originales: 1
callbacks.callback_74 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_4, temp_5
        print("隆Ejecutando Kaiser Modern Gui!")
        temp_4 = bind(callbacks.build_modern_interface, {captures[1], captures[2]})
        temp_5 = {}
        temp_4()
        return unpack_values(temp_5)
    end
end

-- build_loading_interface; bloques originales: 33
callbacks.build_loading_interface = function(captures, arguments)
    local A, B, D, F, G, I, J, O, Q, W, X, a, b, branch_result, g, hh, ih, l, m, n, o, q, u, w, x, z
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        branch_result = temp_1.FindFirstChild(temp_1, "KaiserBypassLoader")
    end
    if branch_result then
        do
            local temp_4
            temp_4 = captures[1].value.KaiserBypassLoader
            temp_4.Destroy(temp_4)
        end
    end
    do
        local temp_10, temp_11, temp_14, temp_3, temp_6
        temp_3 = {}
        temp_3.value = "https://files.catbox.moe/54lm4f.jpg"
        temp_6 = {}
        temp_6.value = "KaiserHub_Media"
        temp_10 = (temp_6.value .. "/KaiserLoaderBg.jpg12")
        temp_11 = {}
        temp_11.value = temp_10
        temp_14 = {}
        temp_14.value = ""
        branch_result = getcustomasset
        B, I, X, l, u = temp_6, getcustomasset, temp_3, temp_11, temp_14
    end
    if (not branch_result) then
        branch_result = getsynasset
        o = getsynasset
        if (not branch_result) then
            branch_result = fileasset
            q = fileasset
            if branch_result then
                q = bind(callbacks.callback_82, {captures[2], captures[3]})
            end
            o = q
        end
        I = o
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = I
        branch_result = isfile
        I, o = isfile, temp_1
    end
    if (not branch_result) then
        branch_result = is_file
        g = is_file
        if (not branch_result) then
            branch_result = readfile
            a = readfile
            if branch_result then
                a = bind(callbacks.callback_43, {})
            end
            g = a
        end
        I = g
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = I
        branch_result = writefile
        I, g = writefile, temp_1
    end
    if (not branch_result) then
        I = write_file
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = I
        branch_result = isfolder
        I, q = isfolder, temp_1
    end
    if (not branch_result) then
        I = bind(callbacks.callback_128, {})
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = I
        branch_result = makefolder
        I, a = makefolder, temp_1
    end
    if (not branch_result) then
        I = bind(callbacks.callback_110, {})
    end
    do
        local temp_1, temp_2
        temp_1 = {}
        temp_1.value = I
        temp_2 = g.value
        branch_result = temp_2
        I, J = temp_2, temp_1
    end
    if branch_result then
        do
            local temp_1
            temp_1 = q.value
            branch_result = temp_1
            A = temp_1
        end
        if branch_result then
            A = o.value
        end
        I = A
    end
    branch_result = I
    if branch_result then
        pcall(bind(callbacks.callback_202, {a, B, J, g, l, X, q, o, u}))
    end
    do
        local temp_22, temp_6, temp_60, temp_74, temp_98
        temp_6 = Instance.new("ScreenGui")
        temp_6.Name = "KaiserBypassLoader"
        temp_6.Parent = captures[1].value
        temp_6.ResetOnSpawn = false
        temp_22 = Instance.new("Frame")
        temp_22.Name = "LoaderFrame"
        temp_22.Size = UDim2.new(0, 420, 0, 205)
        temp_22.Position = UDim2.new(0.5, -210, 0.5, -102)
        temp_22.BackgroundColor3 = Color3.fromRGB(15, 15, 20)
        temp_22.BorderSizePixel = 0
        temp_22.Active = true
        temp_22.ClipsDescendants = true
        temp_22.Parent = temp_6
        temp_60 = Instance.new("UICorner")
        temp_60.CornerRadius = UDim.new(0, 12)
        temp_60.Parent = temp_22
        temp_74 = Instance.new("ImageLabel")
        temp_74.Name = "BackgroundImage"
        temp_74.Size = UDim2.new(1, 0, 1, 0)
        temp_74.Position = UDim2.new(0, 0, 0, 0)
        temp_74.BackgroundTransparency = 1
        temp_98 = (u.value ~= "")
        branch_result = temp_98
        A, D, n, z = temp_6, temp_74, temp_98, temp_22
    end
    if branch_result then
        n = u.value
    end
    branch_result = n
    I = n
    if (not branch_result) then
        I = X.value
    end
    do
        local temporary = {}
        D.Image = I
        D.ScaleType = Enum.ScaleType.Crop
        D.ImageTransparency = 0.5
        D.ZIndex = 1
        D.Parent = z
        temporary[20] = Instance.new("UICorner")
        temporary[20].CornerRadius = UDim.new(0, 12)
        temporary[20].Parent = D
        captures[4].value(z)
        temporary[34] = Color3.fromRGB(255, 255, 255)
        temporary[38] = Color3.fromRGB(0, 0, 0)
        temporary[44] = Instance.new("UIStroke")
        temporary[44].Thickness = 3.5
        temporary[44].ApplyStrokeMode = Enum.ApplyStrokeMode.Border
        temporary[44].LineJoinMode = Enum.LineJoinMode.Round
        temporary[44].Color = temporary[34]
        temporary[44].Parent = z
        temporary[72] = Instance.new("UIGradient")
        temporary[72].Color = ColorSequence.new({ColorSequenceKeypoint.new(0, temporary[34]), ColorSequenceKeypoint.new(0.3, temporary[38]), ColorSequenceKeypoint.new(0.7, unpack_values({Color3.fromRGB(20, 20, 25)})), unpack_values({ColorSequenceKeypoint.new(1, temporary[34])})})
        temporary[72].Parent = temporary[44]
        temporary[102] = captures[5].value
        temporary[105] = TweenInfo.new
        temporary[108] = temporary[102].Create
        temporary[112] = Enum.EasingStyle.Linear
        temporary[119] = temporary[105](3, temporary[112], Enum.EasingDirection.InOut, -1)
        temporary[122] = {["Rotation"] = 360}
        temporary[123] = temporary[108](temporary[102], temporary[72], temporary[119], temporary[122])
        temporary[124] = temporary[123].Play
        temporary[124](temporary[123])
        temporary[128] = Instance.new
        temporary[131] = temporary[128]("TextLabel")
        temporary[136] = UDim2.new
        temporary[137] = temporary[136](1, -20, 0, 35)
        temporary[131].Size = temporary[137]
        temporary[142] = UDim2.new
        temporary[143] = temporary[142](0, 10, 0, 40)
        temporary[131].Position = temporary[143]
        temporary[131].BackgroundTransparency = 1
        temporary[131].Text = "Activando Bypass KaiserHub"
        temporary[154] = Color3.fromRGB
        temporary[155] = temporary[154](255, 255, 255)
        temporary[131].TextColor3 = temporary[155]
        temporary[131].TextSize = 25
        temporary[162] = Enum.Font
        temporary[165] = temporary[162].BuilderSansBold
        temporary[131].Font = temporary[165]
        temporary[131].TextWrapped = true
        temporary[173] = Enum.TextXAlignment
        temporary[176] = temporary[173].Center
        temporary[131].TextXAlignment = temporary[176]
        temporary[131].ZIndex = 3
        temporary[131].Parent = z
        temporary[183] = Instance.new
        temporary[186] = temporary[183]("TextLabel")
        temporary[187] = {}
        temporary[187].value = temporary[186]
        temporary[188] = temporary[187].value
        temporary[193] = UDim2.new
        temporary[194] = temporary[193](1, -20, 0, 25)
        temporary[188].Size = temporary[194]
        temporary[195] = temporary[187].value
        temporary[200] = UDim2.new
        temporary[201] = temporary[200](0, 10, 0, 85)
        temporary[195].Position = temporary[201]
        temporary[202] = temporary[187].value
        temporary[202].BackgroundTransparency = 1
        temporary[205] = temporary[187].value
        temporary[205].Text = ""
        temporary[210] = temporary[187].value
        temporary[215] = Color3.fromRGB
        temporary[216] = temporary[215](255, 255, 255)
        temporary[210].TextColor3 = temporary[216]
        temporary[217] = temporary[187].value
        temporary[217].TextSize = 16
        temporary[220] = temporary[187].value
        temporary[225] = Enum.Font
        temporary[228] = temporary[225].BuilderSansBold
        temporary[220].Font = temporary[228]
        temporary[229] = temporary[187].value
        temporary[229].TextWrapped = true
        temporary[233] = temporary[187].value
        temporary[238] = Enum.TextXAlignment
        temporary[241] = temporary[238].Center
        temporary[233].TextXAlignment = temporary[241]
        temporary[242] = temporary[187].value
        temporary[242].ZIndex = 3
        temporary[245] = temporary[187].value
        temporary[245].Parent = z
        temporary[250] = Instance.new
        temporary[253] = temporary[250]("Frame")
        temporary[258] = UDim2.new
        temporary[259] = temporary[258](0.85, 0, 0, 14)
        temporary[253].Size = temporary[259]
        temporary[264] = UDim2.new
        temporary[265] = temporary[264](0.075, 0, 0.62, 0)
        temporary[253].Position = temporary[265]
        temporary[270] = Color3.fromRGB
        temporary[271] = temporary[270](30, 30, 40)
        temporary[253].BackgroundColor3 = temporary[271]
        temporary[253].BorderSizePixel = 0
        temporary[253].ZIndex = 3
        temporary[253].Parent = z
        temporary[280] = Instance.new
        temporary[283] = temporary[280]("UICorner")
        temporary[288] = UDim.new
        temporary[289] = temporary[288](0, 12)
        temporary[283].CornerRadius = temporary[289]
        temporary[283].Parent = temporary[253]
        temporary[294] = Instance.new
        temporary[297] = temporary[294]("Frame")
        temporary[298] = {}
        temporary[298].value = temporary[297]
        temporary[299] = temporary[298].value
        temporary[304] = UDim2.new
        temporary[305] = temporary[304](0, 0, 1, 0)
        temporary[299].Size = temporary[305]
        temporary[306] = temporary[298].value
        temporary[311] = Color3.fromRGB
        temporary[312] = temporary[311](255, 255, 255)
        temporary[306].BackgroundColor3 = temporary[312]
        temporary[313] = temporary[298].value
        temporary[313].BorderSizePixel = 0
        temporary[316] = temporary[298].value
        temporary[316].ZIndex = 3
        temporary[319] = temporary[298].value
        temporary[319].Parent = temporary[253]
        temporary[324] = Instance.new
        temporary[327] = temporary[324]("UICorner")
        temporary[332] = UDim.new
        temporary[333] = temporary[332](1, 0)
        temporary[327].CornerRadius = temporary[333]
        temporary[336] = temporary[298].value
        temporary[327].Parent = temporary[336]
        temporary[339] = Instance.new
        temporary[342] = temporary[339]("TextLabel")
        temporary[343] = {}
        temporary[343].value = temporary[342]
        temporary[344] = temporary[343].value
        temporary[349] = UDim2.new
        temporary[350] = temporary[349](1, -20, 0, 20)
        temporary[344].Size = temporary[350]
        temporary[351] = temporary[343].value
        temporary[356] = UDim2.new
        temporary[357] = temporary[356](0, 10, 0, 162)
        temporary[351].Position = temporary[357]
        temporary[358] = temporary[343].value
        temporary[358].BackgroundTransparency = 1
        temporary[361] = temporary[343].value
        temporary[361].Text = "0%"
        temporary[366] = temporary[343].value
        temporary[371] = Color3.fromRGB
        temporary[372] = temporary[371](255, 255, 255)
        temporary[366].TextColor3 = temporary[372]
        temporary[373] = temporary[343].value
        temporary[373].TextSize = 15
        temporary[376] = temporary[343].value
        temporary[381] = Enum.Font
        temporary[384] = temporary[381].BuilderSansBold
        temporary[376].Font = temporary[384]
        temporary[385] = temporary[343].value
        temporary[390] = Enum.TextXAlignment
        temporary[393] = temporary[390].Center
        temporary[385].TextXAlignment = temporary[393]
        temporary[394] = temporary[343].value
        temporary[394].ZIndex = 3
        temporary[397] = temporary[343].value
        temporary[397].Parent = z
        temporary[402] = Instance.new
        temporary[405] = temporary[402]("TextLabel")
        temporary[410] = UDim2.new
        temporary[411] = temporary[410](0, 250, 0, 22)
        temporary[405].Size = temporary[411]
        temporary[416] = UDim2.new
        temporary[417] = temporary[416](1, -265, 1, -38)
        temporary[405].Position = temporary[417]
        temporary[405].BackgroundTransparency = 1
        temporary[405].Text = "Script By Kaiser"
        temporary[428] = Color3.fromRGB
        temporary[429] = temporary[428](255, 255, 255)
        temporary[405].TextColor3 = temporary[429]
        temporary[405].TextTransparency = 0.1
        temporary[405].TextSize = 13
        temporary[438] = Enum.Font
        temporary[441] = temporary[438].BuilderSansBold
        temporary[405].Font = temporary[441]
        temporary[446] = Enum.TextXAlignment
        temporary[449] = temporary[446].Right
        temporary[405].TextXAlignment = temporary[449]
        temporary[405].ZIndex = 3
        temporary[405].Parent = z
        temporary[454] = captures[5].value
        temporary[455] = temporary[187].value
        temporary[458] = TweenInfo.new
        temporary[461] = Enum.EasingStyle
        temporary[464] = temporary[461].Sine
        temporary[467] = Enum.EasingDirection
        temporary[470] = temporary[467].InOut
        temporary[472] = temporary[458](0.5, temporary[464], temporary[470], -1, true)
        temporary[475] = temporary[454].Create
        temporary[476] = {["TextTransparency"] = 0.5}
        temporary[477] = temporary[475](temporary[454], temporary[455], temporary[472], temporary[476])
        temporary[478] = temporary[477].Play
        temporary[478](temporary[477])
        temporary[488] = {"Bypass Esp y Hitboxes..", "Bypass Aimbot y Autoshoot...", "Bypass Kill Aura...", "Bypass Auto Farm..."}
        temporary[489] = {}
        temporary[489].value = temporary[488]
        temporary[490] = {}
        temporary[490].value = 0.4
        temporary[491] = temporary[489].value
        temporary[492] = (# temporary[491])
        temporary[493] = temporary[490].value
        temporary[494] = (temporary[492] * temporary[493])
        temporary[495] = captures[5].value
        temporary[496] = temporary[298].value
        temporary[499] = TweenInfo.new
        temporary[502] = Enum.EasingStyle
        temporary[505] = temporary[502].Linear
        temporary[508] = Enum.EasingDirection
        temporary[511] = temporary[508].Out
        temporary[512] = temporary[499](temporary[494], temporary[505], temporary[511])
        temporary[516] = temporary[495].Create
        temporary[518] = UDim2.new
        temporary[519] = temporary[518](1, 0, 1, 0)
        temporary[520] = {["Size"] = temporary[519]}
        temporary[521] = temporary[516](temporary[495], temporary[496], temporary[512], temporary[520])
        temporary[522] = temporary[521].Play
        temporary[522](temporary[521])
        temporary[524] = captures[6].value
        temporary[527] = temporary[524].RenderStepped
        temporary[528] = temporary[527].Connect
        temporary[529] = bind(callbacks.callback_196, {captures[2], captures[3], temporary[298], temporary[343]})
        temporary[530] = temporary[528](temporary[527], temporary[529])
        temporary[533] = task.spawn
        temporary[534] = bind(callbacks.callback_197, {temporary[489], temporary[187], captures[2], captures[3], temporary[490]})
        temporary[533](temporary[534])
        temporary[538] = temporary[521].Completed
        temporary[539] = temporary[538].Wait
        temporary[539](temporary[538])
        temporary[541] = temporary[343].value
        temporary[541].Text = "100%"
        branch_result = temporary[530]
        F, G, O, Q, W, b, hh, ih, m, w, x = temporary[298], temporary[131], temporary[343], temporary[44], temporary[187], temporary[489], temporary[477], temporary[530], temporary[490], temporary[253], temporary[405]
    end
    if branch_result then
        ih.Disconnect(ih)
    end
    do
        local temp_100, temp_101, temp_102, temp_104, temp_105, temp_108, temp_109, temp_110, temp_113,
            temp_114, temp_115, temp_117, temp_120, temp_121, temp_124, temp_125, temp_126, temp_127,
            temp_129, temp_133, temp_134, temp_136, temp_138, temp_28, temp_29, temp_38, temp_41, temp_45,
            temp_46, temp_51, temp_54, temp_64, temp_67, temp_7, temp_77, temp_78, temp_80, temp_83, temp_84,
            temp_87, temp_88, temp_89, temp_90, temp_92, temp_95, temp_96, temp_99
        task.wait(0.3)
        hh.Cancel(hh)
        temp_7 = captures[5].value
        temp_28 = temp_7.Create(temp_7, z, TweenInfo.new(0.4, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {["BackgroundTransparency"] = 1})
        temp_29 = captures[5].value
        temp_38 = temp_29.Create(temp_29, D, TweenInfo.new(0.15), {["ImageTransparency"] = 1})
        temp_38.Play(temp_38)
        temp_41 = captures[5].value
        temp_45 = TweenInfo.new(0.15)
        temp_46 = {}
        temp_51 = temp_41.Create(temp_41, G, temp_45, {["TextTransparency"] = 1})
        temp_51.Play(temp_51)
        temp_54 = captures[5].value
        temp_64 = temp_54.Create(temp_54, W.value, TweenInfo.new(0.15), {["TextTransparency"] = 1})
        temp_64.Play(temp_64)
        temp_67 = captures[5].value
        temp_77 = temp_67.Create(temp_67, O.value, TweenInfo.new(0.15), {["TextTransparency"] = 1})
        temp_78 = temp_77.Play
        temp_78(temp_77)
        temp_80 = captures[5].value
        temp_83 = TweenInfo.new
        temp_84 = temp_83(0.15)
        temp_87 = temp_80.Create
        temp_88 = {["TextTransparency"] = 1}
        temp_89 = temp_87(temp_80, x, temp_84, temp_88)
        temp_90 = temp_89.Play
        temp_90(temp_89)
        temp_92 = captures[5].value
        temp_95 = TweenInfo.new
        temp_96 = temp_95(0.15)
        temp_99 = {["BackgroundTransparency"] = 1}
        temp_100 = temp_92.Create
        temp_101 = temp_100(temp_92, w, temp_96, temp_99)
        temp_102 = temp_101.Play
        temp_102(temp_101)
        temp_104 = captures[5].value
        temp_105 = F.value
        temp_108 = TweenInfo.new
        temp_109 = temp_108(0.15)
        temp_110 = temp_104.Create
        temp_113 = {["BackgroundTransparency"] = 1}
        temp_114 = temp_110(temp_104, temp_105, temp_109, temp_113)
        temp_115 = temp_114.Play
        temp_115(temp_114)
        temp_117 = captures[5].value
        temp_120 = TweenInfo.new
        temp_121 = temp_120(0.15)
        temp_124 = temp_117.Create
        temp_125 = {["Transparency"] = 1}
        temp_126 = temp_124(temp_117, Q, temp_121, temp_125)
        temp_127 = temp_126.Play
        temp_127(temp_126)
        temp_129 = temp_28.Play
        temp_129(temp_28)
        temp_133 = temp_28.Completed
        temp_134 = temp_133.Wait
        temp_134(temp_133)
        temp_136 = A.Destroy
        temp_136(A)
        temp_138 = captures[7].value
        temp_138()
        return unpack_values(temp_46)
    end
end

-- callback_76; bloques originales: 1
callbacks.callback_76 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_10, temp_17, temp_24, temp_3, temp_4, temp_5, temp_6
        temp_1 = {}
        temp_3 = {}
        temp_4 = {}
        temp_3.value = arguments[1]
        temp_5 = {}
        temp_1.value = false
        temp_5.value = nil
        temp_4.value = nil
        temp_6 = {}
        temp_6.value = nil
        temp_10 = temp_3.value.InputBegan
        temp_10.Connect(temp_10, bind(callbacks.callback_86, {captures[1], captures[2], temp_1, temp_4, temp_3, temp_6}))
        temp_17 = temp_3.value.InputChanged
        temp_17.Connect(temp_17, bind(callbacks.callback_87, {captures[1], captures[2], temp_5}))
        temp_24 = captures[3].value.InputChanged
        temp_24.Connect(temp_24, bind(callbacks.callback_88, {temp_5, temp_1, captures[1], captures[2], temp_4, temp_6, captures[4], temp_3}))
        return unpack_values({})
    end
end

-- callback_77; bloques originales: 1
callbacks.callback_77 = function(captures, arguments)
    local branch_result
    local e7 = {}
    makefolder(captures[1].value)
    return unpack_values({})
end

-- callback_78; bloques originales: 5
callbacks.callback_78 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.AntiLagEnabled = false
    branch_result = captures[4].value.AntiLagEnabled
    if branch_result then
        captures[4].value.AntiLagEnabled(false)
    end
    branch_result = captures[5].value
    if branch_result then
        do
            local temp_1
            temp_1 = captures[5].value
            temp_1.Disconnect(temp_1)
            captures[5].value = nil
        end
    end
    captures[6].value()
    return unpack_values({})
end

-- callback_79; bloques originales: 16
callbacks.callback_79 = function(captures, arguments)
    local A, B, I, X, a, branch_result, g, q, u
    local e7 = {}
    do
        local temp_1, temp_29, temp_38, temp_40, temp_7
        temp_1 = arguments[1]
        temp_7 = Instance.new("Frame")
        temp_7.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        temp_7.BorderSizePixel = 0
        temp_7.ZIndex = 2
        temp_7.Active = false
        temp_7.Parent = captures[3].value
        temp_29 = Instance.new("UICorner")
        temp_29.CornerRadius = UDim.new(1, 0)
        temp_29.Parent = temp_7
        temp_38 = captures[4].value
        temp_40 = temp_38.NextInteger(temp_38, 2, 4)
        temp_7.Size = UDim2.new(0, temp_40, 0, temp_40)
        branch_result = (temp_40 == 2)
        B, X, u = temp_7, temp_1, temp_40
    end
    if branch_result then
        do
            local temp_3
            temp_3 = captures[4].value
            B.BackgroundTransparency = temp_3.NextNumber(temp_3, 0.1, 0.1)
        end
    else
        branch_result = (u == 3)
        if branch_result then
            do
                local temp_3
                temp_3 = captures[4].value
                B.BackgroundTransparency = temp_3.NextNumber(temp_3, 0.1, 0.1)
            end
        else
            do
                local temp_3
                temp_3 = captures[4].value
                B.BackgroundTransparency = temp_3.NextNumber(temp_3, 0.1, 0.1)
            end
        end
    end
    do
        local temp_1
        temp_1 = (X and 1.02)
        branch_result = temp_1
        I = temp_1
    end
    if (not branch_result) then
        do
            local temp_1
            temp_1 = captures[4].value
            I = temp_1.NextNumber(temp_1, 0, 1)
        end
    end
    do
        local temp_1, temp_10, temp_3
        temp_1 = captures[4].value
        temp_3 = temp_1.NextNumber(temp_1, 0, 0.98)
        B.Position = UDim2.new(I, 0, temp_3, 0)
        temp_10 = (u == 4)
        branch_result = temp_10
        a, g, q = temp_10, I, temp_3
    end
    if branch_result then
        do
            local temp_1
            temp_1 = captures[4].value
            a = temp_1.NextNumber(temp_1, 0.08, 0.12)
        end
    end
    branch_result = a
    I = a
    if (not branch_result) then
        do
            local temp_1
            temp_1 = (u == 3)
            branch_result = temp_1
            A = temp_1
        end
        if branch_result then
            do
                local temp_1
                temp_1 = captures[4].value
                A = temp_1.NextNumber(temp_1, 0.05, 0.08)
            end
        end
        branch_result = A
        a = A
        if (not branch_result) then
            do
                local temp_1
                temp_1 = captures[4].value
                a = temp_1.NextNumber(temp_1, 0.02, 0.05)
            end
        end
        I = a
    end
    return unpack_values({{["Instancia"] = B, ["Velocidad"] = I, ["XScale"] = g, ["YScale"] = q}})
end

-- callback_80; bloques originales: 5
callbacks.callback_80 = function(captures, arguments)
    local X, branch_result, l
    local e7 = {}
    do
        local temp_1, temp_2, temp_6
        temp_1 = arguments[2]
        temp_2 = arguments[1]
        temp_6 = RaycastParams.new()
        temp_6.FilterType = Enum.RaycastFilterType.Exclude
        temp_6.FilterDescendantsInstances = captures[3].value(temp_1)
        branch_result = workspace.Raycast(workspace, captures[4].value.CFrame.Position, (temp_2.Position - captures[4].value.CFrame.Position), temp_6)
        X, l = temp_2, temp_6
    end
    if branch_result then
        return unpack_values({false})
    end
    branch_result = workspace.Raycast(workspace, captures[5].value.Position, (X.Position - captures[5].value.Position), l)
    if branch_result then
        return unpack_values({false})
    end
    return unpack_values({true})
end

-- callback_81; bloques originales: 1
callbacks.callback_81 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({false})
end

-- callback_82; bloques originales: 1
callbacks.callback_82 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({("rbxasset://" .. arguments[1])})
end

-- load_configuration; bloques originales: 101
callbacks.load_configuration = function(captures, arguments)
    local B, I, X, branch_result, l, o, q, u
    local e7 = {}
    branch_result = readfile
    I = readfile
    if branch_result then
        branch_result = isfile
        X = isfile
        if branch_result then
            X = isfile(captures[1].value)
        end
        I = X
    end
    branch_result = I
    if branch_result then
        do
            local temp_2, temp_3, temp_5
            temp_2 = readfile(captures[1].value)
            temp_3 = captures[2].value
            temp_5 = temp_3.JSONDecode(temp_3, temp_2)
            branch_result = temp_5
            B = temp_5
        end
        if branch_result then
            branch_result = B.Binds
            if branch_result then
                do
                    local temp_4
                    temp_4 = {pairs(B.Binds)}
                    l, o, u = temp_4[2], temp_4[1], temp_4[3]
                end
                while true do
                    do
                        local temp_1, temp_2
                        temp_1, temp_2 = o(l, u)
                        branch_result = temp_1
                        q, u = temp_2, temp_1
                    end
                    if not branch_result then break end
                    captures[5].value.Binds[u] = q
                end
            end
            branch_result = (B.ChamsEnabled ~= nil)
            if branch_result then
                captures[5].value.ChamsEnabled = B.ChamsEnabled
            end
            branch_result = (B.EspBoxEnabled ~= nil)
            if branch_result then
                captures[5].value.EspBoxEnabled = B.EspBoxEnabled
            end
            branch_result = (B.EspLineEnabled ~= nil)
            if branch_result then
                captures[5].value.EspLineEnabled = B.EspLineEnabled
            end
            branch_result = (B.EspLinePosition ~= nil)
            if branch_result then
                captures[5].value.EspLinePosition = B.EspLinePosition
            end
            branch_result = (B.EspHealthEnabled ~= nil)
            if branch_result then
                captures[5].value.EspHealthEnabled = B.EspHealthEnabled
            end
            branch_result = (B.EspNameEnabled ~= nil)
            if branch_result then
                captures[5].value.EspNameEnabled = B.EspNameEnabled
            end
            branch_result = (B.EspDistanceEnabled ~= nil)
            if branch_result then
                captures[5].value.EspDistanceEnabled = B.EspDistanceEnabled
            end
            branch_result = B.ChamsColor
            if branch_result then
                captures[5].value.ChamsColor = Color3.new(B.ChamsColor[1], B.ChamsColor[2], B.ChamsColor[3])
            end
            branch_result = B.EspBoxColor
            if branch_result then
                captures[5].value.EspBoxColor = Color3.new(B.EspBoxColor[1], B.EspBoxColor[2], B.EspBoxColor[3])
            end
            branch_result = B.EspLineColor
            if branch_result then
                captures[5].value.EspLineColor = Color3.new(B.EspLineColor[1], B.EspLineColor[2], B.EspLineColor[3])
            end
            branch_result = (B.NotificationsEnabled ~= nil)
            if branch_result then
                captures[5].value.NotificationsEnabled = B.NotificationsEnabled
            end
            branch_result = (B.FloatingButtonEnabled ~= nil)
            if branch_result then
                captures[5].value.FloatingButtonEnabled = B.FloatingButtonEnabled
            end
            branch_result = (B.InvisibleFloatEnabled ~= nil)
            if branch_result then
                captures[5].value.InvisibleFloatEnabled = B.InvisibleFloatEnabled
            end
            branch_result = (B.KillAuraFloatEnabled ~= nil)
            if branch_result then
                captures[5].value.KillAuraFloatEnabled = B.KillAuraFloatEnabled
            end
            branch_result = (B.AutoEquipKnifeEnabled ~= nil)
            if branch_result then
                captures[5].value.AutoEquipKnifeEnabled = B.AutoEquipKnifeEnabled
            end
            branch_result = (B.AutoFarmEnabled ~= nil)
            if branch_result then
                captures[5].value.AutoFarmEnabled = false
            end
            branch_result = (B.SpeedEnabled ~= nil)
            if branch_result then
                captures[5].value.SpeedEnabled = false
            end
            branch_result = (B.SpeedValue ~= nil)
            if branch_result then
                captures[5].value.SpeedValue = B.SpeedValue
            end
            branch_result = (B.JumpEnabled ~= nil)
            if branch_result then
                captures[5].value.JumpEnabled = B.JumpEnabled
            end
            branch_result = (B.JumpValue ~= nil)
            if branch_result then
                captures[5].value.JumpValue = B.JumpValue
            end
            branch_result = (B.NoclipEnabled ~= nil)
            if branch_result then
                captures[5].value.NoclipEnabled = B.NoclipEnabled
            end
            branch_result = (B.InvisibleEnabled ~= nil)
            if branch_result then
                captures[5].value.InvisibleEnabled = false
            end
            branch_result = (B.FlyEnabled ~= nil)
            if branch_result then
                captures[5].value.FlyEnabled = false
            end
            branch_result = (B.FlySpeed ~= nil)
            if branch_result then
                captures[5].value.FlySpeed = B.FlySpeed
            end
            branch_result = (B.AimbotEnabled ~= nil)
            if branch_result then
                captures[5].value.AimbotEnabled = B.AimbotEnabled
            end
            branch_result = (B.AutoShootEnabled ~= nil)
            if branch_result then
                captures[5].value.AutoShootEnabled = B.AutoShootEnabled
            end
            branch_result = (B.AimbotWallCheck ~= nil)
            if branch_result then
                captures[5].value.AimbotWallCheck = B.AimbotWallCheck
            end
            branch_result = (B.AimbotTeamCheck ~= nil)
            if branch_result then
                captures[5].value.AimbotTeamCheck = B.AimbotTeamCheck
            end
            branch_result = (B.AimbotPartIndex ~= nil)
            if branch_result then
                captures[5].value.AimbotPartIndex = B.AimbotPartIndex
            end
            branch_result = (B.HitboxEnabled ~= nil)
            if branch_result then
                captures[5].value.HitboxEnabled = B.HitboxEnabled
            end
            branch_result = (B.HitboxSize ~= nil)
            if branch_result then
                captures[5].value.HitboxSize = B.HitboxSize
            end
            branch_result = (B.HitboxVisible ~= nil)
            if branch_result then
                captures[5].value.HitboxVisible = B.HitboxVisible
            end
            branch_result = (B.KillAuraEnabled ~= nil)
            if branch_result then
                captures[5].value.KillAuraEnabled = false
            end
            branch_result = (B.AutoClickerEnabled ~= nil)
            if branch_result then
                captures[5].value.AutoClickerEnabled = B.AutoClickerEnabled
            end
            branch_result = (B.ShowFOV ~= nil)
            if branch_result then
                captures[5].value.ShowFOV = B.ShowFOV
            end
            branch_result = (B.FOVIsMobile ~= nil)
            if branch_result then
                captures[5].value.FOVIsMobile = B.FOVIsMobile
            end
            branch_result = (B.FOVRadius ~= nil)
            if branch_result then
                captures[5].value.FOVRadius = B.FOVRadius
            end
            branch_result = (B.FOVThickness ~= nil)
            if branch_result then
                captures[5].value.FOVThickness = B.FOVThickness
            end
            branch_result = (B.FOVColorIndex ~= nil)
            if branch_result then
                captures[5].value.FOVColorIndex = B.FOVColorIndex
                branch_result = captures[6].value[captures[5].value.FOVColorIndex]
                if branch_result then
                    captures[5].value.FOVColor = captures[6].value[captures[5].value.FOVColorIndex].Color
                end
            end
            do
                local temp_3
                temp_3 = B.UIScale
                branch_result = temp_3
                l = temp_3
            end
            if branch_result then
                l = (B.UIScale >= 0.5)
            end
            branch_result = l
            if branch_result then
                captures[5].value.UIScale = B.UIScale
            else
                captures[5].value.UIScale = 1
            end
            branch_result = B.PanelColor
            if branch_result then
                captures[5].value.PanelColor = Color3.new(B.PanelColor[1], B.PanelColor[2], B.PanelColor[3])
            end
        end
    end
    return unpack_values({})
end

-- callback_84; bloques originales: 1
callbacks.callback_84 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        return unpack_values({unpack_values({temp_1.GetUserThumbnailAsync(temp_1, captures[2].value, captures[3].value, captures[4].value)})})
    end
end

-- decode_json_response; bloques originales: 1
callbacks.decode_json_response = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        return unpack_values({unpack_values({temp_1.JSONDecode(temp_1, captures[2].value)})})
    end
end

-- callback_86; bloques originales: 5
callbacks.callback_86 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_12
        temp_1 = {}
        temp_1.value = arguments[1]
        temp_12 = (temp_1.value.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_12
        I, X = temp_12, temp_1
    end
    if (not branch_result) then
        I = (X.value.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        do
            local temp_13
            captures[3].value = true
            captures[4].value = X.value.Position
            captures[6].value = captures[5].value.Position
            temp_13 = X.value.Changed
            temp_13.Connect(temp_13, bind(callbacks.callback_16, {X, captures[1], captures[2], captures[3]}))
        end
    end
    return unpack_values({})
end

-- callback_87; bloques originales: 5
callbacks.callback_87 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_11, temp_2
        temp_2 = arguments[1]
        temp_11 = (temp_2.UserInputType == Enum.UserInputType.MouseMovement)
        branch_result = temp_11
        I, X = temp_11, temp_2
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = X
    end
    return unpack_values({})
end

-- callback_88; bloques originales: 5
callbacks.callback_88 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = arguments[1]
        temp_3 = (temp_1 == captures[1].value)
        branch_result = temp_3
        I, X = temp_3, temp_1
    end
    if branch_result then
        I = captures[2].value
    end
    branch_result = I
    if branch_result then
        do
            local temp_45, temp_46, temp_5, temp_68
            temp_5 = (X.Position - captures[5].value)
            temp_45 = UDim2.new(captures[6].value.X.Scale, (captures[6].value.X.Offset + temp_5.X), captures[6].value.Y.Scale, (captures[6].value.Y.Offset + temp_5.Y))
            temp_46 = captures[7].value
            temp_68 = temp_46.Create(temp_46, captures[8].value, TweenInfo.new(0.08, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {["Position"] = temp_45})
            temp_68.Play(temp_68)
        end
    end
    return unpack_values({})
end

-- callback_89; bloques originales: 1
callbacks.callback_89 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value(captures[2].value)
    return unpack_values({})
end

-- callback_90; bloques originales: 14
callbacks.callback_90 = function(captures, arguments)
    local I, X, branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_2, temp_3, temp_4
        temp_2 = {pcall(bind(callbacks.callback_108, {captures[1], captures[2], captures[3]}))}
        temp_3 = temp_2[2]
        temp_4 = temp_2[1]
        branch_result = temp_4
        I, X = temp_4, temp_3
    end
    if branch_result then
        branch_result = X
        l = X
        if branch_result then
            do
                local temp_3
                temp_3 = (X ~= "")
                branch_result = temp_3
                o = temp_3
            end
            if branch_result then
                o = (X ~= "N/A")
            end
            l = o
        end
        I = l
    end
    branch_result = I
    if branch_result then
        captures[4].value.Text = tostring(X)
    else
        captures[4].value.Text = ("@" .. tostring(captures[1].value.Name))
    end
    do
        local temp_11, temp_12, temp_18, temp_19, temp_21, temp_22, temp_23, temp_4, temp_5
        temp_4 = captures[1].value.UserId
        temp_5 = {}
        temp_5.value = temp_4
        temp_11 = Enum.ThumbnailType.HeadShot
        temp_12 = {}
        temp_12.value = temp_11
        temp_18 = Enum.ThumbnailSize.Size420x420
        temp_19 = {}
        temp_19.value = temp_18
        temp_21 = {pcall(bind(callbacks.callback_84, {captures[5], temp_5, temp_12, temp_19}))}
        temp_22 = temp_21[2]
        temp_23 = temp_21[1]
        branch_result = temp_23
        I, g, l, o, u = temp_23, temp_22, temp_5, temp_19, temp_12
    end
    if branch_result then
        I = g
    end
    branch_result = I
    if branch_result then
        captures[6].value.Image = g
    end
    return unpack_values({})
end

-- callback_91; bloques originales: 1
callbacks.callback_91 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_100, temp_101, temp_103, temp_104, temp_105, temp_106, temp_107, temp_7, temp_8,
            temp_80, temp_92, temp_93, temp_94, temp_98, temp_99
        temp_1 = {}
        temp_1.value = arguments[1]
        temp_7 = Instance.new("ScrollingFrame")
        temp_8 = {}
        temp_8.value = temp_7
        temp_8.value.Name = (temp_1.value .. "Page")
        temp_8.value.Size = UDim2.new(1, 0, 1, 0)
        temp_8.value.BackgroundTransparency = 1
        temp_8.value.BorderSizePixel = 0
        temp_8.value.ScrollBarThickness = 4
        temp_8.value.ScrollBarImageColor3 = Color3.fromRGB(255, 255, 255)
        temp_8.value.ScrollBarImageTransparency = 0.5
        temp_8.value.Visible = false
        temp_8.value.ZIndex = 3
        temp_8.value.Active = true
        temp_8.value.ScrollingDirection = Enum.ScrollingDirection.Y
        temp_8.value.ElasticBehavior = Enum.ElasticBehavior.Always
        temp_8.value.Parent = captures[3].value
        temp_80 = Instance.new("UIListLayout")
        temp_80.Padding = UDim.new(0, 8)
        temp_80.Parent = temp_8.value
        temp_92 = table.insert
        temp_93 = captures[4].value
        temp_94 = temp_8.value
        temp_98 = temp_94.GetPropertyChangedSignal(temp_94, "CanvasPosition")
        temp_99 = bind(callbacks.callback_109, {temp_8, captures[1], captures[2], captures[5], temp_1})
        temp_100 = temp_98.Connect
        temp_101 = {temp_100(temp_98, temp_99)}
        temp_92(temp_93, unpack_values(temp_101))
        temp_103 = captures[6].value
        temp_104 = temp_1.value
        temp_105 = temp_8.value
        temp_103[temp_104] = temp_105
        temp_106 = temp_8.value
        temp_107 = {temp_106}
        return unpack_values(temp_107)
    end
end

-- callback_92; bloques originales: 5
callbacks.callback_92 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_4, temp_5
        temp_1 = captures[1].value
        temp_4 = arguments[1]
        temp_1.ChamsEnabled = temp_4
        temp_5 = captures[4].value
        branch_result = temp_4
        g, o, u = temp_5, temp_4, temp_5
    end
    if branch_result then
        o = "Esp Chams Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Esp Chams Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_93; bloques originales: 5
callbacks.callback_93 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.EspBoxEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Esp Box Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Esp Box Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_94; bloques originales: 5
callbacks.callback_94 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.EspLineEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Esp Lineas Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Esp Linea Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_95; bloques originales: 3
callbacks.callback_95 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_4
        temp_4 = arguments[1]
        branch_result = (temp_4.UserInputType == Enum.UserInputType.Keyboard)
        X = temp_4
    end
    if branch_result then
        do
            local temp_1, temp_9
            temp_1 = captures[3].value
            temp_1.Disconnect(temp_1)
            temp_9 = X.KeyCode.Name
            captures[4].value.Binds[captures[5].value] = temp_9
            captures[6].value.Text = temp_9
            captures[6].value.TextColor3 = Color3.fromRGB(255, 200, 0)
            captures[7].value("KaiserHub", ("Nueva tecla asignada: " .. temp_9))
            captures[8].value()
            task.wait(0.1)
            captures[9].value = false
        end
    end
    return unpack_values({})
end

-- callback_96; bloques originales: 1
callbacks.callback_96 = function(captures, arguments)
    local branch_result
    local e7 = {}
    error("Tamper Detected!")
    return unpack_values({})
end

-- callback_97; bloques originales: 1
callbacks.callback_97 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_2
        temp_2 = {}
        captures[1].value = true
        return unpack_values(temp_2)
    end
end

-- callback_98; bloques originales: 1
callbacks.callback_98 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value[captures[2].value] = captures[3].value
    captures[4].value()
    captures[5].value("KaiserHub", "Color ESP actualizado")
    return unpack_values({})
end

-- callback_99; bloques originales: 4
callbacks.callback_99 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value.KillAuraEnabled
    if branch_result then
        KAStroke.Color = Color3.fromRGB(255, 0, 0)
        KAStroke.Thickness = 2.5
    else
        KAStroke.Color = Color3.fromRGB(45, 45, 50)
        KAStroke.Thickness = 1.2
    end
    return unpack_values({})
end

-- callback_100; bloques originales: 1
callbacks.callback_100 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({("cTbzbvPE86f3" / (10371504 - ("vq30" ^ 10414190)))})
end

-- verify_access_key; bloques originales: 23
callbacks.verify_access_key = function(captures, arguments)
    local A, B, I, J, branch_result, l, q, u
    local e7 = {}
    do
        local temp_11, temp_14, temp_16, temp_17, temp_18, temp_19, temp_7
        temp_7 = game.GetService(game, "Players").LocalPlayer
        temp_11 = tostring(temp_7.UserId)
        temp_14 = temp_7.Name
        temp_16 = {pcall(bind(callbacks.callback_200, {captures[1], captures[2]}))}
        temp_17 = temp_16[1]
        temp_18 = temp_16[2]
        temp_19 = (not temp_17)
        branch_result = temp_19
        B, I, l, u = temp_11, temp_19, temp_14, temp_18
    end
    if (not branch_result) then
        I = (not u)
    end
    branch_result = I
    if branch_result then
        u = B
    end
    do
        local temp_10, temp_13, temp_14, temp_21, temp_22, temp_23, temp_3, temp_6, temp_9
        temp_3 = string.format
        temp_6 = captures[3].value
        temp_9 = temp_6.UrlEncode(temp_6, captures[4].value)
        temp_10 = captures[3].value
        temp_13 = temp_3("https://kaiser-auth.onrender.com/verify?key=%s&hwid=%s&userid=%s&username=%s", temp_9, u, B, unpack_values({temp_10.UrlEncode(temp_10, l)}))
        temp_14 = {}
        temp_14.value = temp_13
        captures[5].value.PlaceholderText = "Validando key..."
        temp_21 = {pcall(bind(callbacks.callback_204, {temp_14}))}
        temp_22 = temp_21[1]
        temp_23 = {}
        temp_23.value = temp_21[2]
        branch_result = temp_22
        J, q = temp_23, temp_14
    end
    if branch_result then
        do
            local temp_2, temp_3, temp_4
            temp_2 = {pcall(bind(callbacks.decode_json_response, {captures[3], J}))}
            temp_3 = temp_2[1]
            temp_4 = temp_2[2]
            branch_result = temp_3
            A, I = temp_4, temp_3
        end
        if branch_result then
            I = A
        end
        branch_result = I
        if branch_result then
            branch_result = (A.status == "success")
            if branch_result then
                branch_result = captures[6].value
                if branch_result then
                    do
                        local temp_1
                        temp_1 = captures[6].value
                        temp_1.Disconnect(temp_1)
                    end
                end
                branch_result = captures[7].value
                if branch_result then
                    do
                        local temp_1
                        temp_1 = captures[7].value
                        temp_1.Disconnect(temp_1)
                    end
                end
                do
                    local temp_1
                    temp_1 = captures[8].value
                    temp_1.Destroy(temp_1)
                    captures[9].value()
                end
            else
                captures[5].value.PlaceholderText = ("Error: " .. tostring(A.message))
            end
        else
            captures[5].value.PlaceholderText = "Respuesta inv谩lida de Render"
        end
    else
        warn(("Error de HTTP: " .. tostring(J.value)))
        branch_result = string.find(string.lower(unpack_values({tostring(J.value)})), "timeout")
        if branch_result then
            captures[5].value.PlaceholderText = "Servidor despertando. Dale de nuevo."
        else
            captures[5].value.PlaceholderText = "Error de red (Revisa consola F9)"
        end
    end
    return unpack_values({})
end

-- callback_102; bloques originales: 10
callbacks.callback_102 = function(captures, arguments)
    local B, X, branch_result, g, l, u
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = arguments[1]
        temp_3 = {pairs(captures[1].value)}
        B, X, l, u = temp_3[2], temp_1, temp_3[3], temp_3[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = u(B, l)
            branch_result = temp_1
            g, l = temp_2, temp_1
        end
        if not branch_result then break end
        g.Visible = (l == X)
    end
    do
        local temp_2
        temp_2 = {pairs(captures[4].value)}
        B, l, u = temp_2[1], temp_2[2], temp_2[3]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = B(l, u)
            branch_result = temp_1
            g, u = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({})
        end
        branch_result = (u == X)
        if branch_result then
            g.BackgroundTransparency = 0
            g.BackgroundColor3 = captures[5].value.PanelColor
            g.TextColor3 = Color3.fromRGB(255, 255, 255)
        else
            g.BackgroundTransparency = 1
            g.TextColor3 = Color3.fromRGB(255, 255, 255)
        end
    end
end

-- callback_103; bloques originales: 1
callbacks.callback_103 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = captures[1].value
        captures[2].value = temp_1.GetNetworkPing(temp_1)
        return unpack_values({})
    end
end

-- callback_104; bloques originales: 7
callbacks.callback_104 = function(captures, arguments)
    local I, branch_result
    local e7 = {}
    branch_result = isfolder
    I = isfolder
    if branch_result then
        I = makefolder
    end
    branch_result = I
    if branch_result then
        branch_result = (not isfolder(captures[1].value))
        if branch_result then
            pcall(bind(callbacks.callback_77, {captures[1]}))
        end
    end
    return unpack_values({})
end

-- callback_105; bloques originales: 4
callbacks.callback_105 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_11
        captures[1].value("KaiserHub", "Reconectando al servidor...")
        task.wait(0.5)
        temp_11 = captures[4].value
        branch_result = ((# temp_11.GetPlayers(temp_11)) <= 1)
    end
    if branch_result then
        do
            local temp_1
            temp_1 = captures[5].value
            temp_1.Teleport(temp_1, game.PlaceId, captures[6].value)
        end
    else
        do
            local temp_1
            temp_1 = captures[5].value
            temp_1.TeleportToPlaceInstance(temp_1, game.PlaceId, game.JobId, captures[6].value)
        end
    end
    return unpack_values({})
end

-- callback_106; bloques originales: 13
callbacks.callback_106 = function(captures, arguments)
    local B, D, J, K, X, branch_result, g, l, o, q, u, z
    local e7 = {}
    do
        local temp_1, temp_4
        temp_1 = captures[1].value
        temp_4 = {ipairs(unpack_values({temp_1.GetChildren(temp_1)}))}
        B, X, l = temp_4[3], temp_4[2], temp_4[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            do
                local temp_13, temp_38, temp_63, temp_64, temp_66
                temp_13 = {"Aimbot", "Hitbox", "ESP", "KillAura", "AutoFarm", "Settings"}
                temp_38 = {["ESP"] = "馃憗锔�", ["Aimbot"] = "馃敨", ["Hitbox"] = "馃幆", ["KillAura"] = "馃懝", ["AutoFarm"] = "馃師锔�", ["Settings"] = "鈿欙笍"}
                temp_63 = {["ESP"] = "Visual", ["Aimbot"] = "Aimbot", ["Hitbox"] = "Hitbox", ["KillAura"] = "Kill Aura", ["AutoFarm"] = "Autofarm", ["Settings"] = "Config"}
                temp_64 = {}
                temp_64.value = bind(callbacks.callback_102, {captures[4], captures[2], captures[3], captures[5], captures[6]})
                temp_66 = {ipairs(temp_13)}
                B, X, g, l, o, q, u = temp_38, temp_13, temp_66[2], temp_63, temp_66[1], temp_66[3], temp_64
            end
            while true do
                do
                    local temp_1, temp_2
                    temp_1, temp_2 = o(g, q)
                    branch_result = temp_1
                    J, q = temp_2, temp_1
                end
                if (not branch_result) then
                    do
                        local temp_1, temp_6
                        temp_1 = captures[1].value
                        temp_6 = {}
                        temp_1.CanvasSize = UDim2.new(0, 0, 0, (((# X) * 39) + 15))
                        u.value("Aimbot")
                        return unpack_values(temp_6)
                    end
                end
                do
                    local temp_1, temp_10, temp_49
                    temp_1 = {}
                    temp_1.value = J
                    temp_10 = Instance.new("TextButton")
                    temp_10.Name = (temp_1.value .. "TabBtn")
                    temp_10.Size = UDim2.new(0, 101, 0, 35)
                    temp_10.Position = UDim2.new(0, 7, 0, (((q - 1) * 39) + 8))
                    temp_10.BackgroundTransparency = 1
                    temp_10.BackgroundColor3 = captures[6].value.PanelColor
                    temp_10.ZIndex = 4
                    temp_10.Active = true
                    temp_10.AutoButtonColor = false
                    temp_49 = B[temp_1.value]
                    branch_result = temp_49
                    J, K, z = temp_1, temp_49, temp_10
                end
                if (not branch_result) then
                    K = ""
                end
                do
                    local temp_2
                    temp_2 = l[J.value]
                    branch_result = temp_2
                    D = temp_2
                end
                if (not branch_result) then
                    D = J.value
                end
                do
                    local temp_42, temp_55, temp_56, temp_59, temp_60
                    z.Text = ("  " .. (K .. (" " .. D)))
                    z.TextColor3 = Color3.fromRGB(255, 255, 255)
                    z.Font = Enum.Font.GothamBold
                    z.TextSize = 14
                    z.TextXAlignment = Enum.TextXAlignment.Left
                    z.Parent = captures[1].value
                    temp_42 = Instance.new("UICorner")
                    temp_42.CornerRadius = UDim.new(0, 6)
                    temp_42.Parent = z
                    captures[5].value[J.value] = z
                    temp_55 = table.insert
                    temp_56 = captures[7].value
                    temp_59 = bind(callbacks.callback_89, {u, J})
                    temp_60 = z.Activated
                    temp_55(temp_56, unpack_values({temp_60.Connect(temp_60, temp_59)}))
                end
            end
        end
        branch_result = o.IsA(o, "TextButton")
        if branch_result then
            o.Destroy(o)
        end
    end
end

-- callback_107; bloques originales: 53
callbacks.callback_107 = function(captures, arguments)
    local I, X, a, branch_result, g, l, o, q
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = arguments[2]
        temp_2 = arguments[1]
        branch_result = temp_1
        I, X = temp_1, temp_2
    end
    if (not branch_result) then
        I = (not captures[1].value.ScriptActive)
    end
    branch_result = I
    if branch_result then
        return unpack_values({})
    end
    branch_result = (X.UserInputType == Enum.UserInputType.Keyboard)
    if branch_result then
        do
            local temp_16, temp_6
            temp_6 = X.KeyCode.Name
            temp_16 = (captures[1].value.Binds.ToggleUI ~= "")
            branch_result = temp_16
            I, l = temp_16, temp_6
        end
        if branch_result then
            I = (l == captures[1].value.Binds.ToggleUI)
        end
        branch_result = I
        if branch_result then
            captures[4].value((not captures[5].value.Visible))
        else
            do
                local temp_10
                temp_10 = (captures[1].value.Binds.ToggleAimbot ~= "")
                branch_result = temp_10
                I = temp_10
            end
            if branch_result then
                I = (l == captures[1].value.Binds.ToggleAimbot)
            end
            branch_result = I
            if branch_result then
                captures[1].value.AimbotEnabled = (not captures[1].value.AimbotEnabled)
                branch_result = captures[6].value.AimbotEnabled
                if branch_result then
                    captures[6].value.AimbotEnabled(captures[1].value.AimbotEnabled)
                end
                do
                    local temp_1, temp_7
                    temp_1 = captures[7].value
                    temp_7 = captures[1].value.AimbotEnabled
                    branch_result = temp_7
                    a, g, q = temp_1, temp_1, temp_7
                end
                if branch_result then
                    q = "Aimbot Activado"
                end
                branch_result = q
                o = q
                if (not branch_result) then
                    o = "Aimbot Desactivado"
                end
                g("KaiserHub", o)
                captures[8].value()
            else
                do
                    local temp_10
                    temp_10 = (captures[1].value.Binds.ToggleHitbox ~= "")
                    branch_result = temp_10
                    I = temp_10
                end
                if branch_result then
                    I = (l == captures[1].value.Binds.ToggleHitbox)
                end
                branch_result = I
                if branch_result then
                    captures[1].value.HitboxEnabled = (not captures[1].value.HitboxEnabled)
                    branch_result = captures[6].value.HitboxEnabled
                    if branch_result then
                        captures[6].value.HitboxEnabled(captures[1].value.HitboxEnabled)
                    end
                    branch_result = (not captures[1].value.HitboxEnabled)
                    if branch_result then
                        captures[9].value()
                    end
                    do
                        local temp_1, temp_7
                        temp_1 = captures[7].value
                        temp_7 = captures[1].value.HitboxEnabled
                        branch_result = temp_7
                        a, g, q = temp_1, temp_1, temp_7
                    end
                    if branch_result then
                        q = "Hitbox Activada"
                    end
                    branch_result = q
                    o = q
                    if (not branch_result) then
                        o = "Hitbox Desactivada"
                    end
                    g("KaiserHub", o)
                    captures[8].value()
                else
                    do
                        local temp_10
                        temp_10 = (captures[1].value.Binds.ToggleKillAura ~= "")
                        branch_result = temp_10
                        I = temp_10
                    end
                    if branch_result then
                        I = (l == captures[1].value.Binds.ToggleKillAura)
                    end
                    branch_result = I
                    if branch_result then
                        captures[1].value.KillAuraEnabled = (not captures[1].value.KillAuraEnabled)
                        branch_result = captures[6].value.KillAuraEnabled
                        if branch_result then
                            captures[6].value.KillAuraEnabled(captures[1].value.KillAuraEnabled)
                        end
                        do
                            local temp_1, temp_7
                            temp_1 = captures[7].value
                            temp_7 = captures[1].value.KillAuraEnabled
                            branch_result = temp_7
                            a, g, q = temp_1, temp_1, temp_7
                        end
                        if branch_result then
                            q = "Kill Aura Activado"
                        end
                        branch_result = q
                        o = q
                        if (not branch_result) then
                            o = "Kill Aura Desactivado"
                        end
                        g("KaiserHub", o)
                        captures[8].value()
                    else
                        do
                            local temp_10
                            temp_10 = (captures[1].value.Binds.ToggleInvisible ~= "")
                            branch_result = temp_10
                            I = temp_10
                        end
                        if branch_result then
                            I = (l == captures[1].value.Binds.ToggleInvisible)
                        end
                        branch_result = I
                        if branch_result then
                            captures[1].value.InvisibleEnabled = (not captures[1].value.InvisibleEnabled)
                            captures[10].value(captures[1].value.InvisibleEnabled)
                            branch_result = captures[6].value.InvisibleEnabled
                            if branch_result then
                                captures[6].value.InvisibleEnabled(captures[1].value.InvisibleEnabled)
                            end
                            do
                                local temp_1, temp_7
                                temp_1 = captures[7].value
                                temp_7 = captures[1].value.InvisibleEnabled
                                branch_result = temp_7
                                a, g, q = temp_1, temp_1, temp_7
                            end
                            if branch_result then
                                q = "Invisibible Activado"
                            end
                            branch_result = q
                            o = q
                            if (not branch_result) then
                                o = "Invisible Desactivado"
                            end
                            g("KaiserHub", o)
                            captures[8].value()
                        end
                    end
                end
            end
        end
    end
    return unpack_values({})
end

-- callback_108; bloques originales: 3
callbacks.callback_108 = function(captures, arguments)
    local I, branch_result
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = captures[1].value
        temp_5 = temp_1.GetAttribute(temp_1, "Pronouns")
        branch_result = temp_5
        I = temp_5
    end
    if (not branch_result) then
        do
            local temp_4
            temp_4 = game.GetService(game, "UserService")
            I = temp_4.GetUserPronounsAsync(temp_4, captures[1].value.UserId)
        end
    end
    return unpack_values({I})
end

-- callback_109; bloques originales: 3
callbacks.callback_109 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value.Visible
    if branch_result then
        captures[4].value[captures[5].value] = captures[1].value.CanvasPosition
    end
    return unpack_values({})
end

-- callback_110; bloques originales: 1
callbacks.callback_110 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({})
end

-- callback_111; bloques originales: 1
callbacks.callback_111 = function(captures, arguments)
    local branch_result
    local e7 = {}
    SetActivePanelColor(captures[1].value)
    return unpack_values({})
end

-- callback_112; bloques originales: 19
callbacks.callback_112 = function(captures, arguments)
    local B, I, J, X, branch_result, g, l, q, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_3
        temp_1 = captures[1].value
        temp_2 = arguments[1]
        temp_3 = (not temp_1)
        branch_result = temp_3
        I, X = temp_3, temp_2
    end
    if (not branch_result) then
        do
            local temp_5
            temp_5 = (not captures[1].value.Parent)
            branch_result = temp_5
            B = temp_5
        end
        if (not branch_result) then
            do
                local temp_1
                temp_1 = captures[1].value
                B = (not temp_1.IsDescendantOf(temp_1, game))
            end
        end
        I = B
    end
    branch_result = I
    if branch_result then
        do
            local temp_1
            temp_1 = captures[4].value
            temp_1.Disconnect(temp_1)
            return unpack_values({})
        end
    end
    do
        local temp_2
        temp_2 = {ipairs(captures[5].value)}
        B, l, u = temp_2[2], temp_2[3], temp_2[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = u(B, l)
            branch_result = temp_1
            g, l = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({})
        end
        do
            local temp_3
            temp_3 = g.Instancia
            g.XScale = (g.XScale - (g.Velocidad * X))
            branch_result = (g.XScale < -0.02)
            q = temp_3
        end
        if branch_result then
            branch_result = q
            if branch_result then
                q.Destroy(q)
            end
            do
                local temp_3
                temp_3 = captures[6].value(true)
                g.Instancia = temp_3.Instancia
                g.Velocidad = temp_3.Velocidad
                g.XScale = temp_3.XScale
                g.YScale = temp_3.YScale
            end
        else
            branch_result = q
            J = q
            if branch_result then
                J = q.Parent
            end
            branch_result = J
            if branch_result then
                q.Position = UDim2.new(g.XScale, 0, g.YScale, 0)
            end
        end
    end
end

-- callback_113; bloques originales: 6
callbacks.callback_113 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = (captures[1].value.EspLinePosition == "Abajo")
    if branch_result then
        captures[1].value.EspLinePosition = "Medio"
    else
        branch_result = (captures[1].value.EspLinePosition == "Medio")
        if branch_result then
            captures[1].value.EspLinePosition = "Arriba"
        else
            captures[1].value.EspLinePosition = "Abajo"
        end
    end
    captures[4].value.S_EspLinePos.Title.Text = ("Posici贸n L铆neas: " .. captures[1].value.EspLinePosition)
    captures[5].value()
    return unpack_values({})
end

-- callback_114; bloques originales: 5
callbacks.callback_114 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_5
        temp_1 = captures[1].value
        temp_2 = arguments[1]
        temp_1.EspHealthEnabled = temp_2
        temp_5 = captures[4].value
        branch_result = temp_2
        g, o, u = temp_5, temp_2, temp_5
    end
    if branch_result then
        o = "Esp Vida Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Esp Vida Desactivado"
    end
    u("Kaiser  Hub", l)
    return unpack_values({})
end

-- callback_115; bloques originales: 5
callbacks.callback_115 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_5
        temp_1 = captures[1].value
        temp_2 = arguments[1]
        temp_1.EspNameEnabled = temp_2
        temp_5 = captures[4].value
        branch_result = temp_2
        g, o, u = temp_5, temp_2, temp_5
    end
    if branch_result then
        o = "Esp Nombres Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Esp Nombres Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_116; bloques originales: 5
callbacks.callback_116 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.EspDistanceEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Esp Distancia Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Esp Distancia Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_117; bloques originales: 5
callbacks.callback_117 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_3, temp_5
        temp_1 = captures[1].value
        temp_3 = arguments[1]
        temp_1.AutoShootEnabled = temp_3
        temp_5 = captures[4].value
        branch_result = temp_3
        g, o, u = temp_5, temp_3, temp_5
    end
    if branch_result then
        o = "AutoShoot Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "AutoShoot Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_118; bloques originales: 5
callbacks.callback_118 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.AimbotEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Aimbot Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Aimbot Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_119; bloques originales: 3
callbacks.callback_119 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_4, temp_8
        temp_4 = captures[1].value.S_AimbotPart
        temp_8 = temp_4.FindFirstChildOfClass(temp_4, "TextLabel")
        branch_result = temp_8
        X = temp_8
    end
    if branch_result then
        X.Text = ("Posici贸n Aimbot: " .. ({"Head", "Torso"})[captures[4].value.AimbotPartIndex])
    end
    return unpack_values({})
end

-- callback_120; bloques originales: 3
callbacks.callback_120 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.AimbotPartIndex = (captures[1].value.AimbotPartIndex + 1)
    branch_result = (captures[1].value.AimbotPartIndex > 3)
    if branch_result then
        captures[1].value.AimbotPartIndex = 1
    end
    captures[4].value()
    captures[5].value("KaiserHub", ("Aimbot ahora apunta a: " .. ({"Head", "Cuello", "Torso"})[captures[1].value.AimbotPartIndex]))
    captures[6].value()
    return unpack_values({})
end

-- callback_121; bloques originales: 5
callbacks.callback_121 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.AimbotWallCheck = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Wallcheck Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Wallcheck Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_122; bloques originales: 5
callbacks.callback_122 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_3, temp_5
        temp_1 = captures[1].value
        temp_3 = arguments[1]
        temp_1.AimbotTeamCheck = temp_3
        temp_5 = captures[4].value
        branch_result = temp_3
        g, o, u = temp_5, temp_3, temp_5
    end
    if branch_result then
        o = "Teamcheck Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Teamcheck Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_123; bloques originales: 7
callbacks.callback_123 = function(captures, arguments)
    local X, branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_4, temp_5
        temp_1 = captures[1].value
        temp_4 = arguments[1]
        temp_1.HitboxEnabled = temp_4
        temp_5 = captures[4].value
        branch_result = temp_4
        X, g, o, u = temp_4, temp_5, temp_4, temp_5
    end
    if branch_result then
        o = "Hitbox Activada"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Hitbox Desactivada"
    end
    u("KaiserHub", l)
    branch_result = (not X)
    if branch_result then
        captures[5].value()
    end
    return unpack_values({})
end

-- callback_124; bloques originales: 5
callbacks.callback_124 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.HitboxVisible = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Hitbox Visible"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Hitbox Invisible"
    end
    u("KaiserHub", l)
    captures[5].value()
    return unpack_values({})
end

-- callback_125; bloques originales: 15
callbacks.callback_125 = function(captures, arguments)
    local I, X, a, branch_result, g, l, o, q
    local e7 = {}
    do
        local temp_1
        temp_1 = arguments[1]
        branch_result = arguments[2]
        X = temp_1
    end
    if branch_result then
        return unpack_values({})
    end
    branch_result = (X.UserInputType == Enum.UserInputType.Keyboard)
    if branch_result then
        do
            local temp_16, temp_6
            temp_6 = X.KeyCode.Name
            temp_16 = (captures[3].value.Binds.ToggleHitboxVisible ~= "")
            branch_result = temp_16
            I, l = temp_16, temp_6
        end
        if branch_result then
            I = (l == captures[3].value.Binds.ToggleHitboxVisible)
        end
        branch_result = I
        if branch_result then
            captures[3].value.HitboxVisible = (not captures[3].value.HitboxVisible)
            branch_result = captures[4].value.HitboxVisible
            if branch_result then
                captures[4].value.HitboxVisible(captures[3].value.HitboxVisible)
            end
            do
                local temp_1, temp_7
                temp_1 = captures[5].value
                temp_7 = captures[3].value.HitboxVisible
                branch_result = temp_7
                a, g, q = temp_1, temp_1, temp_7
            end
            if branch_result then
                q = "Hitbox Visible"
            end
            branch_result = q
            o = q
            if (not branch_result) then
                o = "Hitbox Invisible"
            end
            g("KaiserHub", o)
            captures[6].value()
        end
    end
    return unpack_values({})
end

-- callback_126; bloques originales: 5
callbacks.callback_126 = function(captures, arguments)
    local branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_5
        temp_1 = arguments[1]
        captures[1].value.AutoEquipKnifeEnabled = temp_1
        temp_5 = captures[4].value
        branch_result = temp_1
        g, o, u = temp_5, temp_1, temp_5
    end
    if branch_result then
        o = "Auto Equip Cuchillo Activado"
    end
    branch_result = o
    l = o
    if (not branch_result) then
        l = "Auto Equip Cuchillo Desactivado"
    end
    u("KaiserHub", l)
    return unpack_values({})
end

-- callback_127; bloques originales: 1
callbacks.callback_127 = function(captures, arguments)
    local branch_result
    local e7 = {}
    InstantKillTarget(captures[1].value.Parent)
    return unpack_values({})
end

-- callback_128; bloques originales: 1
callbacks.callback_128 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({false})
end

-- callback_129; bloques originales: 1
callbacks.callback_129 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({})
end

-- callback_130; bloques originales: 1
callbacks.callback_130 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.Visible = (not captures[1].value.Visible)
    return unpack_values({})
end

-- callback_131; bloques originales: 1
callbacks.callback_131 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.Visible = false
    captures[4].value()
    return unpack_values({})
end

-- callback_132; bloques originales: 22
callbacks.callback_132 = function(captures, arguments)
    local A, B, D, I, J, X, a, branch_result, g, l, o, u
    local e7 = {}
    local steps = {}
    steps.entry = function()
        do
            local temp_1, temp_2, temp_5
            temp_1 = captures[1].value
            temp_2 = arguments[1]
            temp_5 = temp_1.Character
            branch_result = temp_5
            B, I, X = temp_5, temp_5, temp_2
        end
        if branch_result then
            I = B.FindFirstChild(B, "HumanoidRootPart")
        end
        branch_result = B
        I, l = B, I
        if branch_result then
            I = B.FindFirstChildOfClass(B, "Humanoid")
        end
        do
            local temp_1
            temp_1 = (not l)
            branch_result = temp_1
            I, u = temp_1, I
        end
        if (not branch_result) then
            I = (not X)
        end
        branch_result = I
        if branch_result then
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_13, temp_3
            temp_3 = l.CFrame
            temp_13 = (X.Position - temp_3.Position).Magnitude
            branch_result = (temp_13 < 4)
            g, o = temp_13, temp_3
        end
        if branch_result then
            l.CFrame = X
            l.AssemblyLinearVelocity = Vector3.zero
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_9
            temp_9 = math.max(1, unpack_values({math.ceil((g / 1.8))}))
            branch_result = u
            a = temp_9
        end
        if branch_result then
            u.PlatformStand = true
        end
        A, J = 0, a
        return "step_2"
    end
    steps.step_2 = function()
        do
            local temp_1
            temp_1 = (A + 1)
            branch_result = ((false and (J <= temp_1)) or ((not false) and (J >= temp_1)))
            A = temp_1
        end
        if branch_result then
            return "step_3"
        else
            return "step_5"
        end
    end
    steps.step_3 = function()
        do
            local temp_1
            temp_1 = (not B)
            branch_result = temp_1
            D, I = A, temp_1
        end
        if (not branch_result) then
            I = (not B.FindFirstChild(B, "HumanoidRootPart"))
        end
        branch_result = I
        if branch_result then
            return "step_4"
        else
            return "step_6"
        end
    end
    steps.step_4 = function()

        return "step_5"
    end
    steps.step_5 = function()
        l.CFrame = X
        l.AssemblyLinearVelocity = Vector3.zero
        l.AssemblyAngularVelocity = Vector3.zero
        branch_result = u
        if branch_result then
            u.PlatformStand = false
        end
        return nil, pack_values(unpack_values({}))
    end
    steps.step_6 = function()
        do
            local temp_19
            l.CFrame = o.Lerp(o, X, (D / a))
            l.AssemblyLinearVelocity = Vector3.zero
            l.AssemblyAngularVelocity = Vector3.zero
            temp_19 = captures[4].value.PreRender
            temp_19.Wait(temp_19)
        end
        return "step_2"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_133; bloques originales: 24
callbacks.callback_133 = function(captures, arguments)
    local B, X, branch_result, l, o
    local e7 = {}
    do
        local temp_34
        captures[1].value.ScriptActive = false
        captures[1].value.InvisibleEnabled = false
        captures[1].value.KillAuraEnabled = false
        captures[1].value.AimbotEnabled = false
        captures[1].value.HitboxEnabled = false
        captures[1].value.FlyEnabled = false
        captures[1].value.ShowFOV = false
        captures[1].value.AutoFarmEnabled = false
        temp_34 = {pairs(captures[4].value)}
        B, X, l = temp_34[3], temp_34[2], temp_34[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            table.clear(captures[4].value)
            branch_result = captures[5].value
            if branch_result then
                captures[5].value()
            end
            branch_result = captures[6].value
            if branch_result then
                captures[6].value()
            end
            branch_result = captures[7].value.Character
            if branch_result then
                do
                    local temp_4, temp_8
                    temp_4 = captures[7].value.Character
                    temp_8 = temp_4.FindFirstChild(temp_4, "HumanoidRootPart")
                    branch_result = temp_8
                    X = temp_8
                end
                if branch_result then
                    do
                        local temp_4
                        temp_4 = X.FindFirstChild(X, "KaiserFlyBV")
                        branch_result = temp_4
                        B = temp_4
                    end
                    if branch_result then
                        B.Destroy(B)
                    end
                end
            end
            branch_result = captures[8].value
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[8].value
                    temp_1.Destroy(temp_1)
                end
            end
            branch_result = captures[9].value
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[9].value
                    temp_1.Destroy(temp_1)
                end
            end
            do
                local temp_1
                temp_1 = captures[10].value
                branch_result = temp_1.FindFirstChild(temp_1, "KaiserUniversalGUI")
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = captures[10].value.KaiserUniversalGUI
                    temp_4.Destroy(temp_4)
                end
            end
            do
                local temp_1
                temp_1 = captures[10].value
                branch_result = temp_1.FindFirstChild(temp_1, "KaiserESP2D")
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = captures[10].value.KaiserESP2D
                    temp_4.Destroy(temp_4)
                end
            end
            do
                local temp_4
                print("KaiserHub cerrado y destruido por completo.")
                temp_4 = {}
                task.spawn(bind(callbacks.callback_195, {captures[2], captures[3]}))
                return unpack_values(temp_4)
            end
        end
        do
            local temp_1
            temp_1 = {}
            temp_1.value = o
            branch_result = temp_1.value
            o = temp_1
        end
        if branch_result then
            pcall(bind(callbacks.callback_30, {o}))
        end
    end
end

-- callback_134; bloques originales: 11
callbacks.callback_134 = function(captures, arguments)
    local B, I, X, branch_result, l
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = {}
        temp_1.value = arguments[1]
        temp_2 = {}
        temp_2.value = arguments[2]
        branch_result = writefile
        B, I, X = temp_2, writefile, temp_1
    end
    if branch_result then
        branch_result = isfile
        l = isfile
        if branch_result then
            l = getcustomasset
        end
        I = l
    end
    branch_result = I
    if branch_result then
        do
            local temp_2, temp_3, temp_4
            temp_2 = {pcall(bind(callbacks.callback_22, {B, X}))}
            temp_3 = temp_2[1]
            temp_4 = temp_2[2]
            branch_result = temp_3
            I, l = temp_3, temp_4
        end
        if branch_result then
            I = l
        end
        branch_result = I
        if branch_result then
            return unpack_values({l})
        end
    end
    return unpack_values({X.value})
end

-- callback_135; bloques originales: 1
callbacks.callback_135 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_13, temp_14, temp_18, temp_25, temp_26, temp_3, temp_30, temp_37, temp_38, temp_4,
            temp_42, temp_49, temp_5, temp_50, temp_54, temp_6, temp_7, temp_8, temp_9
        temp_1 = {}
        temp_3 = {}
        temp_4 = {}
        temp_5 = {}
        temp_6 = {}
        temp_7 = {}
        temp_4.value = arguments[1]
        temp_5.value = false
        temp_8 = {}
        temp_7.value = nil
        temp_1.value = nil
        temp_3.value = nil
        temp_9 = {}
        temp_9.value = nil
        temp_6.value = 0.22
        temp_8.value = bind(callbacks.save_configuration, {captures[1], captures[2], temp_1, temp_3, temp_9})
        temp_13 = table.insert
        temp_14 = captures[3].value
        temp_18 = temp_4.value.InputBegan
        temp_13(temp_14, unpack_values({temp_18.Connect(temp_18, bind(callbacks.callback_32, {captures[1], captures[2], temp_5, temp_1, temp_4, temp_3, temp_9}))}))
        temp_25 = table.insert
        temp_26 = captures[3].value
        temp_30 = temp_4.value.InputChanged
        temp_25(temp_26, unpack_values({temp_30.Connect(temp_30, bind(callbacks.callback_33, {captures[1], captures[2], temp_7}))}))
        temp_37 = table.insert
        temp_38 = captures[3].value
        temp_42 = captures[4].value.InputChanged
        temp_37(temp_38, unpack_values({temp_42.Connect(temp_42, bind(callbacks.callback_34, {temp_7, temp_5, temp_8}))}))
        temp_49 = table.insert
        temp_50 = captures[3].value
        temp_54 = captures[5].value.RenderStepped
        temp_49(temp_50, unpack_values({temp_54.Connect(temp_54, bind(callbacks.callback_35, {temp_9, temp_4, captures[1], captures[2], temp_6}))}))
        return unpack_values({})
    end
end

-- callback_136; bloques originales: 3
callbacks.callback_136 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        task.cancel(captures[1].value)
    end
    captures[1].value = task.delay(0.5, bind(callbacks.callback_36, {captures[1], captures[2], captures[3], captures[4], captures[5], captures[6]}))
    return unpack_values({})
end

-- callback_137; bloques originales: 3
callbacks.callback_137 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_2, temp_3
        temp_2 = {pcall(bind(callbacks.load_configuration, {captures[1], captures[2], captures[3], captures[4], captures[5], captures[6]}))}
        temp_3 = temp_2[2]
        branch_result = (not temp_2[1])
        X = temp_3
    end
    if branch_result then
        warn(("Error al cargar la configuraci贸n: " .. tostring(X)))
    end
    return unpack_values({})
end

-- callback_138; bloques originales: 37
callbacks.callback_138 = function(captures, arguments)
    local A, B, D, I, J, X, a, branch_result, g, l, o, q, z
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = temp_4
        I, X = temp_4, temp_4
    end
    if branch_result then
        I = X.FindFirstChild(X, "HumanoidRootPart")
    end
    branch_result = X
    B, I = I, X
    if branch_result then
        I = X.FindFirstChild(X, "Humanoid")
    end
    branch_result = B
    I, l = B, I
    if branch_result then
        I = captures[4].value
    end
    branch_result = I
    if branch_result then
        B.CFrame = captures[4].value.CFrame
        B.AssemblyLinearVelocity = Vector3.zero
        B.AssemblyAngularVelocity = Vector3.zero
    end
    branch_result = captures[5].value
    if branch_result then
        do
            local temp_1
            temp_1 = captures[5].value
            temp_1.Destroy(temp_1)
            captures[5].value = nil
        end
    end
    branch_result = captures[6].value
    if branch_result then
        do
            local temp_1
            temp_1 = captures[6].value
            temp_1.Destroy(temp_1)
            captures[6].value = nil
        end
    end
    branch_result = captures[4].value
    if branch_result then
        do
            local temp_1
            temp_1 = captures[4].value
            temp_1.Destroy(temp_1)
            captures[4].value = nil
        end
    end
    branch_result = l
    if branch_result then
        l.PlatformStand = false
        l.ChangeState(l, Enum.HumanoidStateType.GettingUp)
        l.DisplayDistanceType = Enum.HumanoidDisplayDistanceType.Viewer
    end
    do
        local temp_2
        temp_2 = {pairs(captures[7].value)}
        a, g, q = temp_2[3], temp_2[1], temp_2[2]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = g(q, a)
            branch_result = temp_1
            J, a = temp_2, temp_1
        end
        if (not branch_result) then
            captures[7].value = {}
            branch_result = X
            if branch_result then
                do
                    local temp_3
                    temp_3 = {pairs(unpack_values({X.GetDescendants(X)}))}
                    J, a, q = temp_3[3], temp_3[2], temp_3[1]
                end
                while true do
                    do
                        local temp_1, temp_2
                        temp_1, temp_2 = q(a, J)
                        branch_result = temp_1
                        A, J = temp_2, temp_1
                    end
                    if not branch_result then break end
                    do
                        local temp_4
                        temp_4 = A.IsA(A, "ParticleEmitter")
                        branch_result = temp_4
                        z = temp_4
                    end
                    if (not branch_result) then
                        do
                            local temp_4
                            temp_4 = A.IsA(A, "Trail")
                            branch_result = temp_4
                            D = temp_4
                        end
                        if (not branch_result) then
                            D = A.IsA(A, "BillboardGui")
                        end
                        z = D
                    end
                    branch_result = z
                    if branch_result then
                        A.Enabled = true
                    else
                        branch_result = A.IsA(A, "BasePart")
                        if branch_result then
                            A.CanCollide = true
                        end
                    end
                end
            end
            return unpack_values({})
        end
        branch_result = a
        A, o = a, a
        if branch_result then
            A = o.Parent
        end
        branch_result = A
        if branch_result then
            o.Transparency = J
        end
    end
end

-- callback_139; bloques originales: 14
callbacks.callback_139 = function(captures, arguments)
    local B, I, branch_result, g, l, o, u
    local e7 = {}
    do
        local temp_1, temp_10, temp_8, temp_9
        temp_1 = arguments[1]
        captures[1].value.InvisibleEnabled = temp_1
        captures[4].value = temp_1
        temp_8 = captures[5].value.Character
        temp_9 = {}
        temp_9.value = temp_8
        temp_10 = temp_9.value
        branch_result = temp_10
        B, I, l = temp_9, temp_10, temp_1
    end
    if branch_result then
        do
            local temp_1
            temp_1 = B.value
            I = temp_1.FindFirstChild(temp_1, "HumanoidRootPart")
        end
    end
    do
        local temp_1, temp_2
        temp_1 = {}
        temp_1.value = I
        temp_2 = B.value
        branch_result = temp_2
        I, l, u = temp_2, temp_1, l
    end
    if branch_result then
        do
            local temp_1
            temp_1 = B.value
            I = temp_1.FindFirstChild(temp_1, "Humanoid")
        end
    end
    do
        local temp_1, temp_3
        temp_1 = {}
        temp_1.value = I
        temp_3 = (not B.value)
        branch_result = temp_3
        I, o, u = temp_3, u, temp_1
    end
    if (not branch_result) then
        do
            local temp_2
            temp_2 = (not l.value)
            branch_result = temp_2
            g = temp_2
        end
        if (not branch_result) then
            g = (not u.value)
        end
        I = g
    end
    branch_result = I
    if branch_result then
        return unpack_values({})
    end
    branch_result = captures[4].value
    if branch_result then
        task.spawn(bind(callbacks.callback_10, {B, captures[2], captures[3], captures[6], l, u, captures[7], captures[8], captures[9]}))
    else
        captures[10].value()
    end
    return unpack_values({})
end

-- callback_140; bloques originales: 12
callbacks.callback_140 = function(captures, arguments)
    local B, I, X, branch_result, g, l, u
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.ScriptActive
        branch_result = temp_4
        I = temp_4
    end
    if branch_result then
        I = captures[1].value.InvisibleEnabled
    end
    branch_result = I
    if branch_result then
        do
            local temp_4
            temp_4 = captures[4].value.Character
            branch_result = temp_4
            X = temp_4
        end
        if branch_result then
            do
                local temp_3
                temp_3 = {ipairs(unpack_values({X.GetDescendants(X)}))}
                B, l, u = temp_3[2], temp_3[3], temp_3[1]
            end
            while true do
                do
                    local temp_1, temp_2
                    temp_1, temp_2 = u(B, l)
                    branch_result = temp_1
                    g, l = temp_2, temp_1
                end
                if not branch_result then break end
                branch_result = g.IsA(g, "BasePart")
                if branch_result then
                    g.CanCollide = false
                end
            end
        end
    end
    return unpack_values({})
end

-- callback_141; bloques originales: 7
callbacks.callback_141 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_2
        temp_2 = arguments[1]
        branch_result = temp_2.IsA(temp_2, "BasePart")
        X = temp_2
    end
    if branch_result then
        X.Material = Enum.Material.SmoothPlastic
        X.Reflectance = 0
    else
        do
            local temp_4
            temp_4 = X.IsA(X, "Decal")
            branch_result = temp_4
            I = temp_4
        end
        if (not branch_result) then
            I = X.IsA(X, "Texture")
        end
        branch_result = I
        if branch_result then
            X.Transparency = 1
        end
    end
    return unpack_values({})
end

-- callback_142; bloques originales: 31
callbacks.callback_142 = function(captures, arguments)
    local A, B, I, J, X, a, branch_result, g, l, o, q, u
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.ScriptActive
        branch_result = temp_4
        I = temp_4
    end
    if branch_result then
        do
            local temp_4
            temp_4 = captures[1].value.InvisibleEnabled
            branch_result = temp_4
            X = temp_4
        end
        if branch_result then
            do
                local temp_1
                temp_1 = captures[4].value
                branch_result = temp_1
                l = temp_1
            end
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[5].value
                    branch_result = temp_1
                    o = temp_1
                end
                if branch_result then
                    o = captures[6].value
                end
                l = o
            end
            X = l
        end
        I = X
    end
    branch_result = I
    if branch_result then
        do
            local temp_4
            temp_4 = captures[7].value.Character
            branch_result = temp_4
            I, X = temp_4, temp_4
        end
        if branch_result then
            I = X.FindFirstChild(X, "HumanoidRootPart")
        end
        branch_result = (not captures[8].value)
        B = I
        if branch_result then
            do
                local temp_1, temp_5
                temp_1 = captures[7].value
                temp_5 = temp_1.FindFirstChild(temp_1, "PlayerScripts")
                branch_result = temp_5
                l = temp_5
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = l.FindFirstChild(l, "PlayerModule")
                    branch_result = temp_4
                    u = temp_4
                end
                if branch_result then
                    do
                        local temp_1
                        temp_1 = require(u)
                        captures[8].value = temp_1.GetControls(temp_1)
                    end
                end
            end
        end
        branch_result = captures[8].value
        if branch_result then
            do
                local temp_25, temp_3, temp_4, temp_41, temp_45, temp_6, temp_9
                temp_3 = workspace.CurrentCamera
                temp_4 = captures[8].value
                temp_6 = temp_4.GetMoveVector(temp_4)
                temp_9 = temp_3.CFrame
                temp_25 = Vector3.new(temp_9.LookVector.X, 0, temp_9.LookVector.Z)
                temp_41 = Vector3.new(temp_9.RightVector.X, 0, temp_9.RightVector.Z)
                temp_45 = (temp_25.Magnitude > 0)
                branch_result = temp_45
                J, g, q, u = temp_45, temp_25, temp_41, temp_6
            end
            if branch_result then
                J = g.Unit
            end
            branch_result = J
            I = J
            if (not branch_result) then
                I = Vector3.new(0, 0, -1)
            end
            do
                local temp_4
                temp_4 = (q.Magnitude > 0)
                branch_result = temp_4
                A, g = temp_4, I
            end
            if branch_result then
                A = q.Unit
            end
            branch_result = A
            a = A
            if (not branch_result) then
                a = Vector3.new(1, 0, 0)
            end
            captures[5].value.Velocity = (((g * (- u.Z)) + (a * u.X)) * (captures[1].value.FlySpeed or 120))
            captures[6].value.CFrame = CFrame.new(captures[4].value.Position, (captures[4].value.Position + g))
        end
        branch_result = B
        if branch_result then
            B.CFrame = captures[4].value.CFrame
            B.AssemblyLinearVelocity = Vector3.zero
            B.AssemblyAngularVelocity = Vector3.zero
        end
    end
    return unpack_values({})
end

-- callback_143; bloques originales: 9
callbacks.callback_143 = function(captures, arguments)
    local B, I, X, branch_result, l
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = arguments[1]
        temp_2 = (not temp_1)
        branch_result = temp_2
        I, X = temp_2, temp_1
    end
    if (not branch_result) then
        I = (not X.Parent)
    end
    branch_result = I
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_3, temp_6
        temp_3 = X.Position
        temp_6 = X.AssemblyLinearVelocity
        branch_result = temp_6
        B, I = temp_3, temp_6
    end
    if (not branch_result) then
        I = Vector3.zero
    end
    branch_result = (I.Magnitude < 0.1)
    l = I
    if branch_result then
        return unpack_values({B})
    end
    do
        local temp_1, temp_2
        temp_1 = {}
        temp_2 = bind(callbacks.callback_103, {captures[3], temp_1})
        temp_1.value = 0.03
        pcall(temp_2)
        return unpack_values({(B + (l * (temp_1.value + (((l.Magnitude > 30) and 0.025) or 0.015))))})
    end
end

-- callback_144; bloques originales: 31
callbacks.callback_144 = function(captures, arguments)
    local A, B, F, I, J, K, M, O, Q, S, V, W, X, a, branch_result, g, l, n, o, q, u, w, y, z
    local e7 = {}
    do
        local temp_1, temp_2, temp_3, temp_4
        temp_1 = arguments[3]
        temp_2 = arguments[1]
        temp_3 = arguments[2]
        temp_4 = (not temp_2)
        branch_result = temp_4
        B, I, X, l = temp_3, temp_4, temp_2, temp_1
    end
    if (not branch_result) then
        I = (not X.Parent)
    end
    branch_result = I
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_4
        temp_4 = captures[3].value.Character
        branch_result = temp_4
        I, u = temp_4, temp_4
    end
    if branch_result then
        I = u.FindFirstChild(u, "HumanoidRootPart")
    end
    do
        local temp_3, temp_7
        temp_3 = X.Parent
        temp_7 = temp_3.FindFirstChild(temp_3, "HumanoidRootPart")
        branch_result = temp_7
        I, g, o = temp_7, temp_3, I
    end
    if (not branch_result) then
        I = X
    end
    do
        local temp_4
        temp_4 = g.FindFirstChildOfClass(g, "Humanoid")
        branch_result = (not o)
        a, q = temp_4, I
    end
    if branch_result then
        return unpack_values({X.Position})
    end
    do
        local temp_10, temp_11, temp_12, temp_16, temp_26, temp_3, temp_4, temp_7
        temp_3 = g.Name
        temp_4 = tick()
        temp_7 = X.Position
        temp_10 = {}
        temp_11 = q.AssemblyLinearVelocity
        temp_12 = bind(callbacks.callback_199, {captures[3], captures[1], captures[2], temp_10, captures[4]})
        temp_10.value = 0.03
        pcall(temp_12)
        temp_16 = ((temp_10.value / 2) + 0.016)
        temp_26 = (q.Position - o.Position).Magnitude
        branch_result = (not l)
        A, J, K, M, n, y, z = temp_4, temp_3, temp_11, temp_16, temp_26, temp_16, temp_7
    end
    if branch_result then
        branch_result = B
        S = B
        if branch_result then
            S = (B > 0)
        end
        branch_result = S
        Q = S
        if branch_result then
            Q = B
        end
        y = ((n / (Q or 1200)) + M)
    end
    do
        local temp_2
        temp_2 = captures[5].value[J]
        branch_result = temp_2
        Q = temp_2
    end
    if (not branch_result) then
        Q = {["lastVel"] = K, ["lastTime"] = A}
    end
    do
        local temp_13
        temp_13 = ((K - Q.lastVel) / math.max((A - Q.lastTime), 0.001))
        branch_result = (K.Dot(K, Q.lastVel) < 0)
        V = temp_13
    end
    if branch_result then
        V = Vector3.zero
    end
    do
        local temp_12
        captures[5].value[J] = {["lastVel"] = K, ["lastTime"] = A}
        temp_12 = ((z + (K * y)) + ((0.5 * V) * (y ^ 2)))
        branch_result = a
        W, w = temp_12, a
    end
    if branch_result then
        do
            local temp_10
            temp_10 = (a.FloorMaterial == Enum.Material.Air)
            branch_result = temp_10
            F = temp_10
        end
        if (not branch_result) then
            do
                local temp_9
                temp_9 = (a.GetState(a) == Enum.HumanoidStateType.Freefall)
                branch_result = temp_9
                O = temp_9
            end
            if (not branch_result) then
                O = (a.GetState(a) == Enum.HumanoidStateType.Jumping)
            end
            F = O
        end
        w = F
    end
    branch_result = w
    if branch_result then
        W = Vector3.new(W.X, ((z.Y + (K.Y * y)) - ((0.5 * (workspace.Gravity or 196.2)) * (y ^ 2))), W.Z)
    end
    do
        local temp_18, temp_4
        temp_4 = RaycastParams.new()
        temp_4.FilterType = Enum.RaycastFilterType.Exclude
        temp_4.FilterDescendantsInstances = {g, u}
        temp_18 = workspace.Raycast(workspace, z, (W - z), temp_4)
        branch_result = temp_18
        F = temp_18
    end
    if branch_result then
        W = (F.Position - ((W - z).Unit * 0.3))
    end
    return unpack_values({W})
end

-- callback_145; bloques originales: 51
callbacks.callback_145 = function(captures, arguments)
    local A, B, D, I, J, K, M, X, a, branch_result, g, l, n, o, q, u, y
    local e7 = {}
    local steps = {}
    steps.entry = function()
        do
            local temp_1, temp_2
            temp_1 = arguments[1]
            temp_2 = (not temp_1)
            branch_result = temp_2
            I, X = temp_2, temp_1
        end
        if (not branch_result) then
            I = (X == captures[1].value)
        end
        branch_result = I
        if branch_result then
            return nil, pack_values(unpack_values({false}))
        end
        branch_result = (not captures[2].value.AimbotTeamCheck)
        if branch_result then
            return nil, pack_values(unpack_values({true}))
        end
        do
            local temp_4
            temp_4 = captures[1].value.Team
            branch_result = temp_4
            I = temp_4
        end
        if branch_result then
            I = X.Team
        end
        branch_result = I
        if branch_result then
            return nil, pack_values(unpack_values({(captures[1].value.Team ~= X.Team)}))
        end
        do
            local temp_3
            temp_3 = X.Character
            branch_result = (not temp_3)
            B = temp_3
        end
        if branch_result then
            return nil, pack_values(unpack_values({false}))
        end
        do
            local temp_1, temp_3
            temp_1 = tick()
            temp_3 = captures[5].value[X]
            branch_result = temp_3
            I, l = temp_3, temp_1
        end
        if branch_result then
            I = ((l - captures[5].value[X].lastCheck) < captures[6].value)
        end
        branch_result = I
        if branch_result then
            return nil, pack_values(unpack_values({captures[5].value[X].isEnemy}))
        end
        do
            local temp_5
            temp_5 = B.FindFirstChild(B, "HumanoidRootPart")
            branch_result = temp_5
            g, o, q, u = temp_5, temp_5, temp_5, true
        end
        if branch_result then
            g = o.FindFirstChild(o, "TeammateIconPart")
        end
        branch_result = g
        I = g
        if (not branch_result) then
            I = B.FindFirstChild(B, "TeammateIconPart")
        end
        branch_result = I
        if branch_result then
            return "step_2"
        else
            return "step_4"
        end
    end
    steps.step_2 = function()
        u = false
        return "step_3"
    end
    steps.step_3 = function()
        do
            local temp_1, temp_6
            temp_1 = captures[5].value
            temp_6 = {u}
            temp_1[X] = {["isEnemy"] = u, ["lastCheck"] = l}
            return nil, pack_values(unpack_values(temp_6))
        end
    end
    steps.step_4 = function()
        do
            local temp_4
            temp_4 = B.FindFirstChild(B, "Head")
            branch_result = temp_4
            a, g = temp_4, temp_4
        end
        if branch_result then
            a = g.FindFirstChildOfClass(g, "BillboardGui")
        end
        branch_result = a
        I = a
        if (not branch_result) then
            I = B.FindFirstChildOfClass(B, "BillboardGui")
        end
        branch_result = I
        q = I
        if branch_result then
            return "step_5"
        else
            return "step_11"
        end
    end
    steps.step_5 = function()
        do
            local temp_3
            temp_3 = {ipairs(unpack_values({q.GetDescendants(q)}))}
            A, J, a = temp_3[3], temp_3[2], temp_3[1]
        end
        return "step_6"
    end
    steps.step_6 = function()
        do
            local temp_1, temp_2
            temp_1, temp_2 = a(J, A)
            branch_result = temp_1
            A, K = temp_1, temp_2
        end
        if branch_result then
            return "step_7"
        else
            return "step_10"
        end
    end
    steps.step_7 = function()
        do
            local temp_4
            temp_4 = K.IsA(K, "ImageLabel")
            branch_result = temp_4
            I = temp_4
        end
        if (not branch_result) then
            I = K.IsA(K, "ImageButton")
        end
        branch_result = I
        if branch_result then
            return "step_8"
        else
            return "step_14"
        end
    end
    steps.step_8 = function()
        do
            local temp_3
            temp_3 = K.ImageColor3
            branch_result = temp_3
            D, I = temp_3, temp_3
        end
        if branch_result then
            do
                local temp_4
                temp_4 = (D.G > 0.6)
                branch_result = temp_4
                n = temp_4
            end
            if branch_result then
                n = (D.R < 0.5)
            end
            I = n
        end
        branch_result = I
        if branch_result then
            return "step_9"
        else
            return "step_12"
        end
    end
    steps.step_9 = function()
        u = false
        return "step_10"
    end
    steps.step_10 = function()

        return "step_11"
    end
    steps.step_11 = function()

        return "step_3"
    end
    steps.step_12 = function()

        return "step_13"
    end
    steps.step_13 = function()

        return "step_6"
    end
    steps.step_14 = function()
        branch_result = K.IsA(K, "Frame")
        if branch_result then
            return "step_15"
        else
            return "step_13"
        end
    end
    steps.step_15 = function()
        do
            local temp_3
            temp_3 = K.BackgroundColor3
            branch_result = temp_3
            D, M = temp_3, temp_3
        end
        if branch_result then
            do
                local temp_4
                temp_4 = (D.G > 0.6)
                branch_result = temp_4
                y = temp_4
            end
            if branch_result then
                y = (D.R < 0.5)
            end
            M = y
        end
        branch_result = M
        if branch_result then
            return "step_16"
        else
            return "step_17"
        end
    end
    steps.step_16 = function()
        u = false
        return "step_10"
    end
    steps.step_17 = function()

        return "step_13"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_146; bloques originales: 5
callbacks.callback_146 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_2, temp_3, temp_7
        temp_1 = arguments[1]
        temp_2 = captures[1].value
        temp_3 = arguments[2]
        temp_7 = (not temp_2.NotificationsEnabled)
        branch_result = temp_7
        B, I, X = temp_3, temp_7, temp_1
    end
    if (not branch_result) then
        I = (not captures[1].value.ScriptActive)
    end
    branch_result = I
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_4
        temp_4 = game.GetService(game, "StarterGui")
        temp_4.SetCore(temp_4, "SendNotification", {["Title"] = X, ["Text"] = B, ["Duration"] = captures[1].value.NotificationDuration})
        return unpack_values({})
    end
end

-- callback_147; bloques originales: 8
callbacks.callback_147 = function(captures, arguments)
    local B, X, branch_result, g, l, o
    local e7 = {}
    do
        local temp_1, temp_4
        temp_1 = captures[1].value
        temp_4 = {ipairs(unpack_values({temp_1.GetPlayers(temp_1)}))}
        B, X, l = temp_4[3], temp_4[2], temp_4[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            return unpack_values({})
        end
        branch_result = o.Character
        if branch_result then
            do
                local temp_3, temp_7
                temp_3 = o.Character
                temp_7 = temp_3.FindFirstChild(temp_3, "KaiserHitboxPart")
                branch_result = temp_7
                g = temp_7
            end
            if branch_result then
                g.Destroy(g)
            end
        end
    end
end

-- callback_148; bloques originales: 25
callbacks.callback_148 = function(captures, arguments)
    local D, I, J, branch_result, l, n, o, q, u, z
    local e7 = {}
    branch_result = (not arguments[1])
    if (not branch_result) then
        do
            local temp_10, temp_20
            captures[2].value("KaiserHub", "Reinicia para recuperar Texturas")
            temp_10 = game.GetService(game, "Lighting")
            temp_10.GlobalShadows = false
            temp_10.FogEnd = 9000000000
            temp_10.Brightness = 0.5
            temp_20 = {pairs(unpack_values({temp_10.GetDescendants(temp_10)}))}
            l, o, u = temp_20[1], temp_20[3], temp_20[2]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = l(u, o)
                branch_result = temp_1
                o, q = temp_1, temp_2
            end
            if (not branch_result) then
                do
                    local temp_3
                    temp_3 = {pairs(unpack_values({workspace.GetDescendants(workspace)}))}
                    l, o, u = temp_3[1], temp_3[3], temp_3[2]
                end
                while true do
                    do
                        local temp_1, temp_2
                        temp_1, temp_2 = l(u, o)
                        branch_result = temp_1
                        o, q = temp_1, temp_2
                    end
                    if not branch_result then break end
                    captures[5].value(q)
                end
                branch_result = (not captures[1].value)
                if branch_result then
                    do
                        local temp_3
                        temp_3 = workspace.DescendantAdded
                        captures[1].value = temp_3.Connect(temp_3, bind(callbacks.callback_38, {captures[3], captures[4], captures[5]}))
                    end
                end
                return unpack_values({})
            end
            do
                local temp_4
                temp_4 = q.IsA(q, "BlurEffect")
                branch_result = temp_4
                I = temp_4
            end
            if (not branch_result) then
                do
                    local temp_4
                    temp_4 = q.IsA(q, "SunRaysEffect")
                    branch_result = temp_4
                    J = temp_4
                end
                if (not branch_result) then
                    do
                        local temp_4
                        temp_4 = q.IsA(q, "ColorCorrectionEffect")
                        branch_result = temp_4
                        z = temp_4
                    end
                    if (not branch_result) then
                        do
                            local temp_4
                            temp_4 = q.IsA(q, "BloomEffect")
                            branch_result = temp_4
                            D = temp_4
                        end
                        if (not branch_result) then
                            do
                                local temp_4
                                temp_4 = q.IsA(q, "Atmosphere")
                                branch_result = temp_4
                                n = temp_4
                            end
                            if (not branch_result) then
                                n = q.IsA(q, "DepthOfFieldEffect")
                            end
                            D = n
                        end
                        z = D
                    end
                    J = z
                end
                I = J
            end
            branch_result = I
            if branch_result then
                q.Enabled = false
            end
        end
    end
    branch_result = captures[1].value
    if branch_result then
        do
            local temp_1
            temp_1 = captures[1].value
            temp_1.Disconnect(temp_1)
            captures[1].value = nil
        end
    end
    captures[2].value("KaiserHub", "Reinicia para recuperar Texturas")
    return unpack_values({})
end

-- callback_149; bloques originales: 1
callbacks.callback_149 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({unpack_values({captures[1].value(arguments[1])})})
end

-- callback_150; bloques originales: 24
callbacks.callback_150 = function(captures, arguments)
    local B, I, X, branch_result, l, o, q, u
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = (not temp_4)
        X = temp_4
    end
    if branch_result then
        return unpack_values({true})
    end
    branch_result = X.FindFirstChildOfClass(X, "ForceField")
    if branch_result then
        return unpack_values({true})
    end
    branch_result = captures[1].value.Team
    if branch_result then
        do
            local temp_11, temp_17
            temp_11 = string.lower(captures[1].value.Team.Name)
            temp_17 = string.find(temp_11, "lobby")
            branch_result = temp_17
            B, I = temp_11, temp_17
        end
        if (not branch_result) then
            do
                local temp_6
                temp_6 = string.find(B, "spectat")
                branch_result = temp_6
                l = temp_6
            end
            if (not branch_result) then
                do
                    local temp_6
                    temp_6 = string.find(B, "espectador")
                    branch_result = temp_6
                    o = temp_6
                end
                if (not branch_result) then
                    do
                        local temp_6
                        temp_6 = string.find(B, "menu")
                        branch_result = temp_6
                        q = temp_6
                    end
                    if (not branch_result) then
                        q = string.find(B, "dead")
                    end
                    o = q
                end
                l = o
            end
            I = l
        end
        branch_result = I
        if branch_result then
            return unpack_values({true})
        end
    end
    do
        local temp_4
        temp_4 = X.FindFirstChild(X, "HumanoidRootPart")
        branch_result = temp_4
        B = temp_4
    end
    if branch_result then
        do
            local temp_2
            temp_2 = {ipairs(captures[4].value)}
            l, o, u = temp_2[2], temp_2[1], temp_2[3]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = o(l, u)
                branch_result = temp_1
                q, u = temp_2, temp_1
            end
            if not branch_result then break end
            branch_result = ((B.Position - q.Centro).Magnitude <= q.Radio)
            if branch_result then
                return unpack_values({true})
            end
        end
    end
    return unpack_values({false})
end

-- callback_151; bloques originales: 6
callbacks.callback_151 = function(captures, arguments)
    local B, branch_result, l, o, q, u
    local e7 = {}
    do
        local temp_1, temp_3, temp_6
        temp_1 = {}
        temp_3 = captures[1].value
        temp_6 = {ipairs(unpack_values({temp_3.GetPlayers(temp_3)}))}
        B, l, o, u = temp_1, temp_6[2], temp_6[1], temp_6[3]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = o(l, u)
            branch_result = temp_1
            q, u = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({B})
        end
        branch_result = q.Character
        if branch_result then
            table.insert(B, q.Character)
        end
    end
end

-- callback_152; bloques originales: 21
callbacks.callback_152 = function(captures, arguments)
    local B, I, X, branch_result, u
    local e7 = {}
    do
        local temp_1
        temp_1 = arguments[1]
        branch_result = (not temp_1)
        X = temp_1
    end
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_4
        temp_4 = X.GetAttribute(X, "Downed")
        branch_result = temp_4
        I = temp_4
    end
    if (not branch_result) then
        do
            local temp_4
            temp_4 = X.GetAttribute(X, "Knocked")
            branch_result = temp_4
            B = temp_4
        end
        if (not branch_result) then
            do
                local temp_4
                temp_4 = X.GetAttribute(X, "IsDowned")
                branch_result = temp_4
                u = temp_4
            end
            if (not branch_result) then
                u = X.GetAttribute(X, "KO")
            end
            B = u
        end
        I = B
    end
    branch_result = I
    if branch_result then
        return unpack_values({true})
    end
    do
        local temp_4
        temp_4 = X.FindFirstChild(X, "Downed")
        branch_result = temp_4
        I = temp_4
    end
    if (not branch_result) then
        do
            local temp_4
            temp_4 = X.FindFirstChild(X, "Knocked")
            branch_result = temp_4
            B = temp_4
        end
        if (not branch_result) then
            B = X.FindFirstChild(X, "KO")
        end
        I = B
    end
    branch_result = I
    if branch_result then
        return unpack_values({true})
    end
    do
        local temp_4
        temp_4 = X.FindFirstChildOfClass(X, "Humanoid")
        branch_result = temp_4
        B, I = temp_4, temp_4
    end
    if branch_result then
        I = (B.Health < 15)
    end
    branch_result = I
    if branch_result then
    
    end
    return unpack_values({false})
end

-- callback_153; bloques originales: 18
callbacks.callback_153 = function(captures, arguments)
    local B, I, X, a, branch_result, g, o, u
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = arguments[1]
        temp_2 = (not temp_1)
        branch_result = temp_2
        I, X = temp_2, temp_1
    end
    if (not branch_result) then
        I = (not X.IsA(X, "Tool"))
    end
    branch_result = I
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_5
        temp_5 = X.FindFirstChild(X, "Throw", true)
        branch_result = temp_5
        I = temp_5
    end
    if (not branch_result) then
        do
            local temp_5
            temp_5 = X.FindFirstChild(X, "KnifeClient", true)
            branch_result = temp_5
            B = temp_5
        end
        if (not branch_result) then
            do
                local temp_5
                temp_5 = X.FindFirstChild(X, "KnifeServer", true)
                branch_result = temp_5
                u = temp_5
            end
            if (not branch_result) then
                u = X.FindFirstChild(X, "ThrowingKinfeHandlerScript", true)
            end
            B = u
        end
        I = B
    end
    branch_result = I
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_51, temp_7
        temp_7 = string.lower(X.Name)
        temp_51 = {ipairs({"combat", "fist", "wallet", "phone", "punch", "boombox", "radio", "knife", "blade", "cuchillo", "dagger", "kunai", "sword", "toy", "juguete", "pizza", "burger", "teddy", "balloon", "drink", "food"})}
        B, g, o, u = temp_7, temp_51[1], temp_51[3], temp_51[2]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = g(u, o)
            branch_result = temp_1
            a, o = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({true})
        end
        branch_result = string.find(B, a)
        if not (not branch_result) then break end
    
    end
    return unpack_values({false})
end

-- callback_154; bloques originales: 18
callbacks.callback_154 = function(captures, arguments)
    local A, B, I, J, X, branch_result, g, l, o, q, u
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = (not temp_4)
        X = temp_4
    end
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_4
        temp_4 = X.FindFirstChildOfClass(X, "Humanoid")
        branch_result = (not temp_4)
        B = temp_4
    end
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_4
        temp_4 = X.FindFirstChildOfClass(X, "Tool")
        branch_result = temp_4
        I, l = temp_4, temp_4
    end
    if branch_result then
        I = captures[4].value(l)
    end
    branch_result = I
    if branch_result then
        return unpack_values({l})
    end
    do
        local temp_1, temp_5
        temp_1 = captures[1].value
        temp_5 = temp_1.FindFirstChild(temp_1, "Backpack")
        branch_result = temp_5
        u = temp_5
    end
    if branch_result then
        do
            local temp_3
            temp_3 = {ipairs(unpack_values({u.GetChildren(u)}))}
            g, o, q = temp_3[3], temp_3[2], temp_3[1]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = q(o, g)
                branch_result = temp_1
                J, g = temp_2, temp_1
            end
            if not branch_result then break end
            do
                local temp_4
                temp_4 = J.IsA(J, "Tool")
                branch_result = temp_4
                A = temp_4
            end
            if branch_result then
                A = captures[4].value(J)
            end
            branch_result = A
            if branch_result then
                do
                    local temp_1
                    temp_1 = {J}
                    B.EquipTool(B, J)
                    task.wait(0.04)
                    return unpack_values(temp_1)
                end
            end
        end
    end
    return unpack_values({nil})
end

-- callback_155; bloques originales: 52
callbacks.callback_155 = function(captures, arguments)
    local A, B, D, I, J, K, M, Q, S, X, a, branch_result, g, l, n, o, q, u, y, z
    local e7 = {}
    do
        local temp_3, temp_4, temp_8
        temp_3 = workspace.CurrentCamera
        temp_4 = {}
        temp_4.value = temp_3
        temp_8 = captures[3].value.Character
        branch_result = temp_8
        B, I, X = temp_8, temp_8, temp_4
    end
    if branch_result then
        I = B.FindFirstChild(B, "Head")
    end
    do
        local temp_1, temp_3
        temp_1 = {}
        temp_1.value = I
        temp_3 = (not X.value)
        branch_result = temp_3
        I, l = temp_3, temp_1
    end
    if (not branch_result) then
        do
            local temp_1
            temp_1 = (not B)
            branch_result = temp_1
            u = temp_1
        end
        if (not branch_result) then
            u = (not l.value)
        end
        I = u
    end
    branch_result = I
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_1, temp_2
        temp_1 = bind(callbacks.callback_80, {captures[1], captures[2], captures[4], X, l})
        temp_2 = captures[5].value
        branch_result = temp_2
        I, o = temp_2, temp_1
    end
    if branch_result then
        I = captures[5].value.Parent
    end
    branch_result = I
    if branch_result then
        do
            local temp_11, temp_4, temp_8, temp_9
            temp_4 = captures[5].value.Parent
            temp_8 = temp_4.FindFirstChildOfClass(temp_4, "Humanoid")
            temp_9 = captures[6].value
            temp_11 = temp_9.GetPlayerFromCharacter(temp_9, temp_4)
            branch_result = temp_8
            I, a, g, q = temp_8, temp_11, temp_4, temp_8
        end
        if branch_result then
            do
                local temp_4
                temp_4 = (q.Health > 0)
                branch_result = temp_4
                J = temp_4
            end
            if branch_result then
                branch_result = a
                z = a
                if branch_result then
                    do
                        local temp_2
                        temp_2 = captures[7].value(a)
                        branch_result = temp_2
                        D = temp_2
                    end
                    if branch_result then
                        D = (not captures[8].value(g))
                    end
                    z = D
                end
                J = z
            end
            I = J
        end
        branch_result = I
        if branch_result then
            branch_result = ((l.value.Position - captures[5].value.Position).Magnitude <= 350)
            if branch_result then
                branch_result = o(captures[5].value, g)
                if branch_result then
                    return unpack_values({captures[5].value})
                end
            end
        end
    end
    do
        local temp_3, temp_4, temp_7
        temp_3 = math.huge
        temp_4 = captures[6].value
        temp_7 = {ipairs(unpack_values({temp_4.GetPlayers(temp_4)}))}
        A, J, a, g, q = temp_7[1], temp_7[3], temp_7[2], nil, temp_3
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = A(a, J)
            branch_result = temp_1
            J, K = temp_1, temp_2
        end
        if (not branch_result) then
            do
                local temp_1
                temp_1 = {g}
                captures[5].value = g
                return unpack_values(temp_1)
            end
        end
        do
            local temp_2
            temp_2 = (K ~= captures[3].value)
            branch_result = temp_2
            D = temp_2
        end
        if branch_result then
            do
                local temp_2
                temp_2 = captures[7].value(K)
                branch_result = temp_2
                M = temp_2
            end
            if branch_result then
                M = K.Character
            end
            D = M
        end
        branch_result = D
        if branch_result then
            do
                local temp_11, temp_3, temp_7
                temp_3 = K.Character
                temp_7 = temp_3.FindFirstChildOfClass(temp_3, "Humanoid")
                temp_11 = temp_3.FindFirstChild(temp_3, "Head")
                branch_result = temp_11
                D, M, n = temp_3, temp_7, temp_11
            end
            if (not branch_result) then
                n = D.FindFirstChild(D, "HumanoidRootPart")
            end
            branch_result = M
            y = M
            if branch_result then
                do
                    local temp_4
                    temp_4 = (M.Health > 0)
                    branch_result = temp_4
                    Q = temp_4
                end
                if branch_result then
                    do
                        local temp_3
                        temp_3 = (not captures[8].value(D))
                        branch_result = temp_3
                        S = temp_3
                    end
                    if branch_result then
                        S = n
                    end
                    Q = S
                end
                y = Q
            end
            branch_result = y
            if branch_result then
                do
                    local temp_11, temp_12
                    temp_11 = (l.value.Position - n.Position).Magnitude
                    temp_12 = (temp_11 <= 350)
                    branch_result = temp_12
                    Q, y = temp_12, temp_11
                end
                if branch_result then
                    Q = (y < q)
                end
                branch_result = Q
                if branch_result then
                    branch_result = o(n, D)
                    if branch_result then
                        g, q = n, y
                    end
                end
            end
        end
    end
end

-- callback_156; bloques originales: 5
callbacks.callback_156 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = temp_4
        I, X = temp_4, temp_4
    end
    if branch_result then
        I = X.FindFirstChildOfClass(X, "Humanoid")
    end
    branch_result = I
    B = I
    if branch_result then
        B.UnequipTools(B)
    end
    return unpack_values({})
end

-- callback_157; bloques originales: 37
callbacks.callback_157 = function(captures, arguments)
    local B, I, Q, X, a, branch_result, g, l, n, o, q, u, y
    local e7 = {}
    local steps = {}
    steps.entry = function()

        return "step_2"
    end
    steps.step_2 = function()
        branch_result = task.wait(0.03)
        if (not branch_result) then
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_1, temp_2, temp_4
            temp_1 = captures[3].value
            temp_2 = captures[1].value
            temp_4 = temp_1.AutoShootEnabled
            branch_result = temp_4
            I, u = temp_4, temp_2
        end
        if branch_result then
            do
                local temp_1, temp_4
                temp_1 = captures[3].value
                temp_4 = temp_1.ScriptActive
                branch_result = temp_4
                X, u = temp_4, temp_1
            end
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[4].value
                    X, u = (not temp_1()), temp_1
                end
            end
            I = X
        end
        branch_result = I
        if branch_result then
            return "step_3"
        else
            return "step_9"
        end
    end
    steps.step_3 = function()
        branch_result = ((tick() - captures[5].value) < captures[6].value)
        if branch_result then
            return "step_4"
        else
            return "step_5"
        end
    end
    steps.step_4 = function()
        captures[7].value()
        getgenv().KaiserTargetPart = nil
        return "step_2"
    end
    steps.step_5 = function()
        do
            local temp_4
            temp_4 = captures[8].value.Character
            branch_result = temp_4
            B, I = temp_4, temp_4
        end
        if branch_result then
            I = B.FindFirstChild(B, "HumanoidRootPart")
        end
        do
            local temp_1
            temp_1 = (not B)
            branch_result = temp_1
            I, l = temp_1, I
        end
        if (not branch_result) then
            I = (not l)
        end
        branch_result = I
        if branch_result then
            return "step_6"
        else
            return "step_7"
        end
    end
    steps.step_6 = function()

        return "step_2"
    end
    steps.step_7 = function()
        do
            local temp_1
            temp_1 = {}
            temp_1.value = captures[9].value()
            branch_result = temp_1.value
            u = temp_1
        end
        if branch_result then
            do
                local temp_2
                temp_2 = captures[10].value()
                branch_result = temp_2
                o = temp_2
            end
            if branch_result then
                do
                    local temp_7
                    getgenv().KaiserTargetPart = u.value
                    temp_7 = workspace.CurrentCamera
                    branch_result = temp_7
                    g = temp_7
                end
                if branch_result then
                    do
                        local temp_10, temp_4, temp_7
                        temp_4 = g.CFrame
                        temp_7 = l.CFrame
                        temp_10 = captures[11].value(u.value, 2000, true)
                        branch_result = temp_10
                        I, a, q = temp_10, temp_7, temp_4
                    end
                    if (not branch_result) then
                        I = u.value.Position
                    end
                    do
                        local temp_1, temp_11, temp_14, temp_26, temp_3
                        temp_1 = captures[12].value
                        temp_3 = temp_1.GetMouseLocation(temp_1)
                        temp_11 = g.ViewportPointToRay(g, temp_3.X, temp_3.Y)
                        temp_14 = g.CFrame
                        temp_26 = CFrame.lookAt(Vector3.zero, temp_14.VectorToObjectSpace(temp_14, temp_11.Direction))
                        Q, n, y = 0, (CFrame.lookAt(g.CFrame.Position, (g.CFrame.Position + (I - g.CFrame.Position).Unit)) * temp_26.Inverse(temp_26)), Vector3.new(I.X, l.Position.Y, I.Z)
                    end
                    while true do
                        do
                            local temp_1
                            temp_1 = (1 + Q)
                            branch_result = ((false and (temp_1 >= 2)) or ((not false) and (2 >= temp_1)))
                            Q = temp_1
                        end
                        if not branch_result then break end
                        g.CFrame = n
                        l.CFrame = CFrame.lookAt(l.Position, y)
                        branch_result = (Q == 1)
                        if branch_result then
                            o.Activate(o)
                            branch_result = u.value.Parent
                            if branch_result then
                                pcall(bind(callbacks.callback_127, {u, captures[1], captures[2]}))
                            end
                        end
                        do
                            local temp_4
                            temp_4 = captures[13].value.RenderStepped
                            temp_4.Wait(temp_4)
                        end
                    end
                    captures[5].value = tick()
                    branch_result = (not captures[3].value.AimbotEnabled)
                    if branch_result then
                        g.CFrame = q
                        l.CFrame = a
                    end
                    task.wait(0.04)
                    captures[7].value()
                end
            end
        else
            getgenv().KaiserTargetPart = nil
        end
        return "step_8"
    end
    steps.step_8 = function()

        return "step_2"
    end
    steps.step_9 = function()
        getgenv().KaiserTargetPart = nil
        return "step_8"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_158; bloques originales: 9
callbacks.callback_158 = function(captures, arguments)
    local B, I, X, branch_result, l
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = arguments[1]
        temp_2 = (not temp_1)
        branch_result = temp_2
        I, X = temp_2, temp_1
    end
    if (not branch_result) then
        I = (not X.Parent)
    end
    branch_result = I
    if branch_result then
        return unpack_values({nil})
    end
    do
        local temp_3, temp_6
        temp_3 = X.Position
        temp_6 = X.AssemblyLinearVelocity
        branch_result = temp_6
        B, I = temp_3, temp_6
    end
    if (not branch_result) then
        I = Vector3.zero
    end
    branch_result = (I.Magnitude < 0.1)
    l = I
    if branch_result then
        return unpack_values({B})
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = 0.03
        pcall(bind(callbacks.callback_40, {captures[3], captures[1], captures[2], temp_1, captures[4]}))
        return unpack_values({(B + (l * (temp_1.value + 0.015)))})
    end
end

-- callback_159; bloques originales: 22
callbacks.callback_159 = function(captures, arguments)
    local A, B, I, X, a, branch_result, g, l, o, q, u, z
    local e7 = {}
    do
        local temp_1
        temp_1 = {}
        temp_1.value = arguments[1]
        branch_result = (not temp_1.value)
        X = temp_1
    end
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = (not temp_4)
        B = temp_4
    end
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_4, temp_5
        temp_4 = B.FindFirstChildOfClass(B, "Tool")
        temp_5 = {}
        temp_5.value = temp_4
        branch_result = (not temp_5.value)
        l = temp_5
    end
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_3, temp_7
        pcall(bind(callbacks.callback_21, {l}))
        temp_3 = l.value
        temp_7 = temp_3.FindFirstChild(temp_3, "Handle")
        branch_result = temp_7
        I = temp_7
    end
    if (not branch_result) then
        do
            local temp_1, temp_5
            temp_1 = l.value
            temp_5 = temp_1.FindFirstChildOfClass(temp_1, "BasePart")
            branch_result = temp_5
            u = temp_5
        end
        if (not branch_result) then
            do
                local temp_1
                temp_1 = l.value
                u = temp_1.FindFirstChild(temp_1, "Blade")
            end
        end
        I = u
    end
    do
        local temp_1, temp_10, temp_11, temp_15, temp_16, temp_20, temp_21, temp_26, temp_27, temp_28, temp_5, temp_6
        temp_1 = X.value
        temp_5 = temp_1.FindFirstChild(temp_1, "HumanoidRootPart")
        temp_6 = X.value
        temp_10 = temp_6.FindFirstChild(temp_6, "Head")
        temp_11 = X.value
        temp_15 = temp_11.FindFirstChild(temp_11, "Torso")
        temp_16 = X.value
        temp_20 = temp_16.FindFirstChild(temp_16, "UpperTorso")
        temp_21 = X.value
        temp_26 = {temp_5, temp_10, temp_15, temp_20, unpack_values({temp_21.FindFirstChild(temp_21, "LowerTorso")})}
        temp_27 = {}
        temp_27.value = temp_26
        temp_28 = captures[4].value
        branch_result = temp_28
        I, o, u = temp_28, temp_27, I
    end
    if branch_result then
        I = u
    end
    branch_result = I
    if branch_result then
        do
            local temp_2
            temp_2 = {ipairs(o.value)}
            a, g, q = temp_2[1], temp_2[2], temp_2[3]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = a(g, q)
                branch_result = temp_1
                A, q = temp_2, temp_1
            end
            if not branch_result then break end
            branch_result = A
            z = A
            if branch_result then
                z = A.IsA(A, "BasePart")
            end
            branch_result = z
            if branch_result then
                captures[4].value(u, A, 0)
                captures[4].value(u, A, 1)
            end
        end
    end
    do
        local temp_1
        temp_1 = {}
        task.spawn(bind(callbacks.callback_39, {l, captures[2], captures[3], o, captures[5], X}))
        return unpack_values(temp_1)
    end
end

-- callback_160; bloques originales: 16
callbacks.callback_160 = function(captures, arguments)
    local B, I, X, a, branch_result, g, o, u
    local e7 = {}
    do
        local temp_1, temp_2
        temp_1 = arguments[1]
        temp_2 = (not temp_1)
        branch_result = temp_2
        I, X = temp_2, temp_1
    end
    if (not branch_result) then
        I = (not X.IsA(X, "Tool"))
    end
    branch_result = I
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_5
        temp_5 = X.FindFirstChild(X, "ThrowingKinfeHandlerScript", true)
        branch_result = temp_5
        I = temp_5
    end
    if (not branch_result) then
        do
            local temp_5
            temp_5 = X.FindFirstChild(X, "KnifeClient", true)
            branch_result = temp_5
            B = temp_5
        end
        if (not branch_result) then
            B = X.FindFirstChild(X, "KnifeServer", true)
        end
        I = B
    end
    branch_result = I
    if branch_result then
        return unpack_values({true})
    end
    do
        local temp_21, temp_7
        temp_7 = string.lower(X.Name)
        temp_21 = {ipairs({"knife", "cuchillo", "blade", "sword", "dagger", "kunai"})}
        B, g, o, u = temp_7, temp_21[1], temp_21[3], temp_21[2]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = g(u, o)
            branch_result = temp_1
            a, o = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({false})
        end
        branch_result = string.find(B, a)
        if not (not branch_result) then break end
    
    end
    return unpack_values({true})
end

-- callback_161; bloques originales: 5
callbacks.callback_161 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = temp_4
        I, X = temp_4, temp_4
    end
    if branch_result then
        I = X.FindFirstChild(X, "HumanoidRootPart")
    end
    branch_result = (not I)
    B = I
    if branch_result then
        return unpack_values({nil})
    end
    return unpack_values({unpack_values({captures[4].value(B)})})
end

-- callback_162; bloques originales: 6
callbacks.callback_162 = function(captures, arguments)
    local B, X, branch_result, g, l, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_5
        temp_1 = {}
        temp_2 = captures[1].value
        temp_5 = {ipairs(unpack_values({temp_2.GetPlayers(temp_2)}))}
        B, X, l, u = temp_5[2], temp_1, temp_5[3], temp_5[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = u(B, l)
            branch_result = temp_1
            g, l = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({X})
        end
        branch_result = captures[2].value(g)
        if branch_result then
            table.insert(X, g)
        end
    end
end

-- callback_163; bloques originales: 9
callbacks.callback_163 = function(captures, arguments)
    local B, I, branch_result, l
    local e7 = {}
    do
        local temp_4, temp_5
        temp_4 = arguments[1].Character
        temp_5 = (not temp_4)
        branch_result = temp_5
        B, I = temp_4, temp_5
    end
    if (not branch_result) then
        I = B.FindFirstChildOfClass(B, "ForceField")
    end
    branch_result = I
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_4
        temp_4 = B.FindFirstChildOfClass(B, "Humanoid")
        branch_result = (not temp_4)
        l = temp_4
    end
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_4
        temp_4 = (l.Health > 0.1)
        branch_result = temp_4
        I = temp_4
    end
    if branch_result then
        I = (l.GetState(l) ~= Enum.HumanoidStateType.Dead)
    end
    return unpack_values({I})
end

-- callback_164; bloques originales: 7
callbacks.callback_164 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    do
        local temp_4
        temp_4 = captures[1].value.Character
        branch_result = (not temp_4)
        X = temp_4
    end
    if branch_result then
        return unpack_values({false})
    end
    do
        local temp_4, temp_5
        temp_4 = X.FindFirstChildOfClass(X, "Tool")
        temp_5 = (not temp_4)
        branch_result = temp_5
        B, I = temp_4, temp_5
    end
    if (not branch_result) then
        I = captures[4].value(B)
    end
    branch_result = I
    if branch_result then
        return unpack_values({false})
    end
    return unpack_values({unpack_values({captures[5].value(B)})})
end

-- callback_165; bloques originales: 20
callbacks.callback_165 = function(captures, arguments)
    local B, I, J, X, a, branch_result, g, l, o, u
    local e7 = {}
    local steps = {}
    steps.entry = function()
        branch_result = captures[1].value()
        if branch_result then
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_4
            temp_4 = captures[2].value.Character
            branch_result = temp_4
            I, X = temp_4, temp_4
        end
        if branch_result then
            I = X.FindFirstChildOfClass(X, "Humanoid")
        end
        do
            local temp_1
            temp_1 = (not X)
            branch_result = temp_1
            B, I = I, temp_1
        end
        if (not branch_result) then
            do
                local temp_1
                temp_1 = (not B)
                branch_result = temp_1
                l = temp_1
            end
            if (not branch_result) then
                l = captures[5].value()
            end
            I = l
        end
        branch_result = I
        if branch_result then
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_1, temp_5
            temp_1 = captures[2].value
            temp_5 = temp_1.FindFirstChild(temp_1, "Backpack")
            branch_result = temp_5
            l = temp_5
        end
        if branch_result then
            return "step_2"
        else
            return "step_7"
        end
    end
    steps.step_2 = function()
        do
            local temp_3
            temp_3 = {ipairs(unpack_values({l.GetChildren(l)}))}
            g, o, u = temp_3[1], temp_3[3], temp_3[2]
        end
        return "step_3"
    end
    steps.step_3 = function()
        do
            local temp_1, temp_2
            temp_1, temp_2 = g(u, o)
            branch_result = temp_1
            a, o = temp_2, temp_1
        end
        if branch_result then
            return "step_4"
        else
            return "step_6"
        end
    end
    steps.step_4 = function()
        do
            local temp_4
            temp_4 = a.IsA(a, "Tool")
            branch_result = temp_4
            J = temp_4
        end
        if branch_result then
            J = captures[6].value(a)
        end
        branch_result = J
        if branch_result then
            return "step_5"
        else
            return "step_8"
        end
    end
    steps.step_5 = function()
        B.EquipTool(B, a)
        return "step_6"
    end
    steps.step_6 = function()

        return "step_7"
    end
    steps.step_7 = function()
        return nil, pack_values(unpack_values({}))
    end
    steps.step_8 = function()

        return "step_3"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_166; bloques originales: 18
callbacks.callback_166 = function(captures, arguments)
    local A, B, J, K, X, a, branch_result, g, o, u, z
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = {}
        temp_3 = captures[1].value()
        branch_result = (not temp_3)
        B, X = temp_3, temp_1
    end
    if branch_result then
        return unpack_values({X})
    end
    do
        local temp_3
        temp_3 = {ipairs(captures[2].value())}
        g, o, u = temp_3[1], temp_3[3], temp_3[2]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = g(u, o)
            branch_result = temp_1
            a, o = temp_2, temp_1
        end
        if (not branch_result) then
            do
                local temp_1
                temp_1 = {X}
                table.sort(X, bind(callbacks.callback_192, {captures[4], captures[5]}))
                return unpack_values(temp_1)
            end
        end
        branch_result = captures[3].value(a)
        if branch_result then
            do
                local temp_3
                temp_3 = a.Character
                branch_result = temp_3
                J = temp_3
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = J.FindFirstChild(J, "HumanoidRootPart")
                    branch_result = temp_4
                    A, z = temp_4, temp_4
                end
                if branch_result then
                    z = (A.Position.Y >= -500)
                end
                branch_result = z
                if branch_result then
                    do
                        local temp_2
                        temp_2 = captures[6].value(A)
                        branch_result = temp_2
                        z = temp_2
                    end
                    if branch_result then
                        do
                            local temp_4
                            temp_4 = (z - B).Magnitude
                            branch_result = (temp_4 <= captures[7].value)
                            K = temp_4
                        end
                        if branch_result then
                            table.insert(X, {["plr"] = a, ["hrp"] = A, ["posReal"] = z, ["dist"] = K})
                        end
                    end
                end
            end
        end
    end
end

-- callback_167; bloques originales: 22
callbacks.callback_167 = function(captures, arguments)
    local B, I, J, X, a, branch_result, l, o, q, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_4, temp_6
        temp_1 = arguments[1]
        temp_2 = captures[1].value
        temp_4 = arguments[2]
        temp_6 = temp_2.Character
        branch_result = temp_6
        B, I, X, l = temp_4, temp_6, temp_1, temp_6
    end
    if branch_result then
        I = l.FindFirstChild(l, "HumanoidRootPart")
    end
    do
        local temp_1
        temp_1 = (not I)
        branch_result = temp_1
        I, u = temp_1, I
    end
    if (not branch_result) then
        do
            local temp_1
            temp_1 = (not X)
            branch_result = temp_1
            o = temp_1
        end
        if (not branch_result) then
            o = (not B)
        end
        I = o
    end
    branch_result = I
    if branch_result then
        return unpack_values({})
    end
    do
        local temp_10, temp_15, temp_17, temp_3
        temp_3 = X.Position
        temp_10 = (temp_3 - u.Position).Magnitude
        temp_15 = (temp_3 - Vector3.new(0, 4.5, 0))
        temp_17 = (temp_10 <= captures[4].value)
        branch_result = temp_17
        I, a, o, q = temp_17, temp_15, temp_3, temp_10
    end
    if branch_result then
        do
            local temp_4
            temp_4 = captures[5].value.KillAuraEnabled
            branch_result = temp_4
            J = temp_4
        end
        if branch_result then
            J = captures[5].value.ScriptActive
        end
        I = J
    end
    branch_result = I
    if branch_result then
        branch_result = (q > 20)
        if branch_result then
            captures[6].value(unpack_values({CFrame.new(a, o)}))
        else
            u.CFrame = CFrame.new(a, o)
            u.AssemblyLinearVelocity = Vector3.zero
        end
    end
    branch_result = B
    I = B
    if branch_result then
        do
            local temp_1, temp_2
            temp_1 = captures[7].value
            temp_2 = captures[8].value
            I = temp_1(unpack_values({temp_2.GetPlayerFromCharacter(temp_2, B)}))
        end
    end
    branch_result = I
    if branch_result then
        captures[9].value(B)
    end
    return unpack_values({})
end

-- callback_168; bloques originales: 31
callbacks.callback_168 = function(captures, arguments)
    local B, I, J, X, a, branch_result, g, l, o, u
    local e7 = {}
    local steps = {}
    steps.entry = function()
        do
            local temp_1
            temp_1 = captures[1].value
            branch_result = temp_1
            I = temp_1
        end
        if (not branch_result) then
            I = (not captures[2].value.ScriptActive)
        end
        branch_result = I
        if branch_result then
            return nil, pack_values(unpack_values({}))
        end
        captures[1].value = true
        return "step_2"
    end
    steps.step_2 = function()
        do
            local temp_4
            temp_4 = captures[2].value.KillAuraEnabled
            branch_result = temp_4
            I = temp_4
        end
        if branch_result then
            I = captures[2].value.ScriptActive
        end
        branch_result = I
        if branch_result then
            return "step_3"
        else
            return "step_5"
        end
    end
    steps.step_3 = function()
        do
            local temp_4
            temp_4 = captures[5].value.Character
            branch_result = temp_4
            I, X = temp_4, temp_4
        end
        if branch_result then
            I = X.FindFirstChildOfClass(X, "Tool")
        end
        branch_result = I
        B, I = I, I
        if branch_result then
            I = captures[6].value(B)
        end
        branch_result = I
        if branch_result then
            return "step_4"
        else
            return "step_6"
        end
    end
    steps.step_4 = function()

        return "step_5"
    end
    steps.step_5 = function()
        captures[1].value = false
        return nil, pack_values(unpack_values({}))
    end
    steps.step_6 = function()
        do
            local temp_2
            temp_2 = captures[7].value()
            branch_result = ((# temp_2) == 0)
            l = temp_2
        end
        if branch_result then
            return "step_7"
        else
            return "step_8"
        end
    end
    steps.step_7 = function()

        return "step_5"
    end
    steps.step_8 = function()
        do
            local temp_3
            temp_3 = (not captures[8].value())
            branch_result = temp_3
            I = temp_3
        end
        if branch_result then
            I = captures[2].value.AutoEquipKnifeEnabled
        end
        branch_result = I
        if branch_result then
            captures[9].value()
            task.wait(0.02)
        end
        branch_result = (not captures[8].value())
        if branch_result then
            return "step_9"
        else
            return "step_10"
        end
    end
    steps.step_9 = function()

        return "step_5"
    end
    steps.step_10 = function()
        do
            local temp_1
            temp_1 = {ipairs(l)}
            g, o, u = temp_1[3], temp_1[2], temp_1[1]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = u(o, g)
                branch_result = temp_1
                a, g = temp_2, temp_1
            end
            if not branch_result then break end
            do
                local temp_11, temp_6
                temp_6 = a.plr.Character
                temp_11 = captures[10].value(a.plr)
                branch_result = temp_11
                I, J = temp_11, temp_6
            end
            if branch_result then
                I = J
            end
            branch_result = I
            if branch_result then
                captures[11].value(a.hrp, J)
            end
        end
        task.wait(captures[12].value)
        return "step_2"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_169; bloques originales: 22
callbacks.callback_169 = function(captures, arguments)
    local B, I, X, branch_result
    local e7 = {}
    while true do
        branch_result = captures[1].value.ScriptActive
        if (not branch_result) then
            return unpack_values({})
        end
        do
            local temp_10, temp_4
            temp_4 = captures[4].value.Heartbeat
            temp_4.Wait(temp_4)
            temp_10 = captures[1].value.KillAuraEnabled
            branch_result = temp_10
            I = temp_10
        end
        if branch_result then
            I = (not captures[5].value)
        end
        branch_result = I
        if branch_result then
            do
                local temp_4
                temp_4 = captures[6].value.Character
                branch_result = temp_4
                I, X = temp_4, temp_4
            end
            if branch_result then
                I = X.FindFirstChildOfClass(X, "Tool")
            end
            branch_result = I
            B, I = I, I
            if branch_result then
                I = captures[7].value(B)
            end
            branch_result = (not I)
            if branch_result then
                branch_result = ((# captures[8].value()) > 0)
                if branch_result then
                    do
                        local temp_3
                        temp_3 = (not captures[9].value())
                        branch_result = temp_3
                        I = temp_3
                    end
                    if branch_result then
                        I = captures[1].value.AutoEquipKnifeEnabled
                    end
                    branch_result = I
                    if branch_result then
                        captures[10].value()
                    end
                    branch_result = captures[9].value()
                    if branch_result then
                        task.spawn(captures[11].value)
                    end
                end
            end
        end
    end
end

-- callback_170; bloques originales: 11
callbacks.callback_170 = function(captures, arguments)
    local A, B, J, K, X, a, branch_result, g, l, n, o, q, u, z
    local e7 = {}
    do
        local temp_1, temp_10, temp_11, temp_2, temp_26, temp_3, temp_4
        temp_1 = {}
        temp_2 = arguments[3]
        temp_1.value = arguments[4]
        temp_3 = arguments[1]
        temp_4 = arguments[2]
        temp_10 = Instance.new("TextButton")
        temp_11 = {}
        temp_11.value = temp_10
        temp_11.value.Size = UDim2.new(0, 50, 0, 28)
        temp_11.value.Position = UDim2.new(1, -62, 0.5, -14)
        temp_26 = temp_11.value
        branch_result = temp_2
        B, J, X, a, l, o, q, u = temp_4, temp_26, temp_3, temp_2, temp_2, temp_11, temp_26, temp_1
    end
    if branch_result then
        a = captures[3].value.PanelColor
    end
    branch_result = a
    g = a
    if (not branch_result) then
        g = Color3.fromRGB(50, 50, 55)
    end
    do
        local temp_25, temp_40, temp_65, temp_66, temp_74
        q.BackgroundColor3 = g
        o.value.Text = ""
        o.value.Active = true
        o.value.ZIndex = 5
        o.value.AutoButtonColor = false
        o.value.Parent = X
        temp_25 = Instance.new("UICorner")
        temp_25.CornerRadius = UDim.new(1, 0)
        temp_25.Parent = o.value
        temp_40 = Instance.new("UIStroke")
        temp_40.Thickness = 1.5
        temp_40.Color = Color3.fromRGB(60, 60, 68)
        temp_40.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
        temp_40.Parent = o.value
        temp_65 = Instance.new("Frame")
        temp_66 = {}
        temp_66.value = temp_65
        temp_66.value.Size = UDim2.new(0, 22, 0, 22)
        temp_74 = temp_66.value
        branch_result = l
        A, K, a, z = temp_74, temp_74, temp_66, l
    end
    if branch_result then
        z = UDim2.new(1, -25, 0.5, -11)
    end
    branch_result = z
    J = z
    if (not branch_result) then
        J = UDim2.new(0, 3, 0.5, -11)
    end
    do
        local temp_27, temp_42, temp_55, temp_56, temp_57, temp_58, temp_59, temp_63, temp_64, temp_65, temp_69, temp_73
        A.Position = J
        a.value.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        a.value.BorderSizePixel = 0
        a.value.Active = false
        a.value.ZIndex = 6
        a.value.Parent = o.value
        temp_27 = Instance.new("UICorner")
        temp_27.CornerRadius = UDim.new(1, 0)
        temp_27.Parent = a.value
        temp_42 = Instance.new("UIStroke")
        temp_42.Thickness = 1
        temp_42.Color = Color3.fromRGB(0, 0, 0)
        temp_42.Transparency = 0.8
        temp_55 = a.value
        temp_56 = {}
        temp_42.Parent = temp_55
        temp_57 = {}
        temp_58 = bind(callbacks.callback_17, {temp_56, captures[1], captures[2], captures[3], captures[4], a, o})
        temp_56.value = l
        temp_59 = {}
        temp_57.value = temp_58
        temp_59.value = false
        temp_63 = bind(callbacks.callback_18, {temp_59, temp_56, temp_57, u, captures[1], captures[2], captures[5]})
        temp_64 = table.insert
        temp_65 = captures[6].value
        temp_69 = o.value.Activated
        temp_64(temp_65, unpack_values({temp_69.Connect(temp_69, temp_63)}))
        temp_73 = bind(callbacks.callback_19, {temp_56, temp_57})
        branch_result = B
        K, n, z = temp_57, temp_73, temp_56
    end
    if branch_result then
        captures[7].value[B] = n
    end
    table.insert(captures[8].value, {["Bg"] = o.value, ["GetState"] = bind(callbacks.callback_37, {z}), ["Update"] = K.value})
    return unpack_values({n})
end

-- callback_171; bloques originales: 1
callbacks.callback_171 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_104, temp_105, temp_106, temp_109, temp_112, temp_113, temp_116, temp_119,
            temp_12, temp_122, temp_125, temp_128, temp_13, temp_133, temp_134, temp_137, temp_140, temp_143,
            temp_148, temp_149, temp_154, temp_155, temp_160, temp_161, temp_168, temp_171, temp_174,
            temp_179, temp_180, temp_185, temp_188, temp_195, temp_196, temp_2, temp_203, temp_206, temp_207,
            temp_208, temp_213, temp_214, temp_215, temp_220, temp_221, temp_222, temp_225, temp_228,
            temp_229, temp_234, temp_235, temp_236, temp_241, temp_244, temp_245, temp_248, temp_251,
            temp_255, temp_258, temp_260, temp_261, temp_262, temp_265, temp_266, temp_267, temp_270,
            temp_271, temp_272, temp_273, temp_277, temp_278, temp_279, temp_282, temp_283, temp_284,
            temp_285, temp_289, temp_290, temp_291, temp_294, temp_295, temp_296, temp_297, temp_3, temp_301,
            temp_302, temp_303, temp_306, temp_307, temp_308, temp_309, temp_313, temp_314, temp_317,
            temp_318, temp_320, temp_4, temp_5, temp_55, temp_6, temp_70, temp_87, temp_88, temp_89, temp_94
        temp_1 = arguments[1]
        temp_2 = {}
        temp_3 = {}
        temp_4 = {}
        temp_4.value = arguments[2]
        temp_5 = {}
        temp_6 = arguments[5]
        temp_5.value = arguments[3]
        temp_2.value = arguments[4]
        temp_3.value = arguments[6]
        temp_12 = Instance.new("TextButton")
        temp_13 = {}
        temp_13.value = temp_12
        temp_13.value.Size = UDim2.new(0, 100, 0, 8)
        temp_13.value.Position = UDim2.new(1, -145, 0.5, -4)
        temp_13.value.BackgroundColor3 = Color3.fromRGB(35, 35, 40)
        temp_13.value.AutoButtonColor = false
        temp_13.value.Text = ""
        temp_13.value.ZIndex = 5
        temp_13.value.Parent = temp_1
        temp_55 = Instance.new("UICorner")
        temp_55.CornerRadius = UDim.new(1, 0)
        temp_55.Parent = temp_13.value
        temp_70 = Instance.new("UIStroke")
        temp_70.Thickness = 1
        temp_70.Color = Color3.fromRGB(45, 45, 50)
        temp_70.Parent = temp_13.value
        temp_87 = Instance.new("Frame")
        temp_88 = {}
        temp_88.value = temp_87
        temp_89 = temp_88.value
        temp_94 = UDim2.new
        temp_104 = math.clamp(((temp_6 - temp_5.value) / (temp_2.value - temp_5.value)), 0, 1)
        temp_105 = temp_94(temp_104, 0, 1, 0)
        temp_89.Size = temp_105
        temp_106 = temp_88.value
        temp_109 = captures[3].value
        temp_112 = temp_109.PanelColor
        temp_106.BackgroundColor3 = temp_112
        temp_113 = temp_88.value
        temp_113.BorderSizePixel = 0
        temp_116 = temp_88.value
        temp_116.ZIndex = 6
        temp_119 = temp_88.value
        temp_122 = temp_13.value
        temp_119.Parent = temp_122
        temp_125 = Instance.new
        temp_128 = temp_125("UICorner")
        temp_133 = UDim.new
        temp_134 = temp_133(1, 0)
        temp_128.CornerRadius = temp_134
        temp_137 = temp_88.value
        temp_128.Parent = temp_137
        temp_140 = Instance.new
        temp_143 = temp_140("Frame")
        temp_148 = UDim2.new
        temp_149 = temp_148(0, 14, 0, 14)
        temp_143.Size = temp_149
        temp_154 = UDim2.new
        temp_155 = temp_154(1, -7, 0.5, -7)
        temp_143.Position = temp_155
        temp_160 = Color3.fromRGB
        temp_161 = temp_160(255, 255, 255)
        temp_143.BackgroundColor3 = temp_161
        temp_143.BorderSizePixel = 0
        temp_143.ZIndex = 7
        temp_168 = temp_88.value
        temp_143.Parent = temp_168
        temp_171 = Instance.new
        temp_174 = temp_171("UICorner")
        temp_179 = UDim.new
        temp_180 = temp_179(1, 0)
        temp_174.CornerRadius = temp_180
        temp_174.Parent = temp_143
        temp_185 = Instance.new
        temp_188 = temp_185("UIStroke")
        temp_188.Thickness = 1
        temp_195 = Color3.fromRGB
        temp_196 = temp_195(0, 0, 0)
        temp_188.Color = temp_196
        temp_188.Transparency = 0.5
        temp_188.Parent = temp_143
        temp_203 = Instance.new
        temp_206 = temp_203("TextBox")
        temp_207 = {}
        temp_207.value = temp_206
        temp_208 = temp_207.value
        temp_213 = UDim2.new
        temp_214 = temp_213(0, 35, 0, 20)
        temp_208.Size = temp_214
        temp_215 = temp_207.value
        temp_220 = UDim2.new
        temp_221 = temp_220(1, 10, 0.5, -10)
        temp_215.Position = temp_221
        temp_222 = temp_207.value
        temp_222.BackgroundTransparency = 1
        temp_225 = temp_207.value
        temp_228 = tostring(temp_6)
        temp_225.Text = temp_228
        temp_229 = temp_207.value
        temp_234 = Color3.fromRGB
        temp_235 = temp_234(255, 200, 0)
        temp_229.TextColor3 = temp_235
        temp_236 = temp_207.value
        temp_241 = Enum.Font
        temp_244 = temp_241.GothamBold
        temp_236.Font = temp_244
        temp_245 = temp_207.value
        temp_245.TextSize = 12
        temp_248 = temp_207.value
        temp_248.ZIndex = 7
        temp_251 = temp_207.value
        temp_251.ClearTextOnFocus = false
        temp_255 = temp_207.value
        temp_258 = temp_13.value
        temp_255.Parent = temp_258
        temp_260 = {}
        temp_261 = {}
        temp_261.value = false
        temp_262 = bind(callbacks.callback_3, {captures[1], captures[2], temp_13, temp_88, temp_5, temp_2, temp_207, captures[3], temp_4, temp_3})
        temp_260.value = temp_262
        temp_265 = table.insert
        temp_266 = captures[4].value
        temp_267 = temp_13.value
        temp_270 = temp_267.InputBegan
        temp_271 = bind(callbacks.callback_4, {captures[1], captures[2], temp_261, temp_260})
        temp_272 = temp_270.Connect
        temp_273 = {temp_272(temp_270, temp_271)}
        temp_265(temp_266, unpack_values(temp_273))
        temp_277 = table.insert
        temp_278 = captures[4].value
        temp_279 = captures[5].value
        temp_282 = temp_279.InputChanged
        temp_283 = bind(callbacks.callback_5, {temp_261, captures[1], captures[2], temp_260})
        temp_284 = temp_282.Connect
        temp_285 = {temp_284(temp_282, temp_283)}
        temp_277(temp_278, unpack_values(temp_285))
        temp_289 = table.insert
        temp_290 = captures[4].value
        temp_291 = captures[5].value
        temp_294 = temp_291.InputEnded
        temp_295 = temp_294.Connect
        temp_296 = bind(callbacks.callback_6, {captures[1], captures[2], temp_261, captures[6]})
        temp_297 = {temp_295(temp_294, temp_296)}
        temp_289(temp_290, unpack_values(temp_297))
        temp_301 = table.insert
        temp_302 = captures[4].value
        temp_303 = temp_207.value
        temp_306 = temp_303.FocusLost
        temp_307 = bind(callbacks.callback_7, {temp_207, captures[1], captures[2], temp_5, temp_2, captures[3], temp_4, temp_88, temp_3, captures[6]})
        temp_308 = temp_306.Connect
        temp_309 = {temp_308(temp_306, temp_307)}
        temp_301(temp_302, unpack_values(temp_309))
        temp_313 = table.insert
        temp_314 = captures[7].value
        temp_317 = bind(callbacks.callback_8, {temp_88, captures[1], captures[2], captures[3]})
        temp_318 = {["Update"] = temp_317}
        temp_313(temp_314, temp_318)
        temp_320 = {}
        return unpack_values(temp_320)
    end
end

-- callback_172; bloques originales: 10
callbacks.callback_172 = function(captures, arguments)
    local B, I, branch_result, l, u
    local e7 = {}
    do
        local temp_4, temp_8
        temp_4 = game.GetService(game, "ReplicatedStorage")
        temp_8 = temp_4.WaitForChild(temp_4, "Packages", 3)
        branch_result = temp_8
        B, I = temp_8, temp_8
    end
    if branch_result then
        I = B.WaitForChild(B, "Networking", 3)
    end
    do
        local temp_1, temp_2
        temp_1 = {}
        temp_1.value = I
        temp_2 = temp_1.value
        branch_result = temp_2
        I, l = temp_2, temp_1
    end
    if branch_result then
        do
            local temp_1
            temp_1 = l.value
            I = temp_1.FindFirstChild(temp_1, "RE/Events/CollectEventSpawnable")
        end
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = I
        u = temp_1
    end
    while true do
        branch_result = captures[3].value.ScriptActive
        if (not branch_result) then
            return unpack_values({})
        end
        branch_result = captures[3].value.AutoFarmEnabled
        if branch_result then
            pcall(bind(callbacks.callback_14, {u, l, captures[1], captures[2]}))
        end
        task.wait(0.05)
    end
end

-- callback_173; bloques originales: 3
callbacks.callback_173 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = arguments[1]
        branch_result = (not captures[1].value[temp_1])
        X = temp_1
    end
    if branch_result then
        do
            local temp_1, temp_107, temp_17, temp_30, temp_49, temp_61, temp_7, temp_80
            temp_1 = {}
            temp_7 = Instance.new("Frame")
            temp_7.BackgroundTransparency = 1
            temp_7.ZIndex = 1
            temp_17 = Instance.new("UIStroke")
            temp_17.Thickness = 1.5
            temp_17.Parent = temp_7
            temp_7.Parent = captures[4].value
            temp_30 = Instance.new("Frame")
            temp_30.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
            temp_30.BorderSizePixel = 0
            temp_30.ZIndex = 2
            temp_30.Parent = captures[4].value
            temp_49 = Instance.new("Frame")
            temp_49.BorderSizePixel = 0
            temp_49.ZIndex = 3
            temp_49.Parent = temp_30
            temp_61 = Instance.new("Frame")
            temp_61.BorderSizePixel = 0
            temp_61.AnchorPoint = Vector2.new(0.5, 0.5)
            temp_61.ZIndex = 0
            temp_61.Parent = captures[4].value
            temp_80 = Instance.new("Highlight")
            temp_80.Name = ("KaiserCham_" .. X.Name)
            temp_80.OutlineColor = Color3.fromRGB(255, 255, 255)
            temp_80.FillTransparency = 0.5
            temp_80.OutlineTransparency = 0
            temp_80.Parent = captures[4].value
            temp_107 = Instance.new("TextLabel")
            temp_107.BackgroundTransparency = 1
            temp_107.TextColor3 = Color3.fromRGB(255, 255, 255)
            temp_107.TextStrokeTransparency = 0
            temp_107.TextStrokeColor3 = Color3.fromRGB(0, 0, 0)
            temp_107.Font = Enum.Font.GothamBold
            temp_107.TextSize = 12
            temp_107.AnchorPoint = Vector2.new(0.5, 1)
            temp_107.ZIndex = 4
            temp_107.Parent = captures[4].value
            temp_1.Box = temp_7
            temp_1.NameText = temp_107
            temp_1.BoxStroke = temp_17
            temp_1.HealthBg = temp_30
            temp_1.HealthBar = temp_49
            temp_1.Line = temp_61
            temp_1.Cham = temp_80
            captures[1].value[X] = temp_1
        end
    end
    return unpack_values({captures[1].value[X]})
end

-- callback_174; bloques originales: 11
callbacks.callback_174 = function(captures, arguments)
    local A, B, I, a, branch_result, l, q, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_3, temp_50, temp_64, temp_80, temp_81, temp_9
        temp_1 = arguments[3]
        temp_2 = arguments[1]
        temp_3 = {}
        temp_3.value = arguments[2]
        temp_9 = Instance.new("TextButton")
        temp_9.Size = UDim2.new(0, 55, 0, 24)
        temp_9.Position = UDim2.new(1, -67, 0.5, -12)
        temp_9.BackgroundColor3 = Color3.fromRGB(35, 35, 40)
        temp_9.Text = ""
        temp_9.Active = true
        temp_9.ZIndex = 5
        temp_9.ClipsDescendants = false
        temp_9.AutoButtonColor = false
        temp_9.Parent = temp_2
        temp_50 = Instance.new("UICorner")
        temp_50.CornerRadius = UDim.new(0, 5)
        temp_50.Parent = temp_9
        temp_64 = Instance.new("UIStroke")
        temp_64.Thickness = 1.2
        temp_64.Color = Color3.fromRGB(45, 45, 50)
        temp_64.Parent = temp_9
        temp_80 = Instance.new("TextLabel")
        temp_81 = {}
        temp_81.value = temp_80
        temp_81.value.Size = UDim2.new(1, 0, 1, 0)
        temp_81.value.Position = UDim2.new(0, 0, 0, 0)
        temp_81.value.BackgroundTransparency = 1
        branch_result = temp_1
        B, I, l, q, u = temp_3, temp_1, temp_1, temp_81, temp_9
    end
    if (not branch_result) then
        do
            local temp_9
            temp_9 = (captures[3].value.Binds[B.value] ~= "")
            branch_result = temp_9
            A = temp_9
        end
        if branch_result then
            A = captures[3].value.Binds[B.value]
        end
        branch_result = A
        a = A
        if (not branch_result) then
            a = "NONE"
        end
        I = a
    end
    do
        local temp_51
        q.value.Text = I
        q.value.TextColor3 = Color3.fromRGB(255, 200, 0)
        q.value.Font = Enum.Font.GothamBold
        q.value.TextSize = 11
        q.value.TextXAlignment = Enum.TextXAlignment.Center
        q.value.TextYAlignment = Enum.TextYAlignment.Center
        q.value.ZIndex = 6
        q.value.Active = false
        q.value.Parent = u
        temp_51 = (not l)
        branch_result = temp_51
        I = temp_51
    end
    if branch_result then
        I = B.value
    end
    branch_result = I
    if branch_result then
        do
            local temp_12, temp_13, temp_4, temp_8, temp_9
            captures[4].value[B.value] = q.value
            temp_4 = {}
            temp_4.value = false
            temp_8 = table.insert
            temp_9 = captures[5].value
            temp_12 = bind(callbacks.callback_13, {temp_4, q, captures[1], captures[2], captures[6], captures[3], B, captures[7], captures[8]})
            temp_13 = u.Activated
            temp_8(temp_9, unpack_values({temp_13.Connect(temp_13, temp_12)}))
        end
    end
    return unpack_values({q.value})
end

-- callback_175; bloques originales: 3
callbacks.callback_175 = function(captures, arguments)
    local branch_result, l, u
    local e7 = {}
    do
        local temp_1, temp_2, temp_3, temp_33, temp_47, temp_65, temp_9
        temp_1 = arguments[1]
        temp_2 = arguments[2]
        temp_3 = arguments[3]
        temp_9 = Instance.new("Frame")
        temp_9.Size = UDim2.new(1, 0, 0, ((temp_3 and 42) or 36))
        temp_9.BackgroundColor3 = Color3.fromRGB(20, 22, 28)
        temp_9.BackgroundTransparency = 0.45
        temp_9.Parent = temp_1
        temp_33 = Instance.new("UICorner")
        temp_33.CornerRadius = UDim.new(0, 8)
        temp_33.Parent = temp_9
        temp_47 = Instance.new("UIStroke")
        temp_47.Thickness = 1.2
        temp_47.Color = Color3.fromRGB(60, 65, 75)
        temp_47.Transparency = 0.2
        temp_47.Parent = temp_9
        temp_65 = Instance.new("TextLabel")
        temp_65.Text = temp_2
        temp_65.TextColor3 = Color3.fromRGB(255, 255, 255)
        temp_65.TextSize = 13
        temp_65.Font = Enum.Font.GothamBold
        temp_65.TextXAlignment = Enum.TextXAlignment.Left
        temp_65.Position = UDim2.new(0, 12, 0, ((temp_3 and 4) or 0))
        temp_65.Size = UDim2.new(0.6, 0, 0, ((temp_3 and 18) or 36))
        temp_65.BackgroundTransparency = 1
        temp_65.Parent = temp_9
        branch_result = temp_3
        l, u = temp_3, temp_9
    end
    if branch_result then
        do
            local temp_6
            temp_6 = Instance.new("TextLabel")
            temp_6.Text = l
            temp_6.TextColor3 = Color3.fromRGB(200, 205, 220)
            temp_6.TextSize = 11
            temp_6.Font = Enum.Font.GothamMedium
            temp_6.TextXAlignment = Enum.TextXAlignment.Left
            temp_6.Position = UDim2.new(0, 12, 0, 22)
            temp_6.Size = UDim2.new(0.6, 0, 0, 14)
            temp_6.BackgroundTransparency = 1
            temp_6.Parent = u
        end
    end
    return unpack_values({u})
end

-- callback_176; bloques originales: 1
callbacks.callback_176 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_2, temp_36, temp_50, temp_7
        temp_2 = arguments[1]
        temp_7 = Instance.new("Frame")
        temp_7.Size = UDim2.new(0, 45, 0, 24)
        temp_7.Position = UDim2.new(1, -57, 0.5, -12)
        temp_7.BackgroundColor3 = captures[3].value.FOVColor
        temp_7.Active = false
        temp_7.Parent = temp_2
        temp_36 = Instance.new("UICorner")
        temp_36.CornerRadius = UDim.new(0, 5)
        temp_36.Parent = temp_7
        temp_50 = Instance.new("UIStroke")
        temp_50.Thickness = 1.2
        temp_50.Color = Color3.fromRGB(55, 55, 62)
        temp_50.Parent = temp_7
        return unpack_values({temp_7})
    end
end

-- callback_177; bloques originales: 1
callbacks.callback_177 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_1, temp_100, temp_106, temp_113, temp_114, temp_117, temp_118, temp_119, temp_120,
            temp_124, temp_127, temp_132, temp_133, temp_138, temp_139, temp_144, temp_145, temp_154,
            temp_157, temp_162, temp_163, temp_168, temp_169, temp_178, temp_181, temp_186, temp_189,
            temp_194, temp_195, temp_2, temp_200, temp_201, temp_208, temp_211, temp_216, temp_217, temp_222,
            temp_223, temp_228, temp_229, temp_236, temp_30, temp_44, temp_64, temp_8
        temp_1 = arguments[2]
        temp_2 = arguments[1]
        temp_8 = Instance.new("Frame")
        temp_8.Size = UDim2.new(1, 0, 0, 28)
        temp_8.BackgroundColor3 = Color3.fromRGB(5, 5, 8)
        temp_8.BackgroundTransparency = 0.75
        temp_8.Parent = temp_2
        temp_30 = Instance.new("UICorner")
        temp_30.CornerRadius = UDim.new(0, 6)
        temp_30.Parent = temp_8
        temp_44 = Instance.new("UIStroke")
        temp_44.Thickness = 1.5
        temp_44.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
        temp_44.Transparency = 0.3
        temp_44.Parent = temp_8
        temp_64 = Instance.new("UIGradient")
        temp_64.Color = ColorSequence.new({ColorSequenceKeypoint.new(0, unpack_values({Color3.fromRGB(255, 0, 60)})), ColorSequenceKeypoint.new(0.5, unpack_values({Color3.fromRGB(40, 0, 10)})), unpack_values({ColorSequenceKeypoint.new(1, unpack_values({Color3.fromRGB(255, 0, 60)}))})})
        temp_64.Parent = temp_44
        temp_100 = TweenInfo.new
        temp_106 = Enum.EasingStyle.Linear
        temp_113 = temp_100(2.5, temp_106, Enum.EasingDirection.InOut, -1)
        temp_114 = captures[3].value
        temp_117 = {["Rotation"] = 360}
        temp_118 = temp_114.Create
        temp_119 = temp_118(temp_114, temp_64, temp_113, temp_117)
        temp_120 = temp_119.Play
        temp_120(temp_119)
        temp_124 = Instance.new
        temp_127 = temp_124("Frame")
        temp_132 = UDim2.new
        temp_133 = temp_132(0.25, 0, 0, 1)
        temp_127.Size = temp_133
        temp_138 = UDim2.new
        temp_139 = temp_138(0.05, 0, 0.5, 0)
        temp_127.Position = temp_139
        temp_144 = Color3.fromRGB
        temp_145 = temp_144(255, 255, 255)
        temp_127.BackgroundColor3 = temp_145
        temp_127.BackgroundTransparency = 0.5
        temp_127.BorderSizePixel = 0
        temp_127.Parent = temp_8
        temp_154 = Instance.new
        temp_157 = temp_154("TextLabel")
        temp_162 = string.upper
        temp_163 = temp_162(temp_1)
        temp_157.Text = temp_163
        temp_168 = Color3.fromRGB
        temp_169 = temp_168(255, 255, 255)
        temp_157.TextColor3 = temp_169
        temp_157.TextTransparency = 0.1
        temp_157.TextSize = 12
        temp_178 = Enum.Font
        temp_181 = temp_178.FredokaOne
        temp_157.Font = temp_181
        temp_186 = Enum.TextXAlignment
        temp_189 = temp_186.Center
        temp_157.TextXAlignment = temp_189
        temp_194 = UDim2.new
        temp_195 = temp_194(0.3, 0, 0, 0)
        temp_157.Position = temp_195
        temp_200 = UDim2.new
        temp_201 = temp_200(0.4, 0, 1, 0)
        temp_157.Size = temp_201
        temp_157.BackgroundTransparency = 1
        temp_157.Parent = temp_8
        temp_208 = Instance.new
        temp_211 = temp_208("Frame")
        temp_216 = UDim2.new
        temp_217 = temp_216(0.25, 0, 0, 1)
        temp_211.Size = temp_217
        temp_222 = UDim2.new
        temp_223 = temp_222(0.7, 0, 0.5, 0)
        temp_211.Position = temp_223
        temp_228 = Color3.fromRGB
        temp_229 = temp_228(255, 255, 255)
        temp_211.BackgroundColor3 = temp_229
        temp_211.BackgroundTransparency = 0.5
        temp_211.BorderSizePixel = 0
        temp_211.Parent = temp_8
        temp_236 = {temp_8}
        return unpack_values(temp_236)
    end
end

-- callback_178; bloques originales: 4
callbacks.callback_178 = function(captures, arguments)
    local A, J, K, a, branch_result, l, o, u
    local e7 = {}
    do
        local temp_1, temp_104, temp_105, temp_106, temp_107, temp_108, temp_11, temp_2, temp_3, temp_35, temp_5, temp_79
        temp_1 = arguments[2]
        temp_2 = arguments[1]
        temp_3 = {}
        temp_3.value = arguments[3]
        temp_5 = captures[1].value(temp_2, temp_1)
        temp_11 = Instance.new("Frame")
        temp_11.Size = UDim2.new(0, 195, 0, 24)
        temp_11.Position = UDim2.new(1, -205, 0.5, -12)
        temp_11.BackgroundTransparency = 1
        temp_11.ZIndex = 5
        temp_11.Parent = temp_5
        temp_35 = Instance.new("UIListLayout")
        temp_35.FillDirection = Enum.FillDirection.Horizontal
        temp_35.HorizontalAlignment = Enum.HorizontalAlignment.Right
        temp_35.VerticalAlignment = Enum.VerticalAlignment.Center
        temp_35.SortOrder = Enum.SortOrder.LayoutOrder
        temp_35.Padding = UDim.new(0, 5)
        temp_35.Parent = temp_11
        temp_79 = Color3.fromRGB(0, 0, 0)
        temp_104 = {temp_79, Color3.fromRGB(0, 255, 0), Color3.fromRGB(255, 0, 0), Color3.fromRGB(0, 85, 255), Color3.fromRGB(100, 255, 100), Color3.fromRGB(255, 255, 255), unpack_values({Color3.fromRGB(160, 32, 240)})}
        temp_105 = {ipairs(temp_104)}
        temp_106 = temp_105[1]
        temp_107 = temp_105[3]
        temp_108 = temp_105[2]
        A, J, a, l, o, u = temp_106, temp_107, temp_108, temp_3, temp_11, temp_5
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = A(a, J)
            branch_result = temp_1
            J, K = temp_1, temp_2
        end
        if not branch_result then break end
        do
            local temp_1, temp_36, temp_50, temp_63, temp_64, temp_67, temp_7
            temp_1 = {}
            temp_1.value = K
            temp_7 = Instance.new("TextButton")
            temp_7.Size = UDim2.new(0, 22, 0, 22)
            temp_7.BackgroundColor3 = temp_1.value
            temp_7.Text = ""
            temp_7.Active = true
            temp_7.ZIndex = 6
            temp_7.AutoButtonColor = false
            temp_7.Parent = o
            temp_36 = Instance.new("UICorner")
            temp_36.CornerRadius = UDim.new(0, 4)
            temp_36.Parent = temp_7
            temp_50 = Instance.new("UIStroke")
            temp_50.Thickness = 1
            temp_50.Color = Color3.fromRGB(45, 45, 52)
            temp_50.Parent = temp_7
            temp_63 = table.insert
            temp_64 = captures[4].value
            temp_67 = temp_7.Activated
            temp_63(temp_64, unpack_values({temp_67.Connect(temp_67, bind(callbacks.callback_98, {captures[5], l, temp_1, captures[6], captures[7], captures[2], captures[3]}))}))
        end
    end
    return unpack_values({u})
end

-- callback_179; bloques originales: 128
callbacks.callback_179 = function(captures, arguments)
    local A, B, D, G, I, J, K, M, Q, R, S, V, W, X, a, branch_result, g, l, n, o, q, u, y, z
    local e7 = {}
    local steps = {}
    steps.entry = function()
        do
            local temp_5
            temp_5 = (not captures[1].value.ScriptActive)
            branch_result = temp_5
            I = temp_5
        end
        if (not branch_result) then
            I = captures[4].value()
        end
        branch_result = I
        if (not branch_result) then
            do
                local temp_3
                temp_3 = workspace.CurrentCamera
                branch_result = (not temp_3)
                X = temp_3
            end
            if branch_result then
                return nil, pack_values(unpack_values({}))
            end
            do
                local temp_1, temp_4
                temp_1 = captures[6].value
                temp_4 = {ipairs(unpack_values({temp_1.GetPlayers(temp_1)}))}
                B, l, u = temp_4[1], temp_4[2], temp_4[3]
            end
            while true do
                do
                    local temp_1, temp_2
                    temp_1, temp_2 = B(l, u)
                    branch_result = temp_1
                    g, u = temp_2, temp_1
                end
                if (not branch_result) then
                    do
                        local temp_2
                        temp_2 = {pairs(captures[5].value)}
                        l, o, u = temp_2[1], temp_2[3], temp_2[2]
                    end
                    while true do
                        do
                            local temp_1, temp_2
                            temp_1, temp_2 = l(u, o)
                            branch_result = temp_1
                            g, o = temp_2, temp_1
                        end
                        if (not branch_result) then
                            return nil, pack_values(unpack_values({}))
                        end
                        branch_result = (not o.Parent)
                        B = o
                        if branch_result then
                            branch_result = g.Box
                            if branch_result then
                                do
                                    local temp_3
                                    temp_3 = g.Box
                                    temp_3.Destroy(temp_3)
                                end
                            end
                            branch_result = g.NameText
                            if branch_result then
                                do
                                    local temp_3
                                    temp_3 = g.NameText
                                    temp_3.Destroy(temp_3)
                                end
                            end
                            branch_result = g.HealthBg
                            if branch_result then
                                do
                                    local temp_3
                                    temp_3 = g.HealthBg
                                    temp_3.Destroy(temp_3)
                                end
                            end
                            branch_result = g.Line
                            if branch_result then
                                do
                                    local temp_3
                                    temp_3 = g.Line
                                    temp_3.Destroy(temp_3)
                                end
                            end
                            branch_result = g.Cham
                            if branch_result then
                                do
                                    local temp_3
                                    temp_3 = g.Cham
                                    temp_3.Destroy(temp_3)
                                end
                            end
                            captures[5].value[B] = nil
                        end
                    end
                end
                do
                    local temp_2
                    temp_2 = (g ~= captures[7].value)
                    branch_result = temp_2
                    q = temp_2
                end
                if branch_result then
                    q = g.Character
                end
                branch_result = q
                if branch_result then
                    do
                        local temp_11, temp_3, temp_7
                        temp_3 = g.Character
                        temp_7 = temp_3.FindFirstChildOfClass(temp_3, "Humanoid")
                        temp_11 = temp_3.FindFirstChild(temp_3, "HumanoidRootPart")
                        branch_result = temp_11
                        J, a, q = temp_11, temp_7, temp_3
                    end
                    if (not branch_result) then
                        do
                            local temp_4
                            temp_4 = q.FindFirstChild(q, "Torso")
                            branch_result = temp_4
                            A = temp_4
                        end
                        if (not branch_result) then
                            do
                                local temp_4
                                temp_4 = q.FindFirstChild(q, "UpperTorso")
                                branch_result = temp_4
                                K = temp_4
                            end
                            if (not branch_result) then
                                K = q.PrimaryPart
                            end
                            A = K
                        end
                        J = A
                    end
                    do
                        local temp_4
                        temp_4 = q.FindFirstChild(q, "Head")
                        branch_result = temp_4
                        A = temp_4
                    end
                    if (not branch_result) then
                        A = J
                    end
                    branch_result = a
                    z = a
                    if branch_result then
                        do
                            local temp_4
                            temp_4 = (a.Health > 0)
                            branch_result = temp_4
                            K = temp_4
                        end
                        if branch_result then
                            K = captures[8].value(g)
                        end
                        z = K
                    end
                    do
                        local temp_2
                        temp_2 = captures[9].value(g)
                        branch_result = z
                        D, K = z, temp_2
                    end
                    if branch_result then
                        branch_result = J
                        M = J
                        if branch_result then
                            M = A
                        end
                        D = M
                    end
                    branch_result = D
                    if branch_result then
                        branch_result = K.Cham
                        if branch_result then
                            K.Cham.Adornee = q
                            K.Cham.Enabled = captures[1].value.ChamsEnabled
                            K.Cham.FillColor = captures[1].value.ChamsColor
                        end
                        do
                            local temp_17, temp_27, temp_5, temp_6, temp_7
                            temp_5 = {X.WorldToViewportPoint(X, J.Position)}
                            temp_6 = temp_5[1]
                            temp_7 = temp_5[2]
                            temp_17 = X.WorldToViewportPoint(X, (A.Position + Vector3.new(0, 0.5, 0)))
                            temp_27 = X.WorldToViewportPoint(X, (J.Position - Vector3.new(0, 3, 0)))
                            branch_result = temp_7
                            M, n, y = temp_6, temp_17, temp_27
                        end
                        if branch_result then
                            do
                                local temp_11, temp_12, temp_16
                                temp_11 = math.abs((n.Y - y.Y))
                                temp_12 = (temp_11 * 0.6)
                                temp_16 = captures[1].value.EspNameEnabled
                                branch_result = temp_16
                                Q, S, V = temp_11, temp_16, temp_12
                            end
                            if (not branch_result) then
                                S = captures[1].value.EspDistanceEnabled
                            end
                            branch_result = S
                            if branch_result then
                                K.NameText.Visible = true
                                K.NameText.Position = UDim2.new(0, M.X, 0, ((M.Y - (Q / 2)) - 5))
                                branch_result = captures[1].value.EspNameEnabled
                                S = ""
                                if branch_result then
                                    S = g.Name
                                end
                                branch_result = captures[1].value.EspDistanceEnabled
                                if branch_result then
                                    do
                                        local temp_17, temp_20
                                        temp_17 = math.floor((X.CFrame.Position - J.Position).Magnitude)
                                        temp_20 = (S == "")
                                        branch_result = temp_20
                                        R, W = temp_20, temp_17
                                    end
                                    if branch_result then
                                        R = ("[" .. (W .. "m]"))
                                    end
                                    branch_result = R
                                    G = R
                                    if (not branch_result) then
                                        G = (S .. (" [" .. (W .. "m]")))
                                    end
                                    S = G
                                end
                                K.NameText.Text = S
                            else
                                K.NameText.Visible = false
                            end
                            branch_result = captures[1].value.EspBoxEnabled
                            if branch_result then
                                K.Box.Visible = true
                                K.Box.Size = UDim2.new(0, V, 0, Q)
                                K.Box.Position = UDim2.new(0, (M.X - (V / 2)), 0, (M.Y - (Q / 2)))
                                K.BoxStroke.Color = captures[1].value.EspBoxColor
                            else
                                K.Box.Visible = false
                            end
                            branch_result = captures[1].value.EspHealthEnabled
                            if branch_result then
                                do
                                    local temp_46, temp_71, temp_76, temp_79, temp_84, temp_85
                                    K.HealthBg.Visible = true
                                    K.HealthBg.Size = UDim2.new(0, 3, 0, Q)
                                    K.HealthBg.Position = UDim2.new(0, ((M.X - (V / 2)) - 6), 0, (M.Y - (Q / 2)))
                                    temp_46 = math.clamp((a.Health / a.MaxHealth), 0, 1)
                                    K.HealthBar.Size = UDim2.new(1, 0, temp_46, 0)
                                    K.HealthBar.Position = UDim2.new(0, 0, (1 - temp_46), 0)
                                    temp_71 = math.clamp((255 - (temp_46 * 255)), 0, 255)
                                    temp_76 = math.clamp((temp_46 * 255), 0, 255)
                                    temp_79 = K.HealthBar
                                    temp_84 = Color3.fromRGB
                                    temp_85 = temp_84(temp_71, temp_76, 0)
                                    temp_79.BackgroundColor3 = temp_85
                                end
                            else
                                K.HealthBg.Visible = false
                            end
                            branch_result = captures[1].value.EspLineEnabled
                            if branch_result then
                                do
                                    local temp_13, temp_19
                                    K.Line.Visible = true
                                    temp_13 = (X.ViewportSize.X / 2)
                                    temp_19 = X.ViewportSize.Y
                                    branch_result = (captures[1].value.EspLinePosition == "Arriba")
                                    S, W = temp_13, temp_19
                                end
                                if branch_result then
                                    W = 0
                                else
                                    branch_result = (captures[1].value.EspLinePosition == "Medio")
                                    if branch_result then
                                        W = (X.ViewportSize.Y / 2)
                                    end
                                end
                                do
                                    local temp_14, temp_4, temp_70, temp_73, temp_83, temp_86, temp_89
                                    temp_4 = Vector2.new(S, W)
                                    temp_14 = Vector2.new(M.X, M.Y)
                                    K.Line.Size = UDim2.new(0, 1, 0, (temp_14 - temp_4).Magnitude)
                                    K.Line.Position = UDim2.new(0, ((temp_4.X + temp_14.X) / 2), 0, ((temp_4.Y + temp_14.Y) / 2))
                                    temp_70 = math.atan2((temp_14.Y - temp_4.Y), (temp_14.X - temp_4.X))
                                    temp_73 = K.Line
                                    temp_73.Rotation = (math.deg(temp_70) - 90)
                                    temp_83 = K.Line
                                    temp_86 = captures[1].value
                                    temp_89 = temp_86.EspLineColor
                                    temp_83.BackgroundColor3 = temp_89
                                end
                            else
                                K.Line.Visible = false
                            end
                        else
                            K.Box.Visible = false
                            K.HealthBg.Visible = false
                            K.Line.Visible = false
                            K.NameText.Visible = false
                        end
                    else
                        branch_result = K.Cham
                        if branch_result then
                            K.Cham.Enabled = false
                        end
                        K.Box.Visible = false
                        K.HealthBg.Visible = false
                        K.Line.Visible = false
                        K.NameText.Visible = false
                    end
                end
            end
        end
        do
            local temp_2
            temp_2 = {pairs(captures[5].value)}
            B, X, l = temp_2[3], temp_2[2], temp_2[1]
        end
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            return nil, pack_values(unpack_values({}))
        end
        branch_result = o.Box
        if branch_result then
            o.Box.Visible = false
        end
        branch_result = o.NameText
        if branch_result then
            o.NameText.Visible = false
        end
        branch_result = o.HealthBg
        if branch_result then
            o.HealthBg.Visible = false
        end
        branch_result = o.Line
        if branch_result then
            o.Line.Visible = false
        end
        captures[7].value()
        getgenv().KaiserTargetPart = nil
        return "step_2"
    end
    steps.step_2 = function()
        branch_result = task.wait(0.03)
        if (not branch_result) then
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_1, temp_2, temp_4
            temp_1 = captures[3].value
            temp_2 = captures[1].value
            temp_4 = temp_1.AutoShootEnabled
            branch_result = temp_4
            I, u = temp_4, temp_2
        end
        if branch_result then
            do
                local temp_1, temp_4
                temp_1 = captures[3].value
                temp_4 = temp_1.ScriptActive
                branch_result = temp_4
                X, u = temp_4, temp_1
            end
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[4].value
                    X, u = (not temp_1()), temp_1
                end
            end
            I = X
        end
        branch_result = I
        if branch_result then
            return "step_3"
        else
            return "step_9"
        end
    end
    steps.step_3 = function()
        branch_result = ((tick() - captures[5].value) < captures[6].value)
        if branch_result then
            return "step_4"
        else
            return "step_5"
        end
    end
    steps.step_4 = function()
        captures[7].value()
        getgenv().KaiserTargetPart = nil
        return "step_2"
    end
    steps.step_5 = function()
        do
            local temp_4
            temp_4 = captures[8].value.Character
            branch_result = temp_4
            B, I = temp_4, temp_4
        end
        if branch_result then
            I = B.FindFirstChild(B, "HumanoidRootPart")
        end
        do
            local temp_1
            temp_1 = (not B)
            branch_result = temp_1
            I, l = temp_1, I
        end
        if (not branch_result) then
            I = (not l)
        end
        branch_result = I
        if branch_result then
            return "step_6"
        else
            return "step_7"
        end
    end
    steps.step_6 = function()

        return "step_2"
    end
    steps.step_7 = function()
        do
            local temp_1
            temp_1 = {}
            temp_1.value = captures[9].value()
            branch_result = temp_1.value
            u = temp_1
        end
        if branch_result then
            do
                local temp_2
                temp_2 = captures[10].value()
                branch_result = temp_2
                o = temp_2
            end
            if branch_result then
                do
                    local temp_7
                    getgenv().KaiserTargetPart = u.value
                    temp_7 = workspace.CurrentCamera
                    branch_result = temp_7
                    g = temp_7
                end
                if branch_result then
                    do
                        local temp_10, temp_4, temp_7
                        temp_4 = g.CFrame
                        temp_7 = l.CFrame
                        temp_10 = captures[11].value(u.value, 2000, true)
                        branch_result = temp_10
                        I, a, q = temp_10, temp_7, temp_4
                    end
                    if (not branch_result) then
                        I = u.value.Position
                    end
                    do
                        local temp_1, temp_11, temp_14, temp_26, temp_3
                        temp_1 = captures[12].value
                        temp_3 = temp_1.GetMouseLocation(temp_1)
                        temp_11 = g.ViewportPointToRay(g, temp_3.X, temp_3.Y)
                        temp_14 = g.CFrame
                        temp_26 = CFrame.lookAt(Vector3.zero, temp_14.VectorToObjectSpace(temp_14, temp_11.Direction))
                        Q, n, y = 0, (CFrame.lookAt(g.CFrame.Position, (g.CFrame.Position + (I - g.CFrame.Position).Unit)) * temp_26.Inverse(temp_26)), Vector3.new(I.X, l.Position.Y, I.Z)
                    end
                    while true do
                        do
                            local temp_1
                            temp_1 = (1 + Q)
                            branch_result = ((false and (temp_1 >= 2)) or ((not false) and (2 >= temp_1)))
                            Q = temp_1
                        end
                        if not branch_result then break end
                        g.CFrame = n
                        l.CFrame = CFrame.lookAt(l.Position, y)
                        branch_result = (Q == 1)
                        if branch_result then
                            o.Activate(o)
                            branch_result = u.value.Parent
                            if branch_result then
                                pcall(bind(callbacks.callback_127, {u, captures[1], captures[2]}))
                            end
                        end
                        do
                            local temp_4
                            temp_4 = captures[13].value.RenderStepped
                            temp_4.Wait(temp_4)
                        end
                    end
                    captures[5].value = tick()
                    branch_result = (not captures[3].value.AimbotEnabled)
                    if branch_result then
                        g.CFrame = q
                        l.CFrame = a
                    end
                    task.wait(0.04)
                    captures[7].value()
                end
            end
        else
            getgenv().KaiserTargetPart = nil
        end
        return "step_8"
    end
    steps.step_8 = function()

        return "step_2"
    end
    steps.step_9 = function()
        getgenv().KaiserTargetPart = nil
        return "step_8"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- callback_180; bloques originales: 5
callbacks.callback_180 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = false
        captures[4].value = X.Position
    end
    return unpack_values({})
end

-- callback_181; bloques originales: 9
callbacks.callback_181 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseMovement)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        do
            local temp_1
            temp_1 = captures[3].value
            branch_result = temp_1
            I = temp_1
        end
        if branch_result then
            I = ((X.Position - captures[3].value).Magnitude > 5)
        end
        branch_result = I
        if branch_result then
            captures[4].value = true
        end
    end
    return unpack_values({})
end

-- callback_182; bloques originales: 9
callbacks.callback_182 = function(captures, arguments)
    local B, branch_result, l, o, u
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        return unpack_values({})
    end
    captures[2].value.InvisibleEnabled = (not captures[2].value.InvisibleEnabled)
    captures[5].value(captures[2].value.InvisibleEnabled)
    branch_result = captures[6].value.InvisibleEnabled
    if branch_result then
        captures[6].value.InvisibleEnabled(captures[2].value.InvisibleEnabled)
    end
    do
        local temp_1, temp_7
        temp_1 = captures[7].value
        temp_7 = captures[2].value.InvisibleEnabled
        branch_result = temp_7
        l, o, u = temp_1, temp_1, temp_7
    end
    if branch_result then
        u = "Invisible Activado"
    end
    branch_result = u
    B = u
    if (not branch_result) then
        B = "Invisible Desactivado"
    end
    l("KaiserHub", B)
    captures[8].value()
    return unpack_values({})
end

-- callback_183; bloques originales: 5
callbacks.callback_183 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_11, temp_2
        temp_2 = arguments[1]
        temp_11 = (temp_2.UserInputType == Enum.UserInputType.MouseButton1)
        branch_result = temp_11
        I, X = temp_11, temp_2
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        captures[3].value = false
        captures[4].value = X.Position
    end
    return unpack_values({})
end

-- callback_184; bloques originales: 9
callbacks.callback_184 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    do
        local temp_1, temp_11
        temp_1 = arguments[1]
        temp_11 = (temp_1.UserInputType == Enum.UserInputType.MouseMovement)
        branch_result = temp_11
        I, X = temp_11, temp_1
    end
    if (not branch_result) then
        I = (X.UserInputType == Enum.UserInputType.Touch)
    end
    branch_result = I
    if branch_result then
        do
            local temp_1
            temp_1 = captures[3].value
            branch_result = temp_1
            I = temp_1
        end
        if branch_result then
            I = ((X.Position - captures[3].value).Magnitude > 5)
        end
        branch_result = I
        if branch_result then
            captures[4].value = true
        end
    end
    return unpack_values({})
end

-- callback_185; bloques originales: 18
callbacks.callback_185 = function(captures, arguments)
    local B, X, branch_result, g, l, o, u
    local e7 = {}
    branch_result = captures[1].value
    if branch_result then
        return unpack_values({})
    end
    captures[2].value.KillAuraEnabled = (not captures[2].value.KillAuraEnabled)
    branch_result = captures[5].value.KillAuraEnabled
    if branch_result then
        captures[5].value.KillAuraEnabled(captures[2].value.KillAuraEnabled)
    end
    do
        local temp_1, temp_7
        temp_1 = captures[6].value
        temp_7 = captures[2].value.KillAuraEnabled
        branch_result = temp_7
        l, o, u = temp_1, temp_1, temp_7
    end
    if branch_result then
        u = "Kill Aura Activado"
    end
    branch_result = u
    B = u
    if (not branch_result) then
        B = "Kill Aura Desactivado"
    end
    l("KaiserHub", B)
    captures[7].value()
    branch_result = (not captures[2].value.KillAuraEnabled)
    if branch_result then
        do
            local temp_1, temp_4
            temp_1 = captures[8].value
            temp_4 = {ipairs(unpack_values({temp_1.GetPlayers(temp_1)}))}
            B, X, l = temp_4[3], temp_4[2], temp_4[1]
        end
        while true do
            do
                local temp_1, temp_2
                temp_1, temp_2 = l(X, B)
                branch_result = temp_1
                B, o = temp_1, temp_2
            end
            if not branch_result then break end
            branch_result = o.Character
            if branch_result then
                do
                    local temp_3, temp_7
                    temp_3 = o.Character
                    temp_7 = temp_3.FindFirstChild(temp_3, "CustomHitbox")
                    branch_result = temp_7
                    g = temp_7
                end
                if branch_result then
                    g.Destroy(g)
                end
            end
        end
    end
    return unpack_values({})
end

-- callback_186; bloques originales: 6
callbacks.callback_186 = function(captures, arguments)
    local X, branch_result
    local e7 = {}
    do
        local temp_1
        temp_1 = arguments[1]
        branch_result = captures[1].value
        X = temp_1
    end
    if branch_result then
        return unpack_values({})
    end
    captures[1].value = true
    branch_result = X
    if branch_result then
        do
            local temp_31, temp_47, temp_48, temp_54, temp_57, temp_67, temp_72
            captures[2].value.GroupTransparency = 1
            captures[5].value.Scale = (captures[6].value.UIScale * 0.97)
            captures[2].value.Visible = true
            temp_31 = TweenInfo.new(0.22, Enum.EasingStyle.Quad, Enum.EasingDirection.Out)
            temp_47 = TweenInfo.new(0.28, Enum.EasingStyle.Quad, Enum.EasingDirection.Out)
            temp_48 = captures[7].value
            temp_54 = temp_48.Create(temp_48, captures[2].value, temp_31, {["GroupTransparency"] = 0})
            temp_54.Play(temp_54)
            temp_57 = captures[7].value
            temp_67 = temp_57.Create(temp_57, captures[5].value, temp_47, {["Scale"] = captures[6].value.UIScale})
            temp_67.Play(temp_67)
            temp_72 = temp_67.Completed
            temp_72.Wait(temp_72)
        end
    else
        do
            local temp_16, temp_32, temp_33, temp_39, temp_40, temp_51, temp_58
            temp_16 = TweenInfo.new(0.14, Enum.EasingStyle.Quad, Enum.EasingDirection.In)
            temp_32 = TweenInfo.new(0.18, Enum.EasingStyle.Quad, Enum.EasingDirection.In)
            temp_33 = captures[7].value
            temp_39 = temp_33.Create(temp_33, captures[2].value, temp_16, {["GroupTransparency"] = 1})
            temp_40 = captures[7].value
            temp_51 = temp_40.Create(temp_40, captures[5].value, temp_32, {["Scale"] = (captures[6].value.UIScale * 0.96)})
            temp_39.Play(temp_39)
            temp_51.Play(temp_51)
            temp_58 = temp_39.Completed
            temp_58.Wait(temp_58)
            captures[2].value.Visible = false
            captures[2].value.GroupTransparency = 0
            captures[5].value.Scale = captures[6].value.UIScale
        end
    end
    captures[1].value = false
    return unpack_values({})
end

-- callback_187; bloques originales: 4
callbacks.callback_187 = function(captures, arguments)
    local B, X, a, branch_result, g, o, u
    local e7 = {}
    do
        local temp_1, temp_35, temp_38, temp_44, temp_45, temp_46, temp_47, temp_7, temp_8
        temp_1 = {}
        temp_1.value = arguments[1]
        temp_7 = Instance.new("Frame")
        temp_8 = {}
        temp_8.value = temp_7
        temp_8.value.Name = "ContenedorEstrellas"
        temp_8.value.Size = UDim2.new(1, 0, 1, 0)
        temp_8.value.BackgroundTransparency = 1
        temp_8.value.ClipsDescendants = true
        temp_8.value.ZIndex = 2
        temp_8.value.Active = false
        temp_35 = temp_8.value
        temp_38 = {}
        temp_35.Parent = temp_1.value
        temp_38.value = {}
        temp_44 = Random.new()
        temp_45 = {}
        temp_46 = {}
        temp_47 = bind(callbacks.callback_79, {captures[1], captures[2], temp_8, temp_46})
        temp_46.value = temp_44
        temp_45.value = temp_47
        B, X, a, g, o, u = temp_8, temp_1, 0, temp_45, temp_46, temp_38
    end
    while true do
        do
            local temp_1
            temp_1 = (1 + a)
            branch_result = ((false and (temp_1 >= 90)) or ((not false) and (temp_1 <= 90)))
            a = temp_1
        end
        if not branch_result then break end
        table.insert(u.value, unpack_values({g.value(false)}))
    end
    do
        local temp_1, temp_10, temp_5
        temp_1 = {}
        temp_1.value = nil
        temp_5 = captures[3].value.RenderStepped
        temp_1.value = temp_5.Connect(temp_5, bind(callbacks.callback_193, {X, captures[1], captures[2], captures[4], temp_1, u, g}))
        temp_10 = {}
        table.insert(captures[5].value, temp_1.value)
        return unpack_values(temp_10)
    end
end

-- callback_188; bloques originales: 5
callbacks.callback_188 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value.UIScale = 1
    branch_result = captures[4].value
    if branch_result then
        captures[4].value.Scale = 1
    end
    branch_result = captures[5].value
    if branch_result then
        captures[5].value.Size = UDim2.new(0, (captures[6].value.X * 1), 0, (captures[6].value.Y * 1))
        captures[5].value.Position = UDim2.new(0.5, ((- (captures[6].value.X * 1)) / 2), 0.5, ((- (captures[6].value.Y * 1)) / 2))
    end
    captures[7].value()
    captures[8].value("KaiserHub", "Tama帽o del panel reiniciado al recomendado (100%)")
    return unpack_values({})
end

-- callback_189; bloques originales: 5
callbacks.callback_189 = function(captures, arguments)
    local B, I, X, branch_result, l, u
    local e7 = {}
    do
        local temp_1, temp_11, temp_14, temp_15, temp_16, temp_17, temp_19, temp_21, temp_22, temp_7, temp_8
        temp_1 = {}
        temp_1.value = 3690079931
        temp_7 = Enum.ThumbnailType.HeadShot
        temp_8 = {}
        temp_8.value = temp_7
        temp_11 = Enum.ThumbnailSize
        temp_14 = bind(callbacks.callback_1, {captures[1], captures[2], temp_1, captures[3]})
        temp_15 = temp_11.Size420x420
        temp_16 = {}
        temp_16.value = temp_15
        temp_17 = bind(callbacks.callback_2, {captures[4], temp_1, temp_8, temp_16})
        pcall(temp_14)
        temp_19 = {pcall(temp_17)}
        temp_21 = temp_19[2]
        temp_22 = temp_19[1]
        branch_result = temp_22
        B, I, X, l, u = temp_8, temp_22, temp_1, temp_16, temp_21
    end
    if branch_result then
        I = u
    end
    branch_result = I
    if branch_result then
        captures[5].value.Image = u
    end
    return unpack_values({})
end

-- callback_190; bloques originales: 1
callbacks.callback_190 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value()
    return unpack_values({})
end

-- callback_191; bloques originales: 1
callbacks.callback_191 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value(false)
    return unpack_values({})
end

-- callback_192; bloques originales: 1
callbacks.callback_192 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({(arguments[1].dist < arguments[2].dist)})
end

-- callback_193; bloques originales: 13
callbacks.callback_193 = function(captures, arguments)
    local B, I, X, branch_result, g, l, q, u
    local e7 = {}
    do
        local temp_1, temp_3
        temp_1 = arguments[1]
        temp_3 = (not captures[1].value)
        branch_result = temp_3
        I, X = temp_3, temp_1
    end
    if (not branch_result) then
        do
            local temp_5
            temp_5 = (not captures[1].value.Parent)
            branch_result = temp_5
            B = temp_5
        end
        if (not branch_result) then
            B = (not captures[4].value.ScriptActive)
        end
        I = B
    end
    branch_result = I
    if branch_result then
        do
            local temp_1
            temp_1 = captures[5].value
            temp_1.Disconnect(temp_1)
            return unpack_values({})
        end
    end
    do
        local temp_2
        temp_2 = {ipairs(captures[6].value)}
        B, l, u = temp_2[2], temp_2[3], temp_2[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = u(B, l)
            branch_result = temp_1
            g, l = temp_2, temp_1
        end
        if (not branch_result) then
            return unpack_values({})
        end
        do
            local temp_3
            temp_3 = g.Instancia
            g.XScale = (g.XScale - (g.Velocidad * X))
            branch_result = (g.XScale < -0.02)
            q = temp_3
        end
        if branch_result then
            do
                local temp_5
                q.Destroy(q)
                temp_5 = captures[7].value(true)
                g.Instancia = temp_5.Instancia
                g.Velocidad = temp_5.Velocidad
                g.XScale = temp_5.XScale
                g.YScale = temp_5.YScale
            end
        else
            q.Position = UDim2.new(g.XScale, 0, g.YScale, 0)
        end
    end
end

-- callback_194; bloques originales: 1
callbacks.callback_194 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[1].value(captures[2].value)
    return unpack_values({})
end

-- callback_195; bloques originales: 1
callbacks.callback_195 = function(captures, arguments)
    local branch_result
    local e7 = {}
    collectgarbage("collect")
    return unpack_values({})
end

-- callback_196; bloques originales: 1
callbacks.callback_196 = function(captures, arguments)
    local branch_result
    local e7 = {}
    captures[4].value.Text = (math.floor((math.clamp(captures[3].value.Size.X.Scale, 0, 1) * 100)) .. "%")
    return unpack_values({})
end

-- callback_197; bloques originales: 4
callbacks.callback_197 = function(captures, arguments)
    local B, X, branch_result, l, o
    local e7 = {}
    do
        local temp_2
        temp_2 = {ipairs(captures[1].value)}
        B, X, l = temp_2[3], temp_2[2], temp_2[1]
    end
    while true do
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if not branch_result then break end
        captures[2].value.Text = o
        task.wait(captures[5].value)
    end
    return unpack_values({})
end

-- callback_198; bloques originales: 3
callbacks.callback_198 = function(captures, arguments)
    local B, I, branch_result
    local e7 = {}
    do
        local temp_2, temp_29, temp_38, temp_40, temp_49, temp_52, temp_7
        temp_2 = arguments[1]
        temp_7 = Instance.new("Frame")
        temp_7.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        temp_7.BorderSizePixel = 0
        temp_7.ZIndex = 2
        temp_7.Active = false
        temp_7.Parent = captures[3].value
        temp_29 = Instance.new("UICorner")
        temp_29.CornerRadius = UDim.new(1, 0)
        temp_29.Parent = temp_7
        temp_38 = captures[4].value
        temp_40 = temp_38.NextInteger(temp_38, 2, 3)
        temp_7.Size = UDim2.new(0, temp_40, 0, temp_40)
        temp_49 = captures[4].value
        temp_7.BackgroundTransparency = temp_49.NextNumber(temp_49, 0.1, 0.1)
        temp_52 = (temp_2 and 1.02)
        branch_result = temp_52
        B, I = temp_7, temp_52
    end
    if (not branch_result) then
        do
            local temp_1
            temp_1 = captures[4].value
            I = temp_1.NextNumber(temp_1, 0, 1)
        end
    end
    do
        local temp_1, temp_10, temp_3
        temp_1 = captures[4].value
        temp_3 = temp_1.NextNumber(temp_1, 0, 0.98)
        B.Position = UDim2.new(I, 0, temp_3, 0)
        temp_10 = captures[4].value
        return unpack_values({{["Instancia"] = B, ["Velocidad"] = temp_10.NextNumber(temp_10, 0.1, 0.25), ["XScale"] = I, ["YScale"] = temp_3}})
    end
end

-- callback_199; bloques originales: 13
callbacks.callback_199 = function(captures, arguments)
    local B, I, X, branch_result, l
    local e7 = {}
    branch_result = captures[1].value.GetNetworkPing
    if branch_result then
        do
            local temp_1, temp_3, temp_4
            temp_1 = captures[1].value
            temp_3 = temp_1.GetNetworkPing(temp_1)
            temp_4 = (temp_3 > 5)
            branch_result = temp_4
            B, X, l = temp_4, temp_3, temp_1
        end
        if branch_result then
            B = (X / 1000)
        end
        branch_result = B
        I = B
        if (not branch_result) then
            I = X
        end
        captures[4].value = I
    else
        do
            local temp_1
            temp_1 = captures[5].value
            branch_result = temp_1
            X = temp_1
        end
        if branch_result then
            do
                local temp_1, temp_5
                temp_1 = captures[5].value
                temp_5 = temp_1.FindFirstChild(temp_1, "Network")
                branch_result = temp_5
                B = temp_5
            end
            if branch_result then
                do
                    local temp_4
                    temp_4 = captures[5].value.Network
                    B = temp_4.FindFirstChild(temp_4, "ServerStatsItem")
                end
            end
            X = B
        end
        branch_result = X
        if branch_result then
            do
                local temp_10
                temp_10 = captures[5].value.Network.ServerStatsItem["Data Ping"]
                captures[4].value = (temp_10.GetValue(temp_10) / 1000)
            end
        end
    end
    return unpack_values({})
end

-- callback_200; bloques originales: 1
callbacks.callback_200 = function(captures, arguments)
    local branch_result
    local e7 = {}
    do
        local temp_4
        temp_4 = game.GetService(game, "RbxAnalyticsService")
        return unpack_values({unpack_values({temp_4.GetClientId(temp_4)})})
    end
end

-- callback_201; bloques originales: 3
callbacks.callback_201 = function(captures, arguments)
    local branch_result
    local e7 = {}
    branch_result = (captures[1].value.UserInputState == Enum.UserInputState.End)
    if branch_result then
        captures[4].value = false
    end
    return unpack_values({})
end

-- callback_202; bloques originales: 11
callbacks.callback_202 = function(captures, arguments)
    local I, X, branch_result
    local e7 = {}
    branch_result = (not captures[1].value(captures[2].value))
    if branch_result then
        captures[3].value(captures[2].value)
    end
    branch_result = (not captures[4].value(captures[5].value))
    if branch_result then
        do
            local temp_3
            temp_3 = game.HttpGet(game, captures[6].value)
            branch_result = temp_3
            I, X = temp_3, temp_3
        end
        if branch_result then
            I = ((# X) > 0)
        end
        branch_result = I
        if branch_result then
            captures[7].value(captures[5].value, X)
        end
    end
    branch_result = captures[4].value(captures[5].value)
    if branch_result then
        captures[9].value = captures[8].value(captures[5].value)
    end
    return unpack_values({})
end

-- callback_203; bloques originales: 1
callbacks.callback_203 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({("wApzWRd" / (14518345 - ("849htSvC6qy" ^ 15743726)))})
end

-- callback_204; bloques originales: 1
callbacks.callback_204 = function(captures, arguments)
    local branch_result
    local e7 = {}
    return unpack_values({unpack_values({game.HttpGet(game, captures[1].value)})})
end

-- unused_205; bloques originales: 50
-- Bloque sin ruta desde la entrada original; conservado como referencia.
callbacks.unused_205 = function(captures, arguments)
    local B, I, Q, X, a, branch_result, g, l, n, o, q, u, y
    local e7 = {}
    local steps = {}
    steps.entry = function()
        branch_result = o.Cham
        if branch_result then
            o.Cham.Enabled = false
        end
        do
            local temp_1, temp_2
            temp_1, temp_2 = l(X, B)
            branch_result = temp_1
            B, o = temp_1, temp_2
        end
        if (not branch_result) then
            return nil, pack_values(unpack_values({}))
        end
        branch_result = o.Box
        if branch_result then
            o.Box.Visible = false
        end
        branch_result = o.NameText
        if branch_result then
            o.NameText.Visible = false
        end
        branch_result = o.HealthBg
        if branch_result then
            o.HealthBg.Visible = false
        end
        branch_result = o.Line
        if branch_result then
            o.Line.Visible = false
        end
        captures[7].value()
        getgenv().KaiserTargetPart = nil
        return "step_2"
    end
    steps.step_2 = function()
        branch_result = task.wait(0.03)
        if (not branch_result) then
            return nil, pack_values(unpack_values({}))
        end
        do
            local temp_1, temp_2, temp_4
            temp_1 = captures[3].value
            temp_2 = captures[1].value
            temp_4 = temp_1.AutoShootEnabled
            branch_result = temp_4
            I, u = temp_4, temp_2
        end
        if branch_result then
            do
                local temp_1, temp_4
                temp_1 = captures[3].value
                temp_4 = temp_1.ScriptActive
                branch_result = temp_4
                X, u = temp_4, temp_1
            end
            if branch_result then
                do
                    local temp_1
                    temp_1 = captures[4].value
                    X, u = (not temp_1()), temp_1
                end
            end
            I = X
        end
        branch_result = I
        if branch_result then
            return "step_3"
        else
            return "step_9"
        end
    end
    steps.step_3 = function()
        branch_result = ((tick() - captures[5].value) < captures[6].value)
        if branch_result then
            return "step_4"
        else
            return "step_5"
        end
    end
    steps.step_4 = function()
        captures[7].value()
        getgenv().KaiserTargetPart = nil
        return "step_2"
    end
    steps.step_5 = function()
        do
            local temp_4
            temp_4 = captures[8].value.Character
            branch_result = temp_4
            B, I = temp_4, temp_4
        end
        if branch_result then
            I = B.FindFirstChild(B, "HumanoidRootPart")
        end
        do
            local temp_1
            temp_1 = (not B)
            branch_result = temp_1
            I, l = temp_1, I
        end
        if (not branch_result) then
            I = (not l)
        end
        branch_result = I
        if branch_result then
            return "step_6"
        else
            return "step_7"
        end
    end
    steps.step_6 = function()

        return "step_2"
    end
    steps.step_7 = function()
        do
            local temp_1
            temp_1 = {}
            temp_1.value = captures[9].value()
            branch_result = temp_1.value
            u = temp_1
        end
        if branch_result then
            do
                local temp_2
                temp_2 = captures[10].value()
                branch_result = temp_2
                o = temp_2
            end
            if branch_result then
                do
                    local temp_7
                    getgenv().KaiserTargetPart = u.value
                    temp_7 = workspace.CurrentCamera
                    branch_result = temp_7
                    g = temp_7
                end
                if branch_result then
                    do
                        local temp_10, temp_4, temp_7
                        temp_4 = g.CFrame
                        temp_7 = l.CFrame
                        temp_10 = captures[11].value(u.value, 2000, true)
                        branch_result = temp_10
                        I, a, q = temp_10, temp_7, temp_4
                    end
                    if (not branch_result) then
                        I = u.value.Position
                    end
                    do
                        local temp_1, temp_11, temp_14, temp_26, temp_3
                        temp_1 = captures[12].value
                        temp_3 = temp_1.GetMouseLocation(temp_1)
                        temp_11 = g.ViewportPointToRay(g, temp_3.X, temp_3.Y)
                        temp_14 = g.CFrame
                        temp_26 = CFrame.lookAt(Vector3.zero, temp_14.VectorToObjectSpace(temp_14, temp_11.Direction))
                        Q, n, y = 0, (CFrame.lookAt(g.CFrame.Position, (g.CFrame.Position + (I - g.CFrame.Position).Unit)) * temp_26.Inverse(temp_26)), Vector3.new(I.X, l.Position.Y, I.Z)
                    end
                    while true do
                        do
                            local temp_1
                            temp_1 = (1 + Q)
                            branch_result = ((false and (temp_1 >= 2)) or ((not false) and (2 >= temp_1)))
                            Q = temp_1
                        end
                        if not branch_result then break end
                        g.CFrame = n
                        l.CFrame = CFrame.lookAt(l.Position, y)
                        branch_result = (Q == 1)
                        if branch_result then
                            o.Activate(o)
                            branch_result = u.value.Parent
                            if branch_result then
                                pcall(bind(callbacks.callback_127, {u, captures[1], captures[2]}))
                            end
                        end
                        do
                            local temp_4
                            temp_4 = captures[13].value.RenderStepped
                            temp_4.Wait(temp_4)
                        end
                    end
                    captures[5].value = tick()
                    branch_result = (not captures[3].value.AimbotEnabled)
                    if branch_result then
                        g.CFrame = q
                        l.CFrame = a
                    end
                    task.wait(0.04)
                    captures[7].value()
                end
            end
        else
            getgenv().KaiserTargetPart = nil
        end
        return "step_8"
    end
    steps.step_8 = function()

        return "step_2"
    end
    steps.step_9 = function()
        getgenv().KaiserTargetPart = nil
        return "step_8"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- unused_206; bloques originales: 7
-- Bloque sin ruta desde la entrada original; conservado como referencia.
callbacks.unused_206 = function(captures, arguments)
    local branch_result, q
    local e7 = {}
    local steps = {}
    steps.entry = function()
        l2 = q.value(1, 6)
        branch_result = (l2 > 2)
        if branch_result then
            return "step_2"
        else
            return "step_4"
        end
    end
    steps.step_2 = function()
        l2 = tostring(l1)
        return "step_3"
    end
    steps.step_3 = function()
        branch_result = true
        if (not branch_result) then
            return nil, pack_values(unpack_values({}))
        end
        l2 = q.value(1, 6)
        branch_result = (l2 > 2)
        if branch_result then
            return "step_2"
        else
            return "step_4"
        end
    end
    steps.step_4 = function()
        l1 = l2
        return "step_3"
    end
    local current_step, result = "entry", nil
    while current_step do
        current_step, result = steps[current_step]()
    end
    if result then
        return unpack_values(result, 1, result.n)
    end
end

-- unused_207; bloques originales: 7
-- Bloque sin ruta desde la entrada original; conservado como referencia.
callbacks.unused_207 = function(captures, arguments)
    local branch_result, q
    local e7 = {}
    while true do
        branch_result = true
        if (not branch_result) then
            return unpack_values({})
        end
        l2 = q.value(1, 6)
        branch_result = (l2 > 2)
        if branch_result then
            l2 = tostring(l1)
        else
            l1 = l2
        end
    end
end

-- main; bloques originales: 24
callbacks.main = function(captures, arguments)
    local A, B, D, Eh, F, Hh, J, K, M, P, R, W, Zh, a, branch_result, ch, g, ih, kh, l, m, o, q, u, w, y, z
    local e7 = {}
    do
        local temp_1, temp_2, temp_3, temp_4, temp_5, temp_6, temp_7
        temp_1 = {}
        temp_2 = {}
        temp_3 = {}
        temp_3.value = nil
        temp_4 = {}
        temp_4.value = nil
        temp_2.value = 2
        temp_5 = math.floor
        temp_6 = {}
        temp_7 = {}
        temp_7.value = temp_5
        temp_6.value = 0
        temp_1.value = {}
        A, B, D, J, a, g, l, o, q, u, z = math.random, temp_4, 0, table.remove, temp_1, temp_7, string.char, temp_2, temp_6, temp_3, {}
    end
    while true do
        do
            local temp_1, temp_2
            temp_1 = (not false)
            temp_2 = (D + 1)
            branch_result = ((false and (temp_2 >= 256)) or (temp_1 and (256 >= temp_2)))
            D = temp_2
        end
        if not branch_result then break end
        z[D] = D
    end
    while true do
        do
            local temp_3
            temp_3 = J(z, A(1, (# z)))
            a.value[temp_3] = l((temp_3 - 1))
            branch_result = ((# z) == 0)
        end
        if not (not branch_result) then break end
    end
    do
        local temp_1, temp_124, temp_125, temp_126, temp_131, temp_136, temp_137, temp_138, temp_143,
            temp_144, temp_145, temp_148, temp_15, temp_151, temp_152, temp_157, temp_16, temp_160, temp_161,
            temp_164, temp_167, temp_172, temp_173, temp_174, temp_175, temp_177, temp_20, temp_24, temp_25,
            temp_29, temp_3, temp_30, temp_34, temp_35, temp_4, temp_45, temp_46, temp_47, temp_48, temp_49,
            temp_5, temp_53, temp_56, temp_6, temp_60, temp_61, temp_67, temp_68, temp_84
        temp_1 = {}
        temp_1.value = {}
        temp_3 = bind(callbacks.next_decryption_byte, {temp_1, q, o, g})
        temp_4 = {}
        temp_4.value = temp_3
        temp_5 = {}
        temp_6 = {}
        temp_6.value = temp_5
        u.value = setmetatable({}, {["__index"] = temp_6.value, ["__metatable"] = nil})
        B.value = bind(callbacks.decode_cached_string, {temp_6, temp_1, a, q, o, temp_4})
        temp_15 = game.GetService(game, "HttpService")
        temp_16 = {}
        temp_16.value = temp_15
        temp_20 = game.GetService(game, "Players")
        temp_24 = game.GetService(game, "CoreGui")
        temp_25 = {}
        temp_25.value = temp_24
        temp_29 = game.GetService(game, "RunService")
        temp_30 = {}
        temp_30.value = temp_29
        temp_34 = game.GetService(game, "TweenService")
        temp_35 = {}
        temp_35.value = temp_34
        tostring(temp_20.LocalPlayer.UserId)
        temp_45 = bind(callbacks.callback_73, {u, B, temp_30})
        temp_46 = bind(callbacks.callback_74, {u, B})
        temp_47 = {}
        temp_47.value = temp_45
        temp_48 = {}
        temp_48.value = temp_46
        temp_49 = {}
        temp_49.value = bind(callbacks.build_loading_interface, {temp_25, u, B, temp_47, temp_35, temp_30, temp_48})
        temp_53 = {}
        temp_53.value = "https://files.catbox.moe/54lm4f.jpg"
        temp_56 = {}
        temp_56.value = "KaiserHub_Media"
        temp_60 = (temp_56.value .. "/KaiserHub_Bg.jpg10")
        temp_61 = {}
        temp_61.value = temp_60
        temp_67 = Instance.new("ScreenGui")
        temp_68 = {}
        temp_68.value = temp_67
        temp_68.value.Name = "KaiserAuthUI"
        temp_68.value.Parent = temp_25.value
        temp_84 = Instance.new("Frame", temp_68.value)
        temp_84.Size = UDim2.new(0, 320, 0, 170)
        temp_84.Position = UDim2.new(0.5, -160, 0.5, -85)
        temp_84.BackgroundTransparency = 1
        temp_84.BorderSizePixel = 0
        temp_84.Active = true
        temp_84.ClipsDescendants = true
        Instance.new("UICorner", temp_84).CornerRadius = UDim.new(0, 12)
        temp_124 = Instance.new("ImageLabel")
        temp_125 = {}
        temp_125.value = temp_124
        temp_126 = temp_125.value
        temp_126.Name = "BackgroundImage"
        temp_131 = temp_125.value
        temp_136 = UDim2.new
        temp_137 = temp_136(1, 0, 1, 0)
        temp_131.Size = temp_137
        temp_138 = temp_125.value
        temp_143 = UDim2.new
        temp_144 = temp_143(0, 0, 0, 0)
        temp_138.Position = temp_144
        temp_145 = temp_125.value
        temp_145.BackgroundTransparency = 1
        temp_148 = temp_125.value
        temp_151 = temp_53.value
        temp_148.Image = temp_151
        temp_152 = temp_125.value
        temp_157 = Enum.ScaleType
        temp_160 = temp_157.Crop
        temp_152.ScaleType = temp_160
        temp_161 = temp_125.value
        temp_161.ImageTransparency = 0
        temp_164 = temp_125.value
        temp_164.ZIndex = 1
        temp_167 = temp_125.value
        temp_167.Parent = temp_84
        temp_172 = game.GetService
        temp_173 = temp_172(game, "UserInputService")
        temp_174 = {}
        temp_174.value = temp_173
        temp_175 = bind(callbacks.callback_76, {u, B, temp_174, temp_35})
        temp_175(temp_84)
        temp_177 = temp_47.value
        temp_177(temp_84)
        branch_result = getcustomasset
        D, F, Hh, K, M, P, R, W, a, l, m, o, q, w, y = temp_48, temp_125, getcustomasset, temp_47, temp_49, temp_84, temp_61, temp_53, temp_35, temp_16, temp_174, temp_25, temp_30, temp_56, temp_68
    end
    if (not branch_result) then
        branch_result = getsynasset
        Zh = getsynasset
        if (not branch_result) then
            branch_result = fileasset
            ch = fileasset
            if branch_result then
                ch = bind(callbacks.callback_15, {u, B})
            end
            Zh = ch
        end
        Hh = Zh
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = Hh
        branch_result = isfile
        Hh, ih = isfile, temp_1
    end
    if (not branch_result) then
        branch_result = is_file
        kh = is_file
        if (not branch_result) then
            branch_result = readfile
            Eh = readfile
            if branch_result then
                Eh = bind(callbacks.callback_70, {})
            end
            kh = Eh
        end
        Hh = kh
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = Hh
        branch_result = writefile
        Hh, Zh = writefile, temp_1
    end
    if (not branch_result) then
        Hh = write_file
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = Hh
        branch_result = isfolder
        Hh, kh = isfolder, temp_1
    end
    if (not branch_result) then
        Hh = bind(callbacks.callback_81, {})
    end
    do
        local temp_1
        temp_1 = {}
        temp_1.value = Hh
        branch_result = makefolder
        Hh, ch = makefolder, temp_1
    end
    if (not branch_result) then
        Hh = bind(callbacks.callback_68, {})
    end
    do
        local temp_1, temp_102, temp_103, temp_108, temp_109, temp_118, temp_119, temp_12, temp_124,
            temp_127, temp_138, temp_141, temp_142, temp_143, temp_148, temp_149, temp_150, temp_155,
            temp_156, temp_157, temp_162, temp_167, temp_172, temp_173, temp_174, temp_177, temp_182,
            temp_183, temp_184, temp_189, temp_192, temp_193, temp_196, temp_199, temp_204, temp_207,
            temp_208, temp_214, temp_215, temp_218, temp_221, temp_226, temp_227, temp_232, temp_233,
            temp_242, temp_243, temp_248, temp_249, temp_254, temp_257, temp_272, temp_275, temp_280,
            temp_281, temp_284, temp_287, temp_292, temp_293, temp_300, temp_303, temp_306, temp_309,
            temp_310, temp_311, temp_314, temp_317, temp_320, temp_323, temp_324, temp_325, temp_328,
            temp_331, temp_332, temp_333, temp_336, temp_339, temp_34, temp_340, temp_341, temp_344,
            temp_347, temp_348, temp_349, temp_35, temp_352, temp_355, temp_356, temp_357, temp_358,
            temp_359, temp_36, temp_360, temp_361, temp_364, temp_365, temp_366, temp_367, temp_370,
            temp_371, temp_372, temp_83, temp_84, temp_85, temp_88, temp_89, temp_90, temp_91, temp_94,
            temp_97
        temp_1 = {}
        temp_1.value = Hh
        task.spawn(bind(callbacks.callback_26, {kh, Zh, temp_1, ih, ch, w, R, W, F, u, B}))
        temp_12 = Instance.new("UIStroke", P)
        temp_12.Color = Color3.fromRGB(255, 255, 255)
        temp_12.Thickness = 3
        temp_12.ApplyStrokeMode = Enum.ApplyStrokeMode.Border
        temp_34 = Instance.new("UIGradient", temp_12)
        temp_35 = {}
        temp_35.value = temp_34
        temp_36 = temp_35.value
        temp_83 = ColorSequence.new({ColorSequenceKeypoint.new(0, unpack_values({Color3.fromRGB(255, 255, 255)})), ColorSequenceKeypoint.new(0.25, unpack_values({Color3.fromRGB(255, 255, 255)})), ColorSequenceKeypoint.new(0.5, unpack_values({Color3.fromRGB(0, 0, 0)})), ColorSequenceKeypoint.new(0.75, unpack_values({Color3.fromRGB(0, 0, 0)})), unpack_values({ColorSequenceKeypoint.new(1, unpack_values({Color3.fromRGB(192, 192, 192)}))})})
        temp_36.Color = temp_83
        temp_84 = {}
        temp_84.value = nil
        temp_85 = q.value
        temp_88 = temp_85.RenderStepped
        temp_89 = bind(callbacks.callback_27, {temp_35, u, B, temp_84})
        temp_90 = temp_88.Connect
        temp_91 = temp_90(temp_88, temp_89)
        temp_84.value = temp_91
        temp_94 = Instance.new
        temp_97 = temp_94("TextLabel", P)
        temp_102 = UDim2.new
        temp_103 = temp_102(1, 0, 0, 25)
        temp_97.Size = temp_103
        temp_108 = UDim2.new
        temp_109 = temp_108(0, 0, 0.14, 0)
        temp_97.Position = temp_109
        temp_97.Text = "Kaiser Hub Ingresa Tu Key"
        temp_118 = Color3.fromRGB
        temp_119 = temp_118(255, 255, 255)
        temp_97.TextColor3 = temp_119
        temp_124 = Enum.Font
        temp_127 = temp_124.BuilderSansBold
        temp_97.Font = temp_127
        temp_97.TextSize = 20
        temp_97.BackgroundTransparency = 1
        temp_97.ZIndex = 3
        temp_97.Parent = P
        temp_138 = Instance.new
        temp_141 = temp_138("TextBox", P)
        temp_142 = {}
        temp_142.value = temp_141
        temp_143 = temp_142.value
        temp_148 = UDim2.new
        temp_149 = temp_148(0, 280, 0, 42)
        temp_143.Size = temp_149
        temp_150 = temp_142.value
        temp_155 = UDim2.new
        temp_156 = temp_155(0.5, -140, 0.38, 0)
        temp_150.Position = temp_156
        temp_157 = temp_142.value
        temp_157.PlaceholderText = "Pega tu key aqu铆"
        temp_162 = temp_142.value
        temp_162.Text = ""
        temp_167 = temp_142.value
        temp_172 = Color3.fromRGB
        temp_173 = temp_172(24, 24, 28)
        temp_167.BackgroundColor3 = temp_173
        temp_174 = temp_142.value
        temp_174.BackgroundTransparency = 0.2
        temp_177 = temp_142.value
        temp_182 = Color3.new
        temp_183 = temp_182(1, 1, 1)
        temp_177.TextColor3 = temp_183
        temp_184 = temp_142.value
        temp_189 = Enum.Font
        temp_192 = temp_189.BuilderSansBold
        temp_184.Font = temp_192
        temp_193 = temp_142.value
        temp_193.TextSize = 14
        temp_196 = temp_142.value
        temp_196.ZIndex = 3
        temp_199 = temp_142.value
        temp_199.Parent = P
        temp_204 = Instance.new
        temp_207 = temp_142.value
        temp_208 = temp_204("UICorner", temp_207)
        temp_214 = UDim.new
        temp_215 = temp_214(0, 12)
        temp_208.CornerRadius = temp_215
        temp_218 = Instance.new
        temp_221 = temp_218("TextButton", P)
        temp_226 = UDim2.new
        temp_227 = temp_226(0, 130, 0, 38)
        temp_221.Size = temp_227
        temp_232 = UDim2.new
        temp_233 = temp_232(0.5, -65, 0.72, 0)
        temp_221.Position = temp_233
        temp_221.Text = "Verificar"
        temp_242 = Color3.fromRGB
        temp_243 = temp_242(192, 192, 192)
        temp_221.BackgroundColor3 = temp_243
        temp_248 = Color3.new
        temp_249 = temp_248(0, 0, 0)
        temp_221.TextColor3 = temp_249
        temp_254 = Enum.Font
        temp_257 = temp_254.BuilderSansBold
        temp_221.Font = temp_257
        temp_221.TextSize = 14
        temp_221.Active = true
        temp_221.AutoButtonColor = false
        temp_221.ZIndex = 3
        temp_221.Parent = P
        temp_272 = Instance.new
        temp_275 = temp_272("UICorner", temp_221)
        temp_280 = UDim.new
        temp_281 = temp_280(0, 12)
        temp_275.CornerRadius = temp_281
        temp_284 = Instance.new
        temp_287 = temp_284("UIStroke", temp_221)
        temp_292 = Color3.fromRGB
        temp_293 = temp_292(255, 255, 255)
        temp_287.Color = temp_293
        temp_287.Thickness = 2.5
        temp_300 = Enum.ApplyStrokeMode
        temp_303 = temp_300.Border
        temp_287.ApplyStrokeMode = temp_303
        temp_306 = Instance.new
        temp_309 = temp_306("UIGradient", temp_287)
        temp_310 = {}
        temp_310.value = temp_309
        temp_311 = temp_310.value
        temp_314 = {}
        temp_317 = ColorSequence.new
        temp_320 = ColorSequenceKeypoint.new
        temp_323 = Color3.fromRGB
        temp_324 = {temp_323(0, 0, 0)}
        temp_325 = temp_320(0, unpack_values(temp_324))
        temp_328 = ColorSequenceKeypoint.new
        temp_331 = Color3.fromRGB
        temp_332 = {temp_331(255, 255, 255)}
        temp_333 = temp_328(0.25, unpack_values(temp_332))
        temp_336 = ColorSequenceKeypoint.new
        temp_339 = Color3.fromRGB
        temp_340 = {temp_339(255, 255, 255)}
        temp_341 = temp_336(0.5, unpack_values(temp_340))
        temp_344 = ColorSequenceKeypoint.new
        temp_347 = Color3.fromRGB
        temp_348 = {temp_347(0, 0, 0)}
        temp_349 = temp_344(0.75, unpack_values(temp_348))
        temp_352 = ColorSequenceKeypoint.new
        temp_355 = Color3.fromRGB
        temp_356 = {temp_355(0, 0, 0)}
        temp_357 = {temp_352(1, unpack_values(temp_356))}
        temp_358 = {temp_325, temp_333, temp_341, temp_349, unpack_values(temp_357)}
        temp_359 = temp_317(temp_358)
        temp_311.Color = temp_359
        temp_360 = {}
        temp_360.value = nil
        temp_361 = q.value
        temp_364 = temp_361.RenderStepped
        temp_365 = bind(callbacks.callback_28, {temp_310, u, B, temp_360})
        temp_366 = temp_364.Connect
        temp_367 = temp_366(temp_364, temp_365)
        temp_360.value = temp_367
        temp_370 = bind(callbacks.callback_29, {temp_142, u, B, l, temp_84, temp_360, y, M})
        temp_371 = temp_221.Activated
        temp_372 = temp_371.Connect
        temp_372(temp_371, temp_370)
        return unpack_values(temp_314)
    end
end

return callbacks.main({}, {...})
