# 🐋 ECOSISTEMA ZYKOS - ARQUITECTURA COMPLETA

## 📋 ESTRUCTURA DEL PROYECTO

```
zykos-ecosystem/
│
├── zykotoken-ar/          # Portal PSYKOSWORLD
│   ├── public/
│   │   └── _redirects
│   ├── src/
│   │   ├── components/
│   │   │   ├── Header.jsx
│   │   │   ├── Footer.jsx
│   │   │   └── BifurcacionRouter.jsx
│   │   ├── pages/
│   │   │   ├── index.html
│   │   │   └── welcome.html
│   │   └── styles/
│   │       └── main.css
│   ├── netlify.toml
│   └── package.json
│
├── zykos-ar/              # Site Pacientes
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── WalletConnect.jsx
│   │   │   ├── BountyCard.jsx
│   │   │   └── Navigation.jsx
│   │   ├── pages/
│   │   │   ├── index.html
│   │   │   ├── bounties.html
│   │   │   └── narrativas.html
│   │   └── styles/
│   │       └── punk.css
│   ├── netlify.toml
│   └── package.json
│
└── docs/
    ├── DNS-SETUP.md
    ├── DEPLOYMENT.md
    └── MEMBERFUL-CONFIG.md
```

---

## 🎯 DOMINIOS Y FUNCIONES

### **1. zykotoken.ar - PSYKOSWORLD (Portal Hub)**
- **Función:** Gateway central con bifurcación inteligente
- **Hosting:** Netlify
- **Features:**
  - Landing page con detección de audiencia
  - Memberful integration
  - Router a zykos.ar o psykotoken.com
  - Sistema de onboarding

### **2. zykos.ar - PACIENTES (ZYK)**
- **Función:** Narrativa pacientes/afectados
- **Hosting:** Netlify
- **Features:**
  - Design punk/disruptivo
  - Wallet connect (MetaMask)
  - Bounties display
  - Community stories
  - Token info accesible

### **3. psykotoken.com - MÉDICOS (PSYKOS)**
- **Función:** Portal profesional/institucional
- **Hosting:** Squarespace (mantener actual)
- **Features:**
  - Clinical backing
  - Research & partnerships
  - Documentación académica
  - NO TOCAR (ya funciona)

---

## 🔧 CONFIGURACIÓN DNS

### **Registros para NIC.ar**

#### **ZYKOS.AR:**
```
Tipo: A
Host: @
Valor: 75.2.60.5
TTL: 3600

Tipo: CNAME
Host: www
Valor: apex-loadbalancer.netlify.com
TTL: 3600
```

#### **ZYKOTOKEN.AR:**
```
Tipo: A
Host: @
Valor: 75.2.60.5
TTL: 3600

Tipo: CNAME
Host: www
Valor: apex-loadbalancer.netlify.com
TTL: 3600
```

---

## 🚀 DEPLOYMENT

### **Opción A: Deploy Manual (Simple)**
1. Crear cuenta en Netlify con: zyko@psykostoken.com
2. Importar repos desde GitHub
3. Click "Deploy" - automático

### **Opción B: Deploy CLI (Avanzado)**
```bash
# Instalar Netlify CLI
npm install -g netlify-cli

# Login
netlify login

# Deploy zykotoken.ar
cd zykotoken-ar
netlify deploy --prod

# Deploy zykos.ar
cd ../zykos-ar
netlify deploy --prod
```

---

## 🎨 DESIGN SYSTEM

### **ZYKOTOKEN.AR (Portal)**
```css
:root {
  --primary: #FF8C00;
  --secondary: #1A1A1A;
  --accent: #FFA500;
  --bg: #000000;
  --text: #FFFFFF;
}
```

### **ZYKOS.AR (Punk)**
```css
:root {
  --punk-orange: #FF6B00;
  --punk-red: #FF0000;
  --bg: #000000;
  --text: #00FF00;
  --glitch: #00FF00;
}
```

---

## 💳 WALLET CONFIGURATION

### **Admin Wallet:**
```
0x6aea80e20849bee22fdc54317ea8ec761ece44f7
```

**Uso:**
- Recibir pagos crypto del merch
- Treasury del ecosistema
- Bounties payments

---

## 📧 MEMBERFUL SETUP

### **Account Info:**
- **Email:** zyko@psykostoken.com
- **Site:** zykosworld

### **Plans:**
```
1. Community Member (FREE)
   - Acceso básico a tropos
   - Forum access
   - Basic bounties

2. ZYKOS Patron ($10/month)
   - Todo lo anterior +
   - Exclusive content
   - Priority bounties
   - Governance voting

3. Professional ($25/month)
   - Todo lo anterior +
   - Access a psykotoken.com research
   - Clinical data
   - Networking events
```

---

## 🔐 CREDENCIALES

### **NIC.ar:**
- Email: gonzaloperezcortizo@gmail.com
- Pass: Estudio1859 o Estudio5918

### **GitHub:**
- Repos: Públicos (sin necesidad de login para ver)

### **Netlify:**
- Crear con: zyko@psykostoken.com
- Deploy automático desde GitHub

---

## 📊 ROADMAP

### **Fase 1: Infraestructura (HOY)**
- [x] Arquitectura definida
- [ ] Repos GitHub creados
- [ ] Código base generado
- [ ] DNS configurado

### **Fase 2: Deploy (MAÑANA)**
- [ ] Sites en Netlify
- [ ] SSL/TLS activo
- [ ] Cross-linking funcional

### **Fase 3: Features (PRÓXIMOS DÍAS)**
- [ ] Memberful integration
- [ ] Wallet connect
- [ ] Bounties system
- [ ] Analytics (Plausible)

---

## 🆘 SOPORTE

### **Si algo falla:**

1. **DNS no propaga:**
   - Esperar 24-48h
   - Verificar en: https://dnschecker.org

2. **Netlify deploy error:**
   - Check build logs
   - Contactar: support@netlify.com

3. **Memberful issues:**
   - Docs: https://memberful.com/help

---

## 🔗 LINKS ÚTILES

- **Netlify Docs:** https://docs.netlify.com
- **NIC.ar Panel:** https://nic.ar
- **GitHub Repos:** (se generarán y compartirán)
- **Memberful Dashboard:** https://zykosworld.memberful.com

---

## ✅ CHECKLIST FINAL

```
☐ DNS configurado en NIC.ar
☐ Repos GitHub públicos creados
☐ Netlify sites deployados
☐ SSL/TLS activo
☐ Memberful account creado
☐ Wallet configurada
☐ Cross-site navigation funcional
☐ Analytics instalado
☐ Testing completo
☐ Documentación entregada
```

---

**Última actualización:** 2025-01-11
**Contacto:** zyko@psykostoken.com
**Wallet:** 0x6aea80e20849bee22fdc54317ea8ec761ece44f7