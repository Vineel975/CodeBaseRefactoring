claim-processing/
├── lib/                                          ← ADD THIS FOLDER
│   └── rules/                                    ← ADD
│       ├── types.ts                              ← NEW
│       ├── cataract.ts                           ← NEW
│       ├── maternity.ts                          ← NEW
│       ├── other.ts                              ← NEW
│       ├── index.ts                              ← NEW
│       ├── index.test.ts                         ← NEW
│       └── README.md                             ← NEW
├── app/
│   ├── api/
│   │   ├── audit/start/route.ts                  ← MODIFY (small change)
│   │   ├── classify-claim-type/route.ts          ← REPLACE entirely
│   │   ├── benefit-section-summary/route.ts      ← MODIFY (small change)
│   │   ├── alignment-cappings/route.ts           ← MODIFY (small change)
│   │   ├── previous-claim-similarity/route.ts    ← MODIFY (small change)
│   │   ├── accommodation-recommend/route.ts      ← MODIFY (small change)
│   │   ├── tariff-file-selection/route.ts        ← NO CHANGE
│   │   └── benefit-plan-limit/route.ts           ← NO CHANGE
│   └── job/[jobId]/
│       ├── page.tsx                              ← NO CHANGE
│       └── components/
│           ├── result-view.tsx                   ← MODIFY (UI flags)
│           ├── patient-info-tab.tsx              ← MODIFY (UI flags)
│           ├── medical-admissibility-tab.tsx     ← MODIFY (UI flags)
│           ├── financial-summary-tab.tsx         ← MODIFY (UI flags)
│           └── processing-logs.tsx               ← NO CHANGE
├── convex/
│   ├── extract.ts                                ← MODIFY (admissibility block)
│   ├── processPdf.ts                             ← MODIFY (optional small change)
│   ├── prompts.ts                                ← REPLACE entirely
│   ├── processing.ts                             ← NO CHANGE
│   ├── jobMutations.ts                           ← NO CHANGE
│   └── schema.ts                                 ← NO CHANGE
├── tsconfig.json                                 ← Verify path alias exists
└── package.json                                  ← NO CHANGE
