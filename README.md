# Config_Oh-My-Posh

Claro! Aqui vai um **resumo direto e tranquilo** de como **baixar**, **usar** e **escolher temas** no **Oh My Posh** no **PowerShell 7**:

---

### ✅ **1. Baixar e instalar o Oh My Posh**

1. **Abra o PowerShell 7 como Administrador**.
2. Digite o seguinte comando para instalar:
   ```powershell
   winget install JanDeDobbeleer.OhMyPosh -s winget
   ```

> Se não tiver o `winget`, você pode baixar manualmente em:  
[https://ohmyposh.dev/docs/windows](https://ohmyposh.dev/docs/windows)

---

### ✅ **2. Instalar uma fonte Nerd Font (para ícones bonitos)**

1. Baixe uma fonte Nerd Font (exemplo: [Caskaydia Cove Nerd Font](https://www.nerdfonts.com/font-downloads)).
2. Instale a fonte (dê dois cliques no `.ttf` e clique em "Instalar").
3. No PowerShell 7, clique com o botão direito na barra superior → **Propriedades** → **Fonte**, e selecione a fonte instalada.

---

### ✅ **3. Ativar o Oh My Posh no PowerShell**

1. Abra o PowerShell 7.
2. Execute:
   ```powershell
   notepad $PROFILE
   ```
3. No arquivo que abrir, adicione:
   ```powershell
   oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\jandedobbeleer.omp.json" | Invoke-Expression
   ```

> Esse exemplo usa o tema `jandedobbeleer`. Você pode trocar o nome por outro (veja abaixo como).

---

### ✅ **4. Ver temas disponíveis e testar**

- Para **ver os temas instalados**:
  ```powershell
  Get-PoshThemes
  ```

- Para **testar um tema temporariamente**:
  ```powershell
  oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\<nome-do-tema>.omp.json" | Invoke-Expression
  ```

> Exemplo:
```powershell
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\paradox.omp.json" | Invoke-Expression
```

---

### ✅ **5. Salvar um tema como padrão**

1. No `notepad $PROFILE`, troque a linha do tema pelo nome do seu preferido:
   ```powershell
   oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\paradox.omp.json" | Invoke-Expression
   ```

---

Acessem esse conteúdo do Youtube : https://youtu.be/6SGIFVJ5Izs?si=W4G4NJ8R0Ue00-RH
