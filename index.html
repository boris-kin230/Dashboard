<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Conformité CILT - Heineken</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- React & ReactDOM -->
    <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <!-- Babel pour JSX -->
    <script crossorigin src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <style>
        /* Ajout de styles personnalisés si nécessaire pour les scrollbars par exemple */
        ::-webkit-scrollbar {
            width: 8px;
            height: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1; 
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd5e1; 
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #94a3b8; 
        }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        const { useState, useEffect } = React;

        // ==========================================
        // 0. ICÔNES (Remplacement de lucide-react par des SVG natifs)
        // ==========================================
        const Star = ({ className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon>
            </svg>
        );

        const Trophy = ({ className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <path d="M6 9H4.5a2.5 2.5 0 0 1 0-5H6"></path>
                <path d="M18 9h1.5a2.5 2.5 0 0 0 0-5H18"></path>
                <path d="M4 22h16"></path>
                <path d="M10 14.66V17c0 .55-.47.98-.97 1.21C7.85 18.75 7 20.24 7 22"></path>
                <path d="M14 14.66V17c0 .55.47.98.97 1.21C16.15 18.75 17 20.24 17 22"></path>
                <path d="M18 2H6v7a6 6 0 0 0 12 0V2Z"></path>
            </svg>
        );

        const Medal = ({ className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <path d="M7.21 15 2.66 7.14a2 2 0 0 1 .13-2.2L4.4 2.8A2 2 0 0 1 6 2h12a2 2 0 0 1 1.6.8l1.6 2.14a2 2 0 0 1 .14 2.2L16.79 15"></path>
                <path d="M11 12 5.12 2.2"></path>
                <path d="m13 12 5.88-9.8"></path>
                <path d="M8 7h8"></path>
                <circle cx="12" cy="17" r="5"></circle>
                <path d="M12 18v-2h-.5"></path>
            </svg>
        );

        const AlertCircle = ({ className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <circle cx="12" cy="12" r="10"></circle>
                <line x1="12" y1="8" x2="12" y2="12"></line>
                <line x1="12" y1="16" x2="12.01" y2="16"></line>
            </svg>
        );

        const MessageSquare = ({ className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                <path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path>
            </svg>
        );

        const IconCheck = () => (
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className="w-5 h-5 text-green-600 bg-green-100 rounded-full p-0.5">
                <path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path>
                <polyline points="22 4 12 14.01 9 11.01"></polyline>
            </svg>
        );

        const IconX = () => (
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className="w-5 h-5 text-red-600 bg-red-100 rounded-full p-0.5">
                <circle cx="12" cy="12" r="10"></circle>
                <line x1="15" y1="9" x2="9" y2="15"></line>
                <line x1="9" y1="9" x2="15" y2="15"></line>
            </svg>
        );

        // ==========================================
        // 1. MOCK DATA (SIMULATION DE BASE DE DONNÉES)
        // ==========================================
        const DEFAULT_EQUIPMENTS = {
          "DEPAL 8/9": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ],
          "SOUTIREUSE 8/9": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ],
          "ETIQUETEUSE 8/9": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ],
          "QF1/PARKER/CERMEX": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ],
          "DUO1": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ],
          "OCME": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ],
          "PAL/MSK": [
            { quart: "Matin", real: true, taux: 100 },
            { quart: "Après-midi", real: true, taux: 100 },
            { quart: "Nuit", real: true, taux: 100 }
          ]
        };

        const DAILY_DATA = {
          "17/03/2026": {
            globalRate: 85,
            equipments: {
              ...DEFAULT_EQUIPMENTS,
              "ETIQUETEUSE 8/9": [
                { quart: "Matin", real: true, taux: 100 },
                { quart: "Après-midi", real: true, taux: 96 },
                { quart: "Nuit", real: true, taux: 100 }
              ],
              "QF1/PARKER/CERMEX": [
                { quart: "Matin", real: true, taux: 100 },
                { quart: "Après-midi", real: false, taux: 0 },
                { quart: "Nuit", real: true, taux: 100 }
              ],
              "DUO1": [
                { quart: "Matin", real: false, taux: 0 },
                { quart: "Après-midi", real: false, taux: 0 },
                { quart: "Nuit", real: false, taux: 0 }
              ],
              "PAL/MSK": [
                { quart: "Matin", real: true, taux: 100 },
                { quart: "Après-midi", real: true, taux: 94 },
                { quart: "Nuit", real: true, taux: 100 }
              ]
            },
            tasks: [
              { id: 1, name: "MARS CDT CILT G8/9 PAL 1, 2, 3, MSK Journalier", points: "1.3 Mousser les sols de la zone 15mns et les rincer", comment: "Raison : juste à l'eau" },
              { id: 2, name: "MARS CDT SS CILT JOURNALIER ETIQUETEUSE CLA/CLB/CLC G8/G9", points: "2.5 Les verniers sont-ils tous au standard (0) ?", comment: "Raison : usure poste" },
              { id: 3, name: "MARS CDT CILT G89 OCME Journalier", points: "Purger les bacs à colle", comment: "" }
            ]
          },
          "16/03/2026": {
            globalRate: 62,
            equipments: {
              ...DEFAULT_EQUIPMENTS,
              "DEPAL 8/9": [
                { quart: "Matin", real: true, taux: 100 },
                { quart: "Après-midi", real: false, taux: 50 },
                { quart: "Nuit", real: true, taux: 100 }
              ],
              "SOUTIREUSE 8/9": [
                { quart: "Matin", real: true, taux: 100 },
                { quart: "Après-midi", real: true, taux: 100 },
                { quart: "Nuit", real: false, taux: 80 }
              ],
              "DUO1": [
                { quart: "Matin", real: true, taux: 100 },
                { quart: "Après-midi", real: true, taux: 90 },
                { quart: "Nuit", real: false, taux: 40 }
              ],
              "OCME": [
                { quart: "Matin", real: false, taux: 60 },
                { quart: "Après-midi", real: true, taux: 100 },
                { quart: "Nuit", real: true, taux: 100 }
              ]
            },
            tasks: [
              { id: 4, name: "Maintenance préventive SOUTIREUSE", points: "Vérification des filtres", comment: "Filtre B remplacé en urgence" }
            ]
          },
          "15/03/2026": {
            globalRate: 98,
            equipments: {
              ...DEFAULT_EQUIPMENTS,
              "PAL/MSK": [
                { quart: "Matin", real: false, taux: 70 },
                { quart: "Après-midi", real: true, taux: 100 },
                { quart: "Nuit", real: true, taux: 100 }
              ]
            },
            tasks: []
          }
        };

        const ANNUAL_DATA = {
          rankings: [
            { team: "Équipe C", score: 92.6, rank: 1, color: "bg-yellow-400", textColor: "text-yellow-900", borderColor: "border-yellow-500" },
            { team: "Équipe D", score: 90.0, rank: 2, color: "bg-gray-300", textColor: "text-gray-800", borderColor: "border-gray-400" },
            { team: "Équipe A", score: 89.8, rank: 3, color: "bg-orange-300", textColor: "text-orange-900", borderColor: "border-orange-500" }
          ],
          table: [
            { name: "Équipe A", heures: 88, rangements: 87, map: 98, reunion: 86, nettoyage: 88, total: 88 },
            { name: "Équipe B", heures: 82, rangements: 90, map: 88, reunion: 80, nettoyage: 82, total: 81 },
            { name: "Équipe C", heures: 91, rangements: 95, map: 99, reunion: 93, nettoyage: 91, total: 94 },
            { name: "Équipe D", heures: 90, rangements: 89, map: 96, reunion: 87, nettoyage: 88, total: 90 }
          ],
          chart: {
            months: ["Janvier", "Février", "Mars"],
            series: [
              { name: "Équipe A", color: "#3b82f6", data: [88, 89, 89.8] },
              { name: "Équipe B", color: "#8b5cf6", data: [82, 85, 81] },
              { name: "Équipe C", color: "#f97316", data: [90, 91.5, 92.6] },
              { name: "Équipe D", color: "#0ea5e9", data: [86, 90, 90] }
            ]
          }
        };

        // ==========================================
        // 2. COMPOSANTS GRAPHIQUES (SVG SÉCURISÉS)
        // ==========================================

        // Jauge SVG Parfaite
        const GaugeChart = ({ value = 0 }) => {
          const radius = 70;
          const strokeWidth = 18;
          const circumference = Math.PI * radius;
          const safeValue = Math.min(Math.max(value, 0), 100);
          const strokeDashoffset = circumference - (safeValue / 100) * circumference;

          let color = "#16a34a"; // Vert
          if (safeValue < 80) color = "#dc2626"; // Rouge
          else if (safeValue < 95) color = "#f59e0b"; // Orange

          return (
            <div className="relative flex flex-col items-center justify-center w-full py-2">
              <svg width="220" height="120" viewBox="0 0 200 110">
                <path d="M 20 100 A 80 80 0 0 1 180 100" fill="none" stroke="#e5e7eb" strokeWidth={strokeWidth} strokeLinecap="round" />
                <path
                  d="M 20 100 A 80 80 0 0 1 180 100"
                  fill="none"
                  stroke={color}
                  strokeWidth={strokeWidth}
                  strokeLinecap="round"
                  strokeDasharray={circumference}
                  strokeDashoffset={strokeDashoffset}
                  className="transition-all duration-1000 ease-out"
                />
              </svg>
              <div className="absolute top-[55%] left-1/2 transform -translate-x-1/2 -translate-y-1/2 flex flex-col items-center">
                <span className="text-4xl font-black text-gray-800 tracking-tighter">{safeValue}%</span>
              </div>
              <div className="absolute bottom-2 left-8 text-xs font-bold text-gray-400">0%</div>
              <div className="absolute bottom-2 right-8 text-xs font-bold text-gray-400">100%</div>
            </div>
          );
        };

        // Graphique en ligne SVG (LineChart)
        const LineChart = ({ data }) => {
          if (!data || !data.series) return null;

          const width = 500;
          const height = 220;
          const paddingX = 40;
          const paddingY = 20;
          
          const minY = 80;
          const maxY = 100;
          const rangeY = maxY - minY;

          const getX = (index) => paddingX + (index * ((width - 2 * paddingX) / (data.months.length - 1)));
          const getY = (value) => height - paddingY - (((value - minY) / rangeY) * (height - 2 * paddingY));

          return (
            <div className="w-full flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow-sm p-4 h-full">
              <h3 className="font-bold text-gray-700 mb-2">Tendance de Conformité</h3>
              
              <div className="flex flex-wrap justify-center gap-4 mb-2 text-xs font-semibold">
                {data.series.map((s, i) => (
                  <div key={i} className="flex items-center gap-1">
                    <div className="w-3 h-3 rounded-full shadow-sm" style={{ backgroundColor: s.color }}></div>
                    <span className="text-gray-600">{s.name}</span>
                  </div>
                ))}
              </div>

              <div className="w-full overflow-x-auto flex justify-center">
                <svg width={width} height={height} viewBox={`0 0 ${width} ${height}`} className="max-w-full">
                  {[80, 85, 90, 95, 100].map(val => (
                    <g key={val}>
                      <text x="5" y={getY(val) + 4} fontSize="10" fill="#9ca3af" fontWeight="bold">{val}%</text>
                      <line x1={paddingX} y1={getY(val)} x2={width - paddingX} y2={getY(val)} stroke="#f3f4f6" strokeDasharray="4 4" />
                    </g>
                  ))}

                  {data.months.map((month, i) => (
                    <text key={i} x={getX(i)} y={height - 2} fontSize="11" fill="#6b7280" textAnchor="middle" fontWeight="bold">{month}</text>
                  ))}

                  {data.series.map((serie, sIdx) => {
                    const pathD = serie.data.map((val, i) => `${i === 0 ? 'M' : 'L'} ${getX(i)} ${getY(val)}`).join(" ");
                    return (
                      <g key={sIdx}>
                        <path d={pathD} fill="none" stroke={serie.color} strokeWidth="3" strokeLinejoin="round" className="drop-shadow-sm" />
                        {serie.data.map((val, i) => (
                          <circle key={i} cx={getX(i)} cy={getY(val)} r="4" fill={serie.color} stroke="#fff" strokeWidth="2" />
                        ))}
                      </g>
                    );
                  })}
                </svg>
              </div>
            </div>
          );
        };

        // ==========================================
        // 3. VUES ET COMPOSANTS D'INTERFACE
        // ==========================================

        const EquipmentTable = ({ title, data = [] }) => {
          return (
            <div className="border border-gray-400 bg-white shadow-sm flex flex-col h-full">
              <div className="bg-[#f498c0] text-center font-bold text-gray-900 border-b border-gray-400 py-1 uppercase text-xs sm:text-sm shadow-inner">
                {title}
              </div>
              <div className="flex-grow overflow-auto">
                <table className="w-full text-xs sm:text-sm">
                  <thead className="bg-white border-b border-gray-300">
                    <tr>
                      <th className="text-left font-semibold text-green-700 px-2 py-1.5 w-1/2 border-r border-gray-300">Quart</th>
                      <th className="font-semibold text-green-700 px-2 py-1.5 border-r border-gray-300 text-center">Réal</th>
                      <th className="font-semibold text-green-700 px-2 py-1.5 text-center">Taux</th>
                    </tr>
                  </thead>
                  <tbody>
                    {data.map((row, index) => (
                      <tr key={index} className="border-b border-gray-200 last:border-none hover:bg-gray-50">
                        <td className="px-2 py-1.5 border-r border-gray-300 font-medium text-gray-700">{row.quart}</td>
                        <td className="px-2 py-1.5 border-r border-gray-300 text-center flex justify-center items-center">
                          {row.real ? <IconCheck /> : <IconX />}
                        </td>
                        <td className="px-2 py-1.5 text-center font-bold text-gray-800">
                          {row.taux > 0 ? `${row.taux} %` : ''}
                        </td>
                      </tr>
                    ))}
                  </tbody>
                </table>
              </div>
            </div>
          );
        };

        const JournalierView = ({ selectedDate, setSelectedDate }) => {
          const currentData = DAILY_DATA[selectedDate] || DAILY_DATA[Object.keys(DAILY_DATA)[0]];
          const equipmentsList = ["SOUTIREUSE 8/9", "ETIQUETEUSE 8/9", "QF1/PARKER/CERMEX", "DUO1", "OCME", "PAL/MSK"];

          return (
            <div className="flex flex-col lg:flex-row gap-4 p-4 bg-gray-100 h-full overflow-y-auto">
              
              <div className="flex flex-col gap-4 w-full lg:w-2/3">
                
                <div className="flex flex-col sm:flex-row gap-4">
                  <div className="bg-white border border-gray-800 shadow-sm w-full sm:w-48 flex-shrink-0 flex flex-col">
                    <div className="bg-gray-200 border-b border-gray-300 px-3 py-1.5 font-bold text-sm text-gray-800 uppercase tracking-wide">
                      Historiques
                    </div>
                    <div className="p-2 flex flex-col gap-1 overflow-y-auto">
                      <div className="flex items-center gap-2 font-bold bg-gray-100 p-1.5 rounded mb-1 border border-gray-200">
                        <div className="w-3 h-3 bg-black rounded-sm"></div> DCS J
                      </div>
                      {Object.keys(DAILY_DATA).map(date => (
                        <label key={date} className={`flex items-center gap-2 cursor-pointer p-1.5 rounded transition-colors ${selectedDate === date ? 'bg-green-50 border border-green-200' : 'hover:bg-gray-50'}`}>
                          <input 
                            type="radio" 
                            name="historyDate"
                            checked={selectedDate === date} 
                            onChange={() => setSelectedDate(date)}
                            className="w-4 h-4 text-green-600 focus:ring-green-500 cursor-pointer"
                          />
                          <span className={`text-sm ${selectedDate === date ? "font-bold text-green-800" : "text-gray-700"}`}>
                            {date}
                          </span>
                        </label>
                      ))}
                      <label className="flex items-center gap-2 cursor-not-allowed opacity-40 p-1.5">
                        <input type="radio" disabled className="w-4 h-4" />
                        <span className="text-sm">14/03/2026</span>
                      </label>
                    </div>
                  </div>

                  <div className="flex flex-col sm:flex-row gap-4 flex-grow">
                    <div className="flex-1 border border-gray-800 bg-white shadow-sm flex flex-col">
                      <div className="bg-[#f498c0] text-center font-bold text-gray-900 border-b border-gray-800 py-1 uppercase text-sm">
                        CONFORMITÉ GLOBAL
                      </div>
                      <div className="flex-grow flex items-center justify-center p-2">
                        <GaugeChart value={currentData.globalRate} />
                      </div>
                    </div>
                    <div className="flex-1">
                      <EquipmentTable title="DEPAL 8/9" data={currentData.equipments["DEPAL 8/9"] || []} />
                    </div>
                  </div>
                </div>

                <div className="grid grid-cols-1 sm:grid-cols-2 xl:grid-cols-3 gap-4">
                  {equipmentsList.map(eq => (
                    <EquipmentTable key={eq} title={eq} data={currentData.equipments[eq] || []} />
                  ))}
                </div>

              </div>

              <div className="w-full lg:w-1/3 bg-white border border-gray-800 shadow-sm flex flex-col overflow-hidden">
                <div className="overflow-x-auto overflow-y-auto h-full">
                  <table className="w-full text-sm text-left min-w-[400px]">
                    <thead className="bg-gray-100 border-b-2 border-green-600 sticky top-0">
                      <tr>
                        <th className="px-3 py-2 font-bold text-green-800 border-r border-gray-300 w-12 text-center">id</th>
                        <th className="px-3 py-2 font-bold text-green-800 border-r border-gray-300 w-1/3">Tâches</th>
                        <th className="px-3 py-2 font-bold text-green-800 border-r border-gray-300 w-1/3">Points non conforme</th>
                        <th className="px-3 py-2 font-bold text-green-800">Commentaires</th>
                      </tr>
                    </thead>
                    <tbody>
                      {currentData.tasks && currentData.tasks.length > 0 ? (
                        currentData.tasks.map((task, idx) => (
                          <tr key={idx} className="border-b border-gray-200 hover:bg-blue-50 transition-colors">
                            <td className="px-2 py-3 border-r border-gray-200 align-top text-gray-500 text-center font-mono">{task.id}</td>
                            <td className="px-3 py-3 border-r border-gray-200 align-top text-gray-800 font-semibold text-xs leading-tight">{task.name}</td>
                            <td className="px-3 py-3 border-r border-gray-200 align-top text-gray-600 text-xs">{task.points}</td>
                            <td className="px-3 py-3 align-top text-gray-600 text-xs">
                              {task.comment && (
                                <div className="flex items-start gap-1 bg-yellow-50 p-1.5 border border-yellow-100 rounded">
                                  <MessageSquare className="w-3.5 h-3.5 mt-0.5 text-blue-500 flex-shrink-0" />
                                  <span className="italic font-medium">{task.comment}</span>
                                </div>
                              )}
                            </td>
                          </tr>
                        ))
                      ) : (
                        <tr>
                          <td colSpan="4" className="text-center py-12 text-gray-400">
                            <div className="flex flex-col items-center gap-2">
                              <IconCheck />
                              <span>Aucune non-conformité signalée pour cette date.</span>
                            </div>
                          </td>
                        </tr>
                      )}
                    </tbody>
                  </table>
                </div>
              </div>

            </div>
          );
        };

        const AnnuelView = () => {
          return (
            <div className="flex flex-col gap-8 h-full p-4 sm:p-6 bg-gray-50 overflow-y-auto">
              
              <div className="flex justify-center items-end gap-2 sm:gap-6 h-40 pt-10">
                <div className={`w-28 sm:w-40 h-28 ${ANNUAL_DATA.rankings[1].color} shadow-lg rounded-t-xl flex flex-col items-center justify-end pb-2 relative border-t-4 ${ANNUAL_DATA.rankings[1].borderColor}`}>
                  <div className="absolute -top-12 flex flex-col items-center">
                    <Medal className="w-10 h-10 text-gray-500 drop-shadow-md mb-1" />
                    <span className="font-black text-gray-800 bg-white px-2.5 py-0.5 rounded-full shadow border border-gray-200 text-xs">2ème</span>
                  </div>
                  <span className={`font-black text-sm sm:text-lg ${ANNUAL_DATA.rankings[1].textColor} text-center leading-tight`}>
                    {ANNUAL_DATA.rankings[1].team}<br/>{ANNUAL_DATA.rankings[1].score}%
                  </span>
                </div>
                
                <div className={`w-32 sm:w-48 h-36 ${ANNUAL_DATA.rankings[0].color} shadow-xl rounded-t-xl flex flex-col items-center justify-end pb-4 relative border-t-4 ${ANNUAL_DATA.rankings[0].borderColor} z-10`}>
                   <div className="absolute -top-14 flex flex-col items-center">
                    <Trophy className="w-12 h-12 text-yellow-600 drop-shadow-md mb-1" />
                    <span className="font-black text-yellow-800 bg-white px-3.5 py-1 rounded-full shadow border border-yellow-200 text-sm">1er</span>
                  </div>
                  <span className={`font-black text-base sm:text-xl ${ANNUAL_DATA.rankings[0].textColor} text-center leading-tight`}>
                     {ANNUAL_DATA.rankings[0].team}<br/>{ANNUAL_DATA.rankings[0].score}%
                  </span>
                </div>

                <div className={`w-28 sm:w-40 h-24 ${ANNUAL_DATA.rankings[2].color} shadow-lg rounded-t-xl flex flex-col items-center justify-end pb-2 relative border-t-4 ${ANNUAL_DATA.rankings[2].borderColor}`}>
                  <div className="absolute -top-12 flex flex-col items-center">
                    <Medal className="w-10 h-10 text-orange-600 drop-shadow-md mb-1" />
                    <span className="font-black text-orange-900 bg-white px-2.5 py-0.5 rounded-full shadow border border-orange-200 text-xs">3ème</span>
                  </div>
                  <span className={`font-black text-sm sm:text-lg ${ANNUAL_DATA.rankings[2].textColor} text-center leading-tight`}>
                    {ANNUAL_DATA.rankings[2].team}<br/>{ANNUAL_DATA.rankings[2].score}%
                  </span>
                </div>
              </div>

              <div className="flex flex-col xl:flex-row gap-6">
                
                <div className="w-full xl:w-1/2 overflow-x-auto">
                  <table className="w-full min-w-[600px] text-sm border-collapse bg-white shadow-md rounded-lg overflow-hidden border border-gray-200">
                    <thead className="bg-[#f3d052] border-b border-gray-300">
                      <tr>
                        <th className="px-3 py-3 border-r border-gray-300/50 text-left text-yellow-900 font-black">Équipes</th>
                        <th className="px-2 py-3 border-r border-gray-300/50 text-center text-yellow-900 font-bold text-xs">Bilan heures</th>
                        <th className="px-2 py-3 border-r border-gray-300/50 text-center text-yellow-900 font-bold text-xs">Rangements</th>
                        <th className="px-2 py-3 border-r border-gray-300/50 text-center text-yellow-900 font-bold text-xs">MAP</th>
                        <th className="px-2 py-3 border-r border-gray-300/50 text-center text-yellow-900 font-bold text-xs">Réunion</th>
                        <th className="px-2 py-3 border-r border-gray-300/50 text-center text-yellow-900 font-bold text-xs">Nettoyage</th>
                        <th className="px-3 py-3 text-center text-yellow-900 font-black bg-[#ecc232]">Total</th>
                      </tr>
                    </thead>
                    <tbody>
                      {ANNUAL_DATA.table.map((row, idx) => (
                        <React.Fragment key={idx}>
                          <tr className="bg-gray-50/80 border-t border-gray-200">
                            <td colSpan="7" className="px-4 pt-3 pb-1 font-black text-gray-800 text-base">{row.name}</td>
                          </tr>
                          <tr className="border-b border-gray-200 hover:bg-gray-50 transition-colors">
                            <td className="px-4 pb-3 pt-1 border-r border-gray-200 text-xs text-gray-500 font-bold uppercase">Année 2026</td>
                            {[row.heures, row.rangements, row.map, row.reunion, row.nettoyage, row.total].map((val, i) => (
                              <td key={i} className={`px-2 pb-3 pt-1 border-r border-gray-200 text-center ${i === 5 ? 'bg-yellow-50/50 font-black text-lg' : 'font-bold'}`}>
                                <div className="flex items-center justify-center gap-1.5">
                                  <Star className={`w-4 h-4 ${val >= 90 ? 'text-yellow-500 fill-yellow-500 drop-shadow-sm' : 'text-gray-300'}`} />
                                  <span className={val >= 90 ? 'text-gray-900' : 'text-gray-500'}>{val}%</span>
                                </div>
                              </td>
                            ))}
                          </tr>
                        </React.Fragment>
                      ))}
                    </tbody>
                  </table>
                </div>

                <div className="w-full xl:w-1/2">
                  <LineChart data={ANNUAL_DATA.chart} />
                </div>

              </div>
            </div>
          );
        };

        // ==========================================
        // 4. COMPOSANT PRINCIPAL (APP)
        // ==========================================

        function App() {
          const [activeTab, setActiveTab] = useState("JOURNALIER");
          const [selectedDate, setSelectedDate] = useState("17/03/2026");
          const [currentTime, setCurrentTime] = useState(new Date());

          useEffect(() => {
            const timer = setInterval(() => setCurrentTime(new Date()), 60000);
            return () => clearInterval(timer);
          }, []);

          const getSafeDateString = () => {
            try {
              return currentTime.toLocaleDateString('fr-FR', { weekday: 'long', day: 'numeric', month: 'long', year: 'numeric' });
            } catch (e) {
              return "Date indisponible";
            }
          };

          const getSafeTimeString = () => {
            try {
              return currentTime.toLocaleTimeString('fr-FR', { hour: '2-digit', minute: '2-digit' });
            } catch (e) {
              return "--:--";
            }
          };

          const tabs = ["JOURNALIER", "FIN DE PROD", "AT", "SEMAINE", "ANNUEL"];

          return (
            <div className="h-screen bg-gray-200 flex flex-col font-sans text-gray-800 overflow-hidden">
              
              <header className="flex flex-col sm:flex-row items-center justify-between px-4 sm:px-8 py-3 border-b-2 border-gray-300 bg-white shadow-sm z-10 flex-shrink-0">
                <div className="flex items-center gap-3">
                  <Star className="w-10 h-10 text-red-600 fill-red-600 drop-shadow-sm" />
                  <span className="text-3xl font-black text-green-800 tracking-tighter">HEINEKEN</span>
                </div>
                
                <h1 className="text-xl md:text-3xl font-black text-green-800 uppercase tracking-widest my-2 sm:my-0 text-center drop-shadow-sm">
                  CONFORMITE {activeTab === "ANNUEL" ? "ANNUELLE BILAN" : "CILT JOURNALIER"} 8/9
                </h1>
                
                <div className="text-gray-700 font-bold bg-gray-100 px-4 py-1.5 rounded-full border border-gray-200">
                  {activeTab === "ANNUEL" ? (
                     <span className="text-xl">BILAN 2026</span>
                  ) : (
                     <span>DCS du {selectedDate.replace(/\//g, '-')}</span>
                  )}
                </div>
              </header>

              <main className="flex-grow flex flex-col overflow-hidden relative">
                {activeTab === "JOURNALIER" && <JournalierView selectedDate={selectedDate} setSelectedDate={setSelectedDate} />}
                {activeTab === "ANNUEL" && <AnnuelView />}
                
                {["FIN DE PROD", "AT", "SEMAINE"].includes(activeTab) && (
                  <div className="flex-grow flex items-center justify-center bg-gray-100 p-6">
                    <div className="text-center bg-white p-10 rounded-xl shadow-md border border-gray-200 max-w-lg">
                      <AlertCircle className="w-20 h-20 text-[#f498c0] mx-auto mb-6" />
                      <h2 className="text-3xl font-black text-gray-800 mb-4">Vue en développement</h2>
                      <p className="text-gray-600 text-lg">La section <span className="font-bold text-green-700">"{activeTab}"</span> sera bientôt disponible.</p>
                      <p className="text-gray-500 mt-4 text-sm">Veuillez cliquer sur <b>JOURNALIER</b> ou <b>ANNUEL</b> en bas pour explorer l'interface interactive.</p>
                    </div>
                  </div>
                )}
              </main>

              <footer className="bg-gray-300 border-t-2 border-gray-400 p-3 flex flex-col xl:flex-row items-center justify-between gap-4 flex-shrink-0 z-10 shadow-[0_-4px_6px_-1px_rgba(0,0,0,0.1)]">
                <div className="flex flex-wrap items-center gap-2 sm:gap-4 justify-center w-full xl:w-auto">
                  {tabs.map((tab) => (
                    <button
                      key={tab}
                      onClick={() => setActiveTab(tab)}
                      className={`px-4 sm:px-8 py-2.5 rounded-full font-black text-xs sm:text-sm tracking-widest transition-all duration-200 uppercase
                        ${activeTab === tab 
                          ? 'bg-gray-900 text-white shadow-[0_4px_10px_rgba(0,0,0,0.3)] transform scale-105 border-2 border-gray-900' 
                          : 'bg-[#f498c0] text-gray-900 hover:bg-[#ee7eac] border-2 border-[#e675a5] shadow-sm hover:shadow-md'
                        }`}
                    >
                      {tab}
                    </button>
                  ))}
                </div>
                
                <div className="bg-white border-2 border-gray-400 rounded px-5 py-2 flex flex-col items-center justify-center min-w-[220px] shadow-sm">
                  <span className="text-xs sm:text-sm text-green-800 font-bold text-center uppercase tracking-wide">
                    Actualisé le {getSafeDateString()}
                  </span>
                  <span className="text-sm sm:text-base text-green-800 font-black">
                    à {getSafeTimeString()}
                  </span>
                </div>
              </footer>
              
            </div>
          );
        }

        // Montage de l'application
        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
