```aura width=860 height=220
<div style={{
  width: '100%', height: '100%', background: '#0d0d14',
  display: 'flex', alignItems: 'center', fontFamily: 'Inter',
  position: 'relative', overflow: 'hidden', borderRadius: 16,
  border: '1px solid rgba(186,225,255,0.18)'
}}>
  <style>{`
    @keyframes drift-a { 0%,100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(320px); opacity: 1; } }
    @keyframes drift-b { 0%,100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-260px); opacity: 1; } }
    @keyframes drift-c { 0%,100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.3); opacity: 0.45; } }
    #orb-1 { animation: drift-a 10s ease-in-out infinite; }
    #orb-2 { animation: drift-b 13s ease-in-out infinite; }
    #orb-3 { animation: drift-a 12s ease-in-out infinite reverse; }
    #orb-4 { animation: drift-b 9s ease-in-out infinite reverse; }
    #orb-5 { animation: drift-c 7s ease-in-out infinite; }
  `}</style>

  <svg width="860" height="220" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="p1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(255,179,186,0.55)" />
        <stop offset="70%" stopColor="rgba(255,179,186,0)" />
      </radialGradient>
      <radialGradient id="p2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(255,223,186,0.45)" />
        <stop offset="70%" stopColor="rgba(255,223,186,0)" />
      </radialGradient>
      <radialGradient id="p3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(186,255,201,0.38)" />
        <stop offset="70%" stopColor="rgba(186,255,201,0)" />
      </radialGradient>
      <radialGradient id="p4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(186,225,255,0.5)" />
        <stop offset="70%" stopColor="rgba(186,225,255,0)" />
      </radialGradient>
      <radialGradient id="p5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(255,255,186,0.3)" />
        <stop offset="70%" stopColor="rgba(255,255,186,0)" />
      </radialGradient>
    </defs>
    <ellipse id="orb-1" cx="160" cy="250" rx="250" ry="170" fill="url(#p1)" />
    <ellipse id="orb-2" cx="420" cy="250" rx="220" ry="160" fill="url(#p4)" />
    <ellipse id="orb-3" cx="300" cy="260" rx="200" ry="150" fill="url(#p2)" />
    <ellipse id="orb-4" cx="640" cy="250" rx="180" ry="140" fill="url(#p3)" />
    <ellipse id="orb-5" cx="760" cy="240" rx="140" ry="110" fill="url(#p5)" />
  </svg>

  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 56, gap: 10 }}>
    <div style={{ display: 'flex', fontSize: 52, fontWeight: 800, color: '#ffffff', letterSpacing: '-1.5px', lineHeight: 1 }}>
      Andres Jara
    </div>
    <div style={{ display: 'flex', fontSize: 17, color: 'rgba(255,223,186,0.9)', letterSpacing: '4px' }}>
      BACKEND · ARCHITECTURE · SYSTEM DESIGN
    </div>
    <div style={{ display: 'flex', gap: 8, marginTop: 10 }}>
      {['Systems Engineering student', 'Costa Rica', 'Open to learn'].map(function(tag, i) {
        return (
          <div key={tag + '-' + i} style={{
            display: 'flex', padding: '5px 14px', borderRadius: 20, fontSize: 12,
            color: 'rgba(255,255,255,0.85)', background: 'rgba(255,255,255,0.07)',
            border: '1px solid rgba(255,255,255,0.14)'
          }}>{tag}</div>
        );
      })}
    </div>
  </div>
</div>
```

```aura width=860 height=190
<div style={{
  width: '100%', height: '100%', background: '#0d0d14', display: 'flex',
  alignItems: 'center', fontFamily: 'Inter', borderRadius: 16,
  border: '1px solid rgba(186,255,201,0.16)', padding: '0 40px'
}}>
  <div style={{ display: 'flex', flexDirection: 'column', width: 470, gap: 10 }}>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: '4px', color: 'rgba(186,255,201,0.8)' }}>ABOUT ME</div>
    <div style={{ display: 'flex', fontSize: 15, lineHeight: 1.5, color: 'rgba(255,255,255,0.85)' }}>
      I'm a Systems Engineering student in Costa Rica focused on backend development, software architecture and system design.
    </div>
    <div style={{ display: 'flex', fontSize: 13, color: 'rgba(255,255,255,0.5)' }}>
      Always improving myself in new topics.
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', marginLeft: 40, gap: 10, flex: 1 }}>
    <div style={{ display: 'flex', fontSize: 12, letterSpacing: '4px', color: 'rgba(255,179,186,0.8)' }}>CURRENTLY LEARNING</div>
    <div style={{ display: 'flex', flexWrap: 'wrap', gap: 8 }}>
      {['PHP', 'MySQL', 'Docker', 'MongoDB', 'JavaScript', 'Security'].map(function(t, i) {
        return (
          <div key={t + '-' + i} style={{
            display: 'flex', padding: '5px 12px', borderRadius: 16, fontSize: 12,
            color: '#ffffff', background: 'rgba(255,179,186,0.12)',
            border: '1px solid rgba(255,179,186,0.35)'
          }}>{t}</div>
        );
      })}
    </div>
  </div>
</div>
```

```aura width=860 height=250
<div style={{
  width: '100%', height: '100%', background: '#0d0d14', display: 'flex',
  flexDirection: 'column', justifyContent: 'center', gap: 16, fontFamily: 'Inter',
  borderRadius: 16, border: '1px solid rgba(255,255,186,0.16)', padding: '0 40px'
}}>
  <div style={{ display: 'flex', fontSize: 12, letterSpacing: '4px', color: 'rgba(255,255,186,0.8)' }}>STACK</div>
  {[
    { label: 'Languages', color: '255,179,186', items: ['PHP', 'C++', 'C#', 'HTML', 'CSS', 'Java'] },
    { label: 'Tools', color: '186,225,255', items: ['Git', 'VS Code', 'Azure', 'React', 'Docker', 'Node.js'] },
    { label: 'Databases', color: '186,255,201', items: ['MySQL', 'MongoDB', 'Supabase'] },
  ].map(function(row, i) {
    return (
      <div key={row.label + '-' + i} style={{ display: 'flex', alignItems: 'center', gap: 12 }}>
        <div style={{ display: 'flex', width: 90, fontSize: 13, color: 'rgba(255,255,255,0.55)' }}>{row.label}</div>
        {row.items.map(function(t, j) {
          return (
            <div key={t + '-' + j} style={{
              display: 'flex', padding: '5px 14px', borderRadius: 16, fontSize: 12, color: '#ffffff',
              background: 'rgba(' + row.color + ',0.1)', border: '1px solid rgba(' + row.color + ',0.4)'
            }}>{t}</div>
          );
        })}
      </div>
    );
  })}
</div>
```

```aura width=860 height=220
<div style={{ width: '100%', height: '100%', display: 'flex', gap: 20, fontFamily: 'Inter' }}>
  {[
    { name: 'Quiniela-App', size: 21, color: '255,179,186', desc: 'Scalable RESTful API with a clean architecture.', tags: ['Node.js', 'Express', 'SQL Server 2022'] },
    { name: 'Proyecto-Redes-Web', size: 19, color: '186,225,255', desc: 'Microservices with Docker and orchestration.', tags: ['Docker', 'Kubernetes', 'Python'] },
    { name: 'Microservices-api-gateway', size: 16, color: '186,255,201', desc: 'API Gateway with JWT auth and async messaging.', tags: ['MySQL', 'Docker', 'Redis', 'RabbitMQ'] },
  ].map(function(p, i) {
    return (
      <div key={p.name} style={{
        display: 'flex', flexDirection: 'column', justifyContent: 'space-between', flex: 1, height: '100%',
        background: '#0d0d14', borderRadius: 16, padding: 22, border: '1px solid rgba(' + p.color + ',0.3)'
      }}>
        <div style={{ display: 'flex', flexDirection: 'column', gap: 8 }}>
          <div style={{ display: 'flex', fontSize: 11, letterSpacing: '3px', color: 'rgba(' + p.color + ',0.85)' }}>PROJECT</div>
          <div style={{ display: 'flex', fontSize: p.size, fontWeight: 800, color: '#ffffff' }}>{p.name}</div>
          <div style={{ display: 'flex', fontSize: 13, lineHeight: 1.4, color: 'rgba(255,255,255,0.65)' }}>{p.desc}</div>
        </div>
        <div style={{ display: 'flex', flexWrap: 'wrap', gap: 6 }}>
          {p.tags.map(function(t, j) {
            return <div key={t + '-' + j} style={{ display: 'flex', padding: '3px 10px', borderRadius: 12, fontSize: 11, color: '#fff', background: 'rgba(' + p.color + ',0.14)' }}>{t}</div>;
          })}
        </div>
      </div>
    );
  })}
</div>
```
