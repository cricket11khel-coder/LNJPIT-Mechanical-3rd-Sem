'use client';
import React, { useState } from 'react';

const mechRoutine = {
  Monday: [
    { time: "10:00 - 11:00", subject: "Engineering Mathematics-III (M-III)", code: "102303", faculty: "Prof. Gajendra Nath Tripathi (GNT)" },
    { time: "11:00 - 12:00", subject: "Basic Electronics Engineering (BEE)", code: "102305", faculty: "Prof. Avinash Kumar (AK)" },
    { time: "12:00 - 01:00", subject: "Thermodynamics (TD)", code: "102304", faculty: "Prof. Pankaj Kumar (PK)" },
    { time: "01:00 - 02:00", subject: "LUNCH BREAK", code: "LUNCH", faculty: "-" },
    { time: "02:00 - 03:00", subject: "Universal Human Values (UHV)", code: "102306", faculty: "Prof. Guddi Kumari (GK)" },
    { time: "03:00 - 05:00", subject: "EM Lab / BEE Lab", code: "LAB", faculty: "Prof. Ajit Kumar Chauhan / Mr. Rohit Kumar" }
  ],
  Tuesday: [
    { time: "10:00 - 11:00", subject: "Thermodynamics (TD)", code: "102304", faculty: "Prof. Pankaj Kumar (PK)" },
    { time: "11:00 - 12:00", subject: "Engineering Mathematics-III (M-III)", code: "102303", faculty: "Prof. Gajendra Nath Tripathi (GNT)" },
    { time: "12:00 - 01:00", subject: "Material Science and Engineering (MSE)", code: "102302", faculty: "Prof. Navneet Kumar Singh (NKS)" },
    { time: "01:00 - 02:00", subject: "LUNCH BREAK", code: "LUNCH", faculty: "-" },
    { time: "02:00 - 03:00", subject: "Indian Knowledge System (IKS)", code: "102307", faculty: "Prof. Sachindra Kumar (SK)" },
    { time: "03:00 - 05:00", subject: "Sports", code: "SPORTS", faculty: "-" }
  ],
  Wednesday: [
    { time: "10:00 - 11:00", subject: "Material Science and Engineering (MSE)", code: "102302", faculty: "Prof. Navneet Kumar Singh (NKS)" },
    { time: "11:00 - 12:00", subject: "Engineering Mathematics-III (M-III)", code: "102303", faculty: "Prof. Gajendra Nath Tripathi (GNT)" },
    { time: "12:00 - 01:00", subject: "Engineering Mechanics (EM)", code: "102301", faculty: "Prof. Ajit Kumar Chauhan (AKC)" },
    { time: "01:00 - 02:00", subject: "LUNCH BREAK", code: "LUNCH", faculty: "-" },
    { time: "02:00 - 03:00", subject: "Library / Free Slot", code: "FREE", faculty: "-" },
    { time: "03:00 - 05:00", subject: "Library", code: "LIB", faculty: "-" }
  ],
  Thursday: [
    { time: "10:00 - 11:00", subject: "Engineering Mechanics (EM)", code: "102301", faculty: "Prof. Ajit Kumar Chauhan (AKC)" },
    { time: "11:00 - 12:00", subject: "Basic Electronics Engineering (BEE)", code: "102305", faculty: "Prof. Avinash Kumar (AK)" },
    { time: "12:00 - 01:00", subject: "Indian Knowledge System (IKS)", code: "102307", faculty: "Prof. Sachindra Kumar (SK)" },
    { time: "01:00 - 02:00", subject: "LUNCH BREAK", code: "LUNCH", faculty: "-" },
    { time: "02:00 - 03:00", subject: "Universal Human Values (UHV)", code: "102306", faculty: "Prof. Guddi Kumari (GK)" },
    { time: "03:00 - 05:00", subject: "EM Lab / BEE Lab", code: "LAB", faculty: "Prof. Ajit Kumar Chauhan / Miss Seema Kumari" }
  ],
  Friday: [
    { time: "10:00 - 11:00", subject: "Universal Human Values (UHV)", code: "102306", faculty: "Prof. Guddi Kumari (GK)" },
    { time: "11:00 - 12:00", subject: "Material Science and Engineering (MSE)", code: "102302", faculty: "Prof. Navneet Kumar Singh (NKS)" },
    { time: "12:00 - 01:00", subject: "Engineering Mechanics (EM)", code: "102301", faculty: "Prof. Ajit Kumar Chauhan (AKC)" },
    { time: "01:00 - 02:00", subject: "LUNCH BREAK", code: "LUNCH", faculty: "-" },
    { time: "02:00 - 03:00", subject: "Engineering Mechanics Tutorial (EM-T)", code: "EMT", faculty: "Prof. Ajit Kumar Chauhan (AKC)" },
    { time: "03:00 - 05:00", subject: "Internship-1", code: "102308", faculty: "Prof. Bharti Kumari (BK)" }
  ],
  Saturday: [
    { time: "10:00 - 11:00", subject: "Basic Electronics Engineering (BEE)", code: "102305", faculty: "Prof. Avinash Kumar (AK)" },
    { time: "11:00 - 12:00", subject: "Engineering Mathematics-III (M-III)", code: "102303", faculty: "Prof. Gajendra Nath Tripathi (GNT)" },
    { time: "12:00 - 01:00", subject: "Thermodynamics (TD)", code: "102304", faculty: "Prof. Pankaj Kumar (PK)" },
    { time: "01:00 - 02:00", subject: "LUNCH BREAK", code: "LUNCH", faculty: "-" },
    { time: "02:00 - 03:00", subject: "Indian Knowledge System (IKS)", code: "102307", faculty: "Prof. Sachindra Kumar (SK)" },
    { time: "03:00 - 05:00", subject: "Mentor-Mentee Interaction", code: "MENTOR", faculty: "-" }
  ]
};

export default function MechAttendance() {
  const [selectedDay, setSelectedDay] = useState('Monday');

  return (
    <main style={{ padding: '20px', maxWidth: '800px', margin: '0 auto', fontFamily: 'Inter, sans-serif' }}>
      <header style={{ textAlign: 'center', marginBottom: '20px' }}>
        <h1 style={{ color: '#1e293b', fontSize: '24px' }}>LNJPIT Chapra</h1>
        <p style={{ color: '#64748b' }}>Department of Mechanical Engineering | 3rd Semester (Room No: 04)</p>
      </header>

      <div style={{ display: 'flex', gap: '8px', overflowX: 'auto', marginBottom: '20px', paddingBottom: '5px' }}>
        {Object.keys(mechRoutine).map((day) => (
          <button
            key={day}
            onClick={() => setSelectedDay(day)}
            style={{
              padding: '10px 16px',
              borderRadius: '8px',
              border: 'none',
              cursor: 'pointer',
              fontWeight: '600',
              background: selectedDay === day ? '#2563eb' : '#e2e8f0',
              color: selectedDay === day ? '#ffffff' : '#475569',
              whiteSpace: 'nowrap'
            }}
          >
            {day}
          </button>
        ))}
      </div>

      <div style={{ background: '#f8fafc', padding: '16px', borderRadius: '12px', border: '1px solid #e2e8f0' }}>
        <h2 style={{ fontSize: '18px', color: '#334155', marginBottom: '12px' }}>{selectedDay} Schedule</h2>
        <div style={{ display: 'flex', flexDirection: 'column', gap: '10px' }}>
          {mechRoutine[selectedDay].map((slot, index) => (
            <div 
              key={index} 
              style={{ 
                background: '#ffffff', 
                padding: '12px 16px', 
                borderRadius: '8px', 
                boxShadow: '0 1px 3px rgba(0,0,0,0.05)',
                display: 'flex',
                justifyContent: 'space-between',
                alignItems: 'center',
                flexWrap: 'wrap',
                gap: '8px'
              }}
            >
              <div>
                <span style={{ fontSize: '12px', background: '#e0f2fe', color: '#0369a1', padding: '2px 8px', borderRadius: '4px', fontWeight: 'bold' }}>
                  {slot.time}
                </span>
                <h3 style={{ fontSize: '15px', color: '#0f172a', margin: '6px 0 2px 0' }}>{slot.subject}</h3>
                <p style={{ fontSize: '13px', color: '#64748b', margin: 0 }}>{slot.faculty}</p>
              </div>
              {slot.code !== 'LUNCH' && slot.code !== 'FREE' && (
                <span style={{ fontSize: '12px', background: '#f1f5f9', color: '#475569', padding: '4px 8px', borderRadius: '6px' }}>
                  Code: {slot.code}
                </span>
              )}
            </div>
          ))}
        </div>
      </div>

      <div style={{ textAlign: 'center', marginTop: '30px' }}>
        <a 
          href="/" 
          style={{ color: '#2563eb', textDecoration: 'none', fontWeight: '500', fontSize: '14px' }}
        >
          ← Back to Home
        </a>
      </div>
    </main>
  );
}
