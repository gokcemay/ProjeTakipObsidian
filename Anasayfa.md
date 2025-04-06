Bu sayfa sizin başlangıç sayfanız. Bu sayfayı kullanarak günlük yapacaklarınızı ve takip edilen aktif projelerin ya da toplantıların listesine ulaşmanız mümkün. Ayrıca **Hızlı Ekleme** tuşları ile *Yeni Kurum*, *Yeni Kişi* ve *Yeni Proje* ekleyebilirsiniz. Unutmayın [[Kullanım notları]] hemen elinizin altında.

## Bugünün Görevleri
```tasks
not done
due today

```

---
## Yakın Görevler
```tasks
not done
due AFTER yesterday
due BEFORE in two weeks
```
---
## Hızlı Ekleme
 `BUTTON[yeni-kurum, yeni-kisi, yeni-proje]`
```meta-bind-button
style: primary
label: Yeni Kurum
id: yeni-kurum
hidden: true
actions:
- type: templaterCreateNote 
  templateFile: "Kurum Şablonu 1.md" 
  folderPath: "20 Kişiler ve Kurumlar" 
  fileName: Yeni Kurum
- type: open
  link: Yeni Kurum.md
```
```meta-bind-button
style: destructive
label: Yeni Kişi
id: yeni-kisi
hidden: True
actions:
- type: templaterCreateNote 
  templateFile: "00 Meta/02 Şablonlar/Kişi şablonu.md" 
  folderPath: "20 Kişiler ve Kurumlar" 
  fileName: Yeni Kişi
- type: open
  link: Yeni Kişi.md
```

![[Aktif Projeler Listesi]]
```meta-bind-button
style: default
label: Yeni Proje
id: yeni-proje
hidden: True
actions:
- type: templaterCreateNote 
  templateFile: "00 Meta/02 Şablonlar/Kişi şablonu.md" 
  folderPath: "20 Kişiler ve Kurumlar" 
  fileName: Yeni Kişi
- type: open
  link: Yeni Proje.md
```

```meta-bind-button
style: destructive
label: Light Mode
id: light-mode
hidden: true
actions:
  - type: command
    command: theme:use-light
```

```meta-bind-button
style: primary
label: Dark Mode
id: dark-mode
hidden: true
actions:
  - type: command
    command: theme:use-dark
```
![[Toplantılar listesi]]