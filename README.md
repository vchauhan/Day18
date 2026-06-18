[meeting-dashboard.html](https://github.com/user-attachments/files/29104769/meeting-dashboard.html)
[quarterly_growth_strategy_meeting.html](https://github.com/user-attachments/files/29104328/quarterly_growth_strategy_meeting.html)# Day18
Build a Brain Dump Action Planner Skill with Claude
[Uploading quarterly_growth_strat<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:var(--font-sans);color:var(--color-text-primary)}
.page{padding:1.5rem 0}
.top-bar{display:flex;align-items:center;justify-content:space-between;margin-bottom:1.5rem;flex-wrap:wrap;gap:.5rem}
.top-title{font-size:18px;font-weight:500}
.top-meta{font-size:13px;color:var(--color-text-secondary)}
.metrics{display:grid;grid-template-columns:repeat(auto-fit,minmax(130px,1fr));gap:10px;margin-bottom:1.5rem}
.metric{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:.9rem 1rem}
.metric-label{font-size:12px;color:var(--color-text-secondary);margin-bottom:4px}
.metric-value{font-size:22px;font-weight:500}
.metric-value.warn{color:var(--color-text-danger)}
.metric-value.ok{color:var(--color-text-success)}
.section{margin-bottom:1.5rem}
.section-header{font-size:15px;font-weight:500;margin-bottom:.75rem;display:flex;align-items:center;gap:8px}
.section-header i{font-size:16px;color:var(--color-text-secondary);aria-hidden:true}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:10px}
.card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1rem 1.1rem}
.card-title{font-size:13px;font-weight:500;margin-bottom:4px}
.card-body{font-size:13px;color:var(--color-text-secondary);line-height:1.6}
.badge{display:inline-flex;align-items:center;gap:4px;font-size:11px;padding:2px 8px;border-radius:var(--border-radius-md);font-weight:500;white-space:nowrap}
.b-high{background:#FCEBEB;color:#A32D2D}
.b-med{background:#FAEEDA;color:#854F0B}
.b-low{background:#EAF3DE;color:#3B6D11}
.b-open{background:#E6F1FB;color:#185FA5}
.b-conflict{background:#FBEAF0;color:#993556}
.b-pending{background:#F1EFE8;color:#5F5E5A}
.b-done{background:#EAF3DE;color:#3B6D11}
table{width:100%;border-collapse:collapse;font-size:13px}
thead tr{border-bottom:0.5px solid var(--color-border-tertiary)}
th{text-align:left;padding:8px 10px;font-weight:500;color:var(--color-text-secondary);font-size:12px}
td{padding:8px 10px;vertical-align:middle;color:var(--color-text-primary);border-bottom:0.5px solid var(--color-border-tertiary)}
tr:last-child td{border-bottom:none}
tr:hover td{background:var(--color-background-secondary)}
.table-wrap{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);overflow:hidden}
.speaker-list{display:flex;flex-direction:column;gap:8px}
.speaker-row{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:.85rem 1rem}
.speaker-header{display:flex;align-items:center;gap:10px;margin-bottom:6px}
.avatar{width:32px;height:32px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:500;flex-shrink:0}
.av-ceo{background:#EEEDFE;color:#3C3489}
.av-sales{background:#E1F5EE;color:#0F6E56}
.av-cfo{background:#FAEEDA;color:#854F0B}
.av-vpm{background:#FAECE7;color:#993C1D}
.av-pd{background:#FBEAF0;color:#993556}
.av-cto{background:#E6F1FB;color:#185FA5}
.av-cs{background:#EAF3DE;color:#3B6D11}
.speaker-name{font-size:13px;font-weight:500}
.speaker-role{font-size:11px;color:var(--color-text-secondary)}
.speaker-items{font-size:12px;color:var(--color-text-secondary);line-height:1.7;padding-left:42px}
.risk-list{display:flex;flex-direction:column;gap:8px}
.risk-item{border-left:3px solid #E24B4A;border-radius:0;padding:.7rem 1rem;background:var(--color-background-primary);border-top:0.5px solid var(--color-border-tertiary);border-right:0.5px solid var(--color-border-tertiary);border-bottom:0.5px solid var(--color-border-tertiary);border-radius:0 var(--border-radius-md) var(--border-radius-md) 0}
.risk-title{font-size:13px;font-weight:500;margin-bottom:3px}
.risk-body{font-size:12px;color:var(--color-text-secondary);line-height:1.6}
.conflict-item{border-left:3px solid #D4537E;border-top:0.5px solid var(--color-border-tertiary);border-right:0.5px solid var(--color-border-tertiary);border-bottom:0.5px solid var(--color-border-tertiary);border-radius:0 var(--border-radius-md) var(--border-radius-md) 0;padding:.7rem 1rem;background:var(--color-background-primary);margin-bottom:8px}
.divider{height:0.5px;background:var(--color-border-tertiary);margin:1.5rem 0}
.tag-row{display:flex;flex-wrap:wrap;gap:6px;margin-top:6px}
</style>

<div class="page">
  <h2 class="sr-only" style="position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0,0,0,0)">Quarterly Growth Strategy Meeting — action plan dashboard</h2>

  <div class="top-bar">
    <div>
      <div class="top-title">Quarterly growth strategy meeting</div>
      <div class="top-meta">Transcript mode &nbsp;·&nbsp; 7 speakers</div>
    </div>
    <span class="badge b-pending"><i class="ti ti-clock" aria-hidden="true"></i> Follow-up: next leadership meeting</span>
  </div>

  <div class="metrics">
    <div class="metric"><div class="metric-label">Q2 revenue growth</div><div class="metric-value warn">12%</div></div>
    <div class="metric"><div class="metric-label">Growth target</div><div class="metric-value">18%</div></div>
    <div class="metric"><div class="metric-label">Deals closed / expected</div><div class="metric-value warn">9 / 14</div></div>
    <div class="metric"><div class="metric-label">Website traffic increase</div><div class="metric-value ok">+34%</div></div>
    <div class="metric"><div class="metric-label">Customer retention</div><div class="metric-value ok">94%</div></div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-file-description" aria-hidden="true"></i> Summary</div>
    <div class="card" style="grid-column:1/-1">
      <div class="card-body">The leadership team reviewed Q2 performance, which came in at 12% revenue growth against an 18% target. The shortfall was driven by 5 enterprise deals slipping due to procurement delays and security review requests. Discussion covered conversion rate improvements, engineering capacity constraints, reporting performance issues affecting both customers and prospects, hiring plan deferral, and a pending customer conference budget. Several decisions were deferred pending further information.</div>
    </div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-bulb" aria-hidden="true"></i> Key takeaways</div>
    <div class="cards">
      <div class="card"><div class="card-title">Revenue gap is deal-slip driven</div><div class="card-body">5 of 14 expected enterprise contracts slipped to next quarter — primarily due to procurement delays and security review requests from two clients.</div></div>
      <div class="card"><div class="card-title">Reporting performance is a cross-functional issue</div><div class="card-body">Dashboard loading problems are generating support tickets and being cited by prospects during sales calls. Treated as a priority over some planned releases.</div></div>
      <div class="card"><div class="card-title">Engineering is near capacity</div><div class="card-body">The team is focused on the August analytics dashboard. Website redesign work may require additional contractors; cost estimate not yet available.</div></div>
      <div class="card"><div class="card-title">Lead generation is improving</div><div class="card-body">Website traffic is up 34% vs last quarter. Conversion rates remain below expectations; a redesign and simplified demo-request flow are planned.</div></div>
      <div class="card"><div class="card-title">Hiring decisions deferred</div><div class="card-body">Department heads submitted conflicting headcount requests. All hiring decisions are on hold until Q3 forecasts are finalized.</div></div>
      <div class="card"><div class="card-title">Conference budget pending vendor proposals</div><div class="card-body">Annual customer conference budget cannot be approved until the CFO receives final vendor proposals. To be revisited next month.</div></div>
    </div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-checkbox" aria-hidden="true"></i> Action items</div>
    <div class="table-wrap">
      <table>
        <thead><tr><th>Task</th><th>Owner</th><th>Deadline</th><th>Status</th></tr></thead>
        <tbody>
          <tr><td>Get cost estimate for website redesign / contractor work</td><td>CTO</td><td>Not specified</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
          <tr><td>Complete architecture review before approving website spend</td><td>CTO</td><td>Not specified</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
          <tr><td>Prioritize investigation of reporting performance / dashboard loading</td><td>Engineering team</td><td>Already started</td><td><span class="badge b-high">🔴 High priority</span></td></tr>
          <tr><td>Plan website redesign and simplified demo-request process</td><td>VP Marketing</td><td>Not specified</td><td><span class="badge b-med">🟠 Medium priority</span></td></tr>
          <tr><td>Finalize Q3 revenue forecast before approving hiring plan</td><td>CFO / CEO</td><td>Not specified</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
          <tr><td>Collect final vendor proposals for customer conference</td><td>CFO</td><td>Before next month</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
          <tr><td>Revisit conference budget once proposals received</td><td>CEO / CFO</td><td>Next month</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
          <tr><td>Complete engineering milestone review before public commitments on analytics dashboard</td><td>CTO / Product Director</td><td>Before conference</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
          <tr><td>Follow up on all open items</td><td>All leaders</td><td>Next leadership meeting</td><td><span class="badge b-pending">⏳ Pending</span></td></tr>
        </tbody>
      </table>
    </div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-help-circle" aria-hidden="true"></i> Open questions</div>
    <div class="cards">
      <div class="card"><span class="badge b-open" style="margin-bottom:6px">❓ Open question</span><div class="card-title">Will slipped enterprise deals close in Q3?</div><div class="card-body">If they slip again, the annual revenue target may be missed.</div></div>
      <div class="card"><span class="badge b-open" style="margin-bottom:6px">❓ Open question</span><div class="card-title">What will the website redesign cost?</div><div class="card-body">Architecture review not yet complete. Contractor spend unapproved until estimate is ready.</div></div>
      <div class="card"><span class="badge b-open" style="margin-bottom:6px">❓ Open question</span><div class="card-title">Will the August analytics dashboard release on time?</div><div class="card-body">CTO cannot currently guarantee the August date. Milestone review needed before any public announcement.</div></div>
      <div class="card"><span class="badge b-open" style="margin-bottom:6px">❓ Open question</span><div class="card-title">Should the analytics dashboard be announced at the conference?</div><div class="card-body">Depends on engineering milestone review and confidence in the August release date.</div></div>
      <div class="card"><span class="badge b-open" style="margin-bottom:6px">❓ Open question</span><div class="card-title">What headcount will be approved for next year?</div><div class="card-body">Department heads submitted conflicting requests. No decision until Q3 forecast is finalized.</div></div>
    </div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-alert-triangle" aria-hidden="true"></i> Risks &amp; blockers</div>
    <div class="risk-list">
      <div class="risk-item"><div class="risk-title">Annual revenue target at risk</div><div class="risk-body">If the 5 slipped enterprise deals move again in Q3, the full-year target will be missed. CFO flagged this explicitly.</div></div>
      <div class="risk-item"><div class="risk-title">Engineering capacity constraint</div><div class="risk-body">Team is close to capacity with the August analytics dashboard. Adding the website redesign may require external contractors, adding cost and timeline risk.</div></div>
      <div class="risk-item"><div class="risk-title">Reporting performance affecting sales and retention</div><div class="risk-body">Dashboard loading issues are actively being raised by prospects during sales calls and driving up support ticket volume. Root cause under investigation.</div></div>
      <div class="risk-item"><div class="risk-title">August analytics dashboard date uncertain</div><div class="risk-body">CTO cannot guarantee the release date. Any premature public commitment (e.g. at the conference) creates reputational risk.</div></div>
      <div class="risk-item"><div class="risk-title">Conversion rate below expectations</div><div class="risk-body">Despite strong traffic growth (+34%), conversion rates remain low. Website redesign not yet approved or scoped.</div></div>
    </div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-alert-circle" aria-hidden="true"></i> Conflicts</div>
    <div class="conflict-item"><span class="badge b-conflict" style="margin-bottom:5px">⚠️ Conflict</span><div class="risk-title">Website redesign vs. engineering capacity</div><div class="risk-body">VP Marketing wants a website redesign to improve conversion rates. CTO warns engineering is at capacity due to the August analytics dashboard. These two priorities compete for the same resource pool.</div></div>
    <div class="conflict-item"><span class="badge b-conflict" style="margin-bottom:5px">⚠️ Conflict</span><div class="risk-title">Reporting performance fix vs. planned feature roadmap</div><div class="risk-body">Product Director and Head of Sales both flagged that fixing reporting performance may have more business impact than some planned releases — implying existing roadmap priorities may need to be reshuffled.</div></div>
    <div class="conflict-item"><span class="badge b-conflict" style="margin-bottom:5px">⚠️ Conflict</span><div class="risk-title">Conflicting headcount requests</div><div class="risk-body">Department heads submitted different headcount numbers. No resolution was reached; decision deferred to after Q3 forecast.</div></div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-users" aria-hidden="true"></i> Speaker summary</div>
    <div class="speaker-list">
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-ceo">CEO</div><div><div class="speaker-name">CEO</div><div class="speaker-role">Chaired the meeting</div></div></div>
        <div class="speaker-items">Flagged 12% vs 18% revenue gap · Deferred hiring until Q3 forecast · Blocked website spend until cost estimate available · Requested milestone review before any public dashboard commitment · Deferred conference budget to next month</div>
      </div>
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-sales">HoS</div><div><div class="speaker-name">Head of Sales</div><div class="speaker-role">Sales</div></div></div>
        <div class="speaker-items">Reported 9 of 14 enterprise deals closed · Cited procurement delays and security reviews as reasons for slippage · Noted prospects raising reporting performance in sales calls · Asked about announcing analytics dashboard at conference</div>
      </div>
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-cfo">CFO</div><div><div class="speaker-name">CFO</div><div class="speaker-role">Finance</div></div></div>
        <div class="speaker-items">Flagged annual target risk if deals slip again · Raised need for headcount clarity · Awaiting final vendor proposals before approving conference budget · Asked for website redesign cost estimate</div>
      </div>
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-vpm">VPM</div><div><div class="speaker-name">VP Marketing</div><div class="speaker-role">Marketing</div></div></div>
        <div class="speaker-items">Reported +34% website traffic growth · Acknowledged lower-than-expected conversion rates · Plans website redesign and simplified demo-request flow · Raised customer conference budget approval</div>
      </div>
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-pd">PD</div><div><div class="speaker-name">Product Director</div><div class="speaker-role">Product</div></div></div>
        <div class="speaker-items">Flagged engineering timeline risk if website work is added · Agreed reporting performance fix may outrank some planned releases · Conditional on milestone review before committing to August conference announcement</div>
      </div>
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-cto">CTO</div><div><div class="speaker-name">CTO</div><div class="speaker-role">Engineering</div></div></div>
        <div class="speaker-items">Confirmed engineering is near capacity · Website work may require contractors · Architecture review not complete · Cannot guarantee August dashboard date · Confirmed reporting performance investigation has started</div>
      </div>
      <div class="speaker-row">
        <div class="speaker-header"><div class="avatar av-cs">CSL</div><div><div class="speaker-name">Customer Success Lead</div><div class="speaker-role">Customer Success</div></div></div>
        <div class="speaker-items">Reported 94% customer retention · Flagged significant increase in support ticket volume driven by reporting performance and dashboard loading times</div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-header"><i class="ti ti-notes" aria-hidden="true"></i> Additional notes</div>
    <div class="cards">
      <div class="card"><div class="card-title">Decisions made in this meeting</div><div class="card-body">No additional website spending approved until cost estimate is received · Hiring decisions postponed until Q3 forecast finalized · Conference budget deferred to next month · No public commitments on August dashboard date until milestone review complete</div></div>
      <div class="card"><div class="card-title">Attribution note</div><div class="card-body">Ownership of several action items (architecture review, cost estimate) is assigned to the CTO but no individual name was given. "Engineering team" is used as attributed in the transcript.</div></div>
    </div>
  </div>
</div>
egy_meeting.html…]()[meeting-dashboard.html](https://github.com/user-attachments/files/29104784/meeting-dashboard.html)

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Quarterly Growth Strategy — Meeting Dashboard</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0f1117;
    --surface: #181c26;
    --surface2: #1f2435;
    --border: rgba(255,255,255,0.07);
    --border2: rgba(255,255,255,0.12);
    --text: #e8eaf0;
    --muted: #7b8294;
    --dim: #4a5068;
    --accent: #5b6ef5;
    --accent-glow: rgba(91,110,245,0.15);
    --red: #f55b5b;
    --red-bg: rgba(245,91,91,0.1);
    --amber: #f5a623;
    --amber-bg: rgba(245,166,35,0.1);
    --green: #3ecf8e;
    --green-bg: rgba(62,207,142,0.1);
    --blue: #5b9ef5;
    --blue-bg: rgba(91,158,245,0.1);
    --pink: #d45bf5;
    --pink-bg: rgba(212,91,245,0.1);
    --mono: 'IBM Plex Mono', monospace;
    --sans: 'Inter', system-ui, sans-serif;
    --r: 8px;
    --r-lg: 12px;
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html { font-size: 15px; }
  body {
    font-family: var(--sans);
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
    min-height: 100vh;
  }

  /* Layout */
  .shell { max-width: 1140px; margin: 0 auto; padding: 0 24px 64px; }
  .topbar {
    display: flex; align-items: center; justify-content: space-between;
    padding: 20px 0 28px;
    border-bottom: 1px solid var(--border);
    margin-bottom: 32px;
    flex-wrap: wrap; gap: 12px;
  }
  .topbar-left { display: flex; align-items: center; gap: 14px; }
  .logo-mark {
    width: 36px; height: 36px; border-radius: 8px;
    background: var(--accent-glow);
    border: 1px solid rgba(91,110,245,0.3);
    display: flex; align-items: center; justify-content: center;
    font-family: var(--mono); font-size: 13px; color: var(--accent); font-weight: 500;
  }
  .meeting-title { font-size: 15px; font-weight: 600; letter-spacing: -0.2px; }
  .meeting-sub { font-size: 12px; color: var(--muted); margin-top: 1px; }
  .topbar-right { display: flex; align-items: center; gap: 8px; }
  .pill {
    font-size: 11px; font-family: var(--mono); font-weight: 500;
    padding: 4px 10px; border-radius: 20px;
    background: var(--surface2); border: 1px solid var(--border2);
    color: var(--muted); white-space: nowrap;
  }
  .pill.live { color: var(--green); border-color: rgba(62,207,142,0.25); background: var(--green-bg); }

  /* Metrics row */
  .metrics { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px,1fr)); gap: 12px; margin-bottom: 32px; }
  .metric {
    background: var(--surface); border: 1px solid var(--border);
    border-radius: var(--r-lg); padding: 16px 18px;
    position: relative; overflow: hidden;
  }
  .metric::before {
    content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
    background: var(--accent-color, var(--accent));
    opacity: 0.6;
  }
  .metric-label { font-size: 11px; color: var(--muted); text-transform: uppercase; letter-spacing: .05em; margin-bottom: 6px; }
  .metric-value { font-family: var(--mono); font-size: 26px; font-weight: 500; line-height: 1; }
  .metric-value.warn { color: var(--red); }
  .metric-value.ok { color: var(--green); }
  .metric-value.neutral { color: var(--text); }
  .metric-note { font-size: 11px; color: var(--muted); margin-top: 5px; }

  /* Two-col layout */
  .two-col { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; margin-bottom: 16px; }
  @media (max-width: 720px) { .two-col { grid-template-columns: 1fr; } }

  /* Sections */
  .section { margin-bottom: 16px; }
  .card {
    background: var(--surface); border: 1px solid var(--border);
    border-radius: var(--r-lg); overflow: hidden;
  }
  .card-head {
    display: flex; align-items: center; justify-content: space-between;
    padding: 14px 18px; border-bottom: 1px solid var(--border);
  }
  .card-head-left { display: flex; align-items: center; gap: 8px; }
  .card-icon {
    width: 22px; height: 22px; border-radius: 5px;
    display: flex; align-items: center; justify-content: center;
    font-size: 12px;
  }
  .card-title { font-size: 13px; font-weight: 600; letter-spacing: -0.1px; }
  .count-badge {
    font-family: var(--mono); font-size: 11px;
    background: var(--surface2); border: 1px solid var(--border2);
    color: var(--muted); border-radius: 20px; padding: 2px 8px;
  }
  .card-body { padding: 16px 18px; }

  /* Summary */
  .summary-text { font-size: 13.5px; color: var(--muted); line-height: 1.75; }

  /* Key takeaways grid */
  .takeaway-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
  @media (max-width: 520px) { .takeaway-grid { grid-template-columns: 1fr; } }
  .takeaway {
    background: var(--surface2); border: 1px solid var(--border);
    border-radius: var(--r); padding: 12px 14px;
  }
  .takeaway-title { font-size: 12px; font-weight: 600; margin-bottom: 4px; }
  .takeaway-body { font-size: 12px; color: var(--muted); line-height: 1.6; }

  /* Action items table */
  .table-wrap { overflow-x: auto; }
  table { width: 100%; border-collapse: collapse; font-size: 12.5px; }
  th {
    text-align: left; padding: 9px 14px;
    font-size: 11px; font-weight: 500; color: var(--dim);
    text-transform: uppercase; letter-spacing: .06em;
    border-bottom: 1px solid var(--border);
    white-space: nowrap;
  }
  td { padding: 10px 14px; border-bottom: 1px solid var(--border); vertical-align: middle; }
  tr:last-child td { border-bottom: none; }
  tr:hover td { background: rgba(255,255,255,0.02); }
  .task-name { font-weight: 500; color: var(--text); }
  .task-owner { color: var(--muted); font-family: var(--mono); font-size: 11.5px; }
  .task-deadline { color: var(--muted); font-size: 12px; }
  .task-deadline.soon { color: var(--amber); }

  /* Badges */
  .badge {
    display: inline-flex; align-items: center; gap: 4px;
    font-size: 10.5px; font-weight: 500; padding: 3px 8px;
    border-radius: 20px; white-space: nowrap; font-family: var(--mono);
  }
  .b-high { background: var(--red-bg); color: var(--red); border: 1px solid rgba(245,91,91,0.2); }
  .b-med { background: var(--amber-bg); color: var(--amber); border: 1px solid rgba(245,166,35,0.2); }
  .b-low { background: var(--green-bg); color: var(--green); border: 1px solid rgba(62,207,142,0.2); }
  .b-pending { background: var(--surface2); color: var(--muted); border: 1px solid var(--border2); }
  .b-open { background: var(--blue-bg); color: var(--blue); border: 1px solid rgba(91,158,245,0.2); }
  .b-conflict { background: var(--pink-bg); color: var(--pink); border: 1px solid rgba(212,91,245,0.2); }
  .b-started { background: var(--green-bg); color: var(--green); border: 1px solid rgba(62,207,142,0.2); }

  /* Risks */
  .risk-list { display: flex; flex-direction: column; gap: 10px; }
  .risk-item {
    border-left: 2px solid var(--red);
    padding: 10px 14px;
    background: var(--surface2); border-radius: 0 var(--r) var(--r) 0;
  }
  .risk-title { font-size: 12.5px; font-weight: 600; margin-bottom: 3px; }
  .risk-body { font-size: 12px; color: var(--muted); line-height: 1.6; }

  /* Conflicts */
  .conflict-list { display: flex; flex-direction: column; gap: 10px; }
  .conflict-item {
    border-left: 2px solid var(--pink);
    padding: 10px 14px;
    background: var(--surface2); border-radius: 0 var(--r) var(--r) 0;
  }

  /* Open questions */
  .oq-list { display: flex; flex-direction: column; gap: 8px; }
  .oq-item {
    display: flex; align-items: flex-start; gap: 10px;
    padding: 10px 14px; background: var(--surface2);
    border-radius: var(--r); border: 1px solid var(--border);
  }
  .oq-num {
    font-family: var(--mono); font-size: 11px; color: var(--dim);
    min-width: 20px; padding-top: 1px;
  }
  .oq-content {}
  .oq-title { font-size: 12.5px; font-weight: 600; margin-bottom: 3px; }
  .oq-body { font-size: 12px; color: var(--muted); }

  /* Speakers */
  .speaker-grid { display: flex; flex-direction: column; gap: 10px; }
  .speaker-row {
    display: flex; gap: 12px; align-items: flex-start;
    padding: 12px 14px; background: var(--surface2);
    border-radius: var(--r); border: 1px solid var(--border);
  }
  .avatar {
    width: 34px; height: 34px; border-radius: 50%;
    display: flex; align-items: center; justify-content: center;
    font-size: 10px; font-weight: 600; flex-shrink: 0;
    font-family: var(--mono); border: 1px solid transparent;
  }
  .av-ceo { background: rgba(91,110,245,0.15); color: #8fa3f5; border-color: rgba(91,110,245,0.25); }
  .av-sales { background: rgba(62,207,142,0.12); color: #3ecf8e; border-color: rgba(62,207,142,0.25); }
  .av-cfo { background: rgba(245,166,35,0.12); color: var(--amber); border-color: rgba(245,166,35,0.25); }
  .av-vpm { background: rgba(245,91,91,0.12); color: #f57b7b; border-color: rgba(245,91,91,0.2); }
  .av-pd { background: rgba(212,91,245,0.12); color: var(--pink); border-color: rgba(212,91,245,0.2); }
  .av-cto { background: rgba(91,158,245,0.12); color: var(--blue); border-color: rgba(91,158,245,0.2); }
  .av-cs { background: rgba(62,207,142,0.08); color: #2ea870; border-color: rgba(62,207,142,0.15); }
  .speaker-info {}
  .speaker-name { font-size: 12.5px; font-weight: 600; }
  .speaker-items { font-size: 12px; color: var(--muted); line-height: 1.65; margin-top: 3px; }

  /* Footer */
  .footer {
    margin-top: 48px; padding-top: 20px;
    border-top: 1px solid var(--border);
    font-size: 11.5px; color: var(--dim);
    display: flex; justify-content: space-between; align-items: center;
    flex-wrap: wrap; gap: 8px;
  }

  /* Responsive */
  @media (max-width: 640px) {
    .shell { padding: 0 16px 48px; }
    .metrics { grid-template-columns: 1fr 1fr; }
    .takeaway-grid { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>
<div class="shell">

  <!-- Topbar -->
  <div class="topbar">
    <div class="topbar-left">
      <div class="logo-mark">Q2</div>
      <div>
        <div class="meeting-title">Quarterly Growth Strategy Meeting</div>
        <div class="meeting-sub">Leadership · 7 Attendees · Transcript Mode</div>
      </div>
    </div>
    <div class="topbar-right">
      <span class="pill">9 action items</span>
      <span class="pill">5 open questions</span>
      <span class="pill live">● Follow-up pending</span>
    </div>
  </div>

  <!-- Metrics -->
  <div class="metrics">
    <div class="metric" style="--accent-color: var(--red)">
      <div class="metric-label">Q2 Revenue Growth</div>
      <div class="metric-value warn">12%</div>
      <div class="metric-note">Target was 18%</div>
    </div>
    <div class="metric" style="--accent-color: var(--amber)">
      <div class="metric-label">Deals Closed</div>
      <div class="metric-value warn">9/14</div>
      <div class="metric-note">5 slipped to Q3</div>
    </div>
    <div class="metric" style="--accent-color: var(--green)">
      <div class="metric-label">Website Traffic</div>
      <div class="metric-value ok">+34%</div>
      <div class="metric-note">vs. last quarter</div>
    </div>
    <div class="metric" style="--accent-color: var(--green)">
      <div class="metric-label">Customer Retention</div>
      <div class="metric-value ok">94%</div>
      <div class="metric-note">Support tickets up</div>
    </div>
    <div class="metric" style="--accent-color: var(--red)">
      <div class="metric-label">Annual Target</div>
      <div class="metric-value warn">At risk</div>
      <div class="metric-note">If deals slip again</div>
    </div>
  </div>

  <!-- Summary + Key Takeaways -->
  <div class="two-col">
    <div class="section">
      <div class="card" style="height:100%">
        <div class="card-head">
          <div class="card-head-left">
            <div class="card-icon" style="background:rgba(91,110,245,0.12)">📋</div>
            <span class="card-title">Summary</span>
          </div>
        </div>
        <div class="card-body">
          <p class="summary-text">The leadership team reviewed Q2 performance, which came in at 12% revenue growth against an 18% target. The shortfall was driven by 5 enterprise deals slipping due to procurement delays and security review requests. Discussion covered conversion rate improvements, engineering capacity constraints, reporting performance issues affecting both customers and prospects, hiring plan deferral, and a pending customer conference budget. Several decisions were deferred pending further information.</p>
        </div>
      </div>
    </div>

    <div class="section">
      <div class="card" style="height:100%">
        <div class="card-head">
          <div class="card-head-left">
            <div class="card-icon" style="background:rgba(245,166,35,0.12)">💡</div>
            <span class="card-title">Key Takeaways</span>
          </div>
          <span class="count-badge">6</span>
        </div>
        <div class="card-body">
          <div class="takeaway-grid">
            <div class="takeaway">
              <div class="takeaway-title">Revenue gap is deal-slip driven</div>
              <div class="takeaway-body">5 of 14 enterprise contracts slipped — procurement delays and security reviews.</div>
            </div>
            <div class="takeaway">
              <div class="takeaway-title">Reporting performance is a priority</div>
              <div class="takeaway-body">Dashboard loading issues cited by prospects and driving support tickets.</div>
            </div>
            <div class="takeaway">
              <div class="takeaway-title">Engineering is near capacity</div>
              <div class="takeaway-body">August analytics dashboard in progress. Website work may need contractors.</div>
            </div>
            <div class="takeaway">
              <div class="takeaway-title">Traffic up, conversions lag</div>
              <div class="takeaway-body">Website traffic +34% but conversion rates still below expectations.</div>
            </div>
            <div class="takeaway">
              <div class="takeaway-title">Hiring decisions deferred</div>
              <div class="takeaway-body">Conflicting headcount requests. On hold until Q3 forecast is finalized.</div>
            </div>
            <div class="takeaway">
              <div class="takeaway-title">Conference budget pending</div>
              <div class="takeaway-body">Awaiting final vendor proposals. Revisit next month.</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Action Items -->
  <div class="section">
    <div class="card">
      <div class="card-head">
        <div class="card-head-left">
          <div class="card-icon" style="background:rgba(62,207,142,0.12)">✅</div>
          <span class="card-title">Action Items</span>
        </div>
        <span class="count-badge">9</span>
      </div>
      <div class="table-wrap">
        <table>
          <thead>
            <tr>
              <th>Task</th>
              <th>Owner</th>
              <th>Deadline</th>
              <th>Status</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><span class="task-name">Get cost estimate for website redesign / contractor work</span></td>
              <td><span class="task-owner">CTO</span></td>
              <td><span class="task-deadline">Not specified</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Complete architecture review before approving website spend</span></td>
              <td><span class="task-owner">CTO</span></td>
              <td><span class="task-deadline">Not specified</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Prioritize fix for reporting performance / dashboard loading</span></td>
              <td><span class="task-owner">Engineering</span></td>
              <td><span class="task-deadline">Already started</span></td>
              <td><span class="badge b-high">🔴 High priority</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Plan website redesign and simplified demo-request process</span></td>
              <td><span class="task-owner">VP Marketing</span></td>
              <td><span class="task-deadline">Not specified</span></td>
              <td><span class="badge b-med">🟠 Medium priority</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Finalize Q3 revenue forecast before approving hiring plan</span></td>
              <td><span class="task-owner">CFO / CEO</span></td>
              <td><span class="task-deadline">Not specified</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Collect final vendor proposals for customer conference</span></td>
              <td><span class="task-owner">CFO</span></td>
              <td><span class="task-deadline soon">Before next month</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Revisit conference budget once proposals received</span></td>
              <td><span class="task-owner">CEO / CFO</span></td>
              <td><span class="task-deadline soon">Next month</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Complete engineering milestone review before public dashboard commitment</span></td>
              <td><span class="task-owner">CTO / Product</span></td>
              <td><span class="task-deadline">Before conference</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
            <tr>
              <td><span class="task-name">Follow up on all open items</span></td>
              <td><span class="task-owner">All leaders</span></td>
              <td><span class="task-deadline soon">Next leadership mtg</span></td>
              <td><span class="badge b-pending">⏳ Pending</span></td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>

  <!-- Risks + Open Questions -->
  <div class="two-col">
    <div class="section">
      <div class="card" style="height:100%">
        <div class="card-head">
          <div class="card-head-left">
            <div class="card-icon" style="background:rgba(245,91,91,0.12)">⚠️</div>
            <span class="card-title">Risks &amp; Blockers</span>
          </div>
          <span class="count-badge">5</span>
        </div>
        <div class="card-body">
          <div class="risk-list">
            <div class="risk-item">
              <div class="risk-title">Annual revenue target at risk</div>
              <div class="risk-body">If the 5 slipped enterprise deals move again in Q3, the full-year target will be missed. CFO flagged this explicitly.</div>
            </div>
            <div class="risk-item">
              <div class="risk-title">Engineering capacity constraint</div>
              <div class="risk-body">Team is close to capacity with the August analytics dashboard. Adding the website redesign may require external contractors.</div>
            </div>
            <div class="risk-item">
              <div class="risk-title">Reporting performance affecting sales &amp; retention</div>
              <div class="risk-body">Dashboard loading issues are being raised by prospects in sales calls and driving up support ticket volume.</div>
            </div>
            <div class="risk-item">
              <div class="risk-title">August analytics dashboard date uncertain</div>
              <div class="risk-body">CTO cannot guarantee the release date. Any premature public commitment creates reputational risk.</div>
            </div>
            <div class="risk-item">
              <div class="risk-title">Conversion rate below expectations</div>
              <div class="risk-body">Despite strong traffic growth (+34%), conversion rates remain low. Redesign not yet approved or scoped.</div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="section">
      <div class="card" style="height:100%">
        <div class="card-head">
          <div class="card-head-left">
            <div class="card-icon" style="background:rgba(91,158,245,0.12)">❓</div>
            <span class="card-title">Open Questions</span>
          </div>
          <span class="count-badge">5</span>
        </div>
        <div class="card-body">
          <div class="oq-list">
            <div class="oq-item">
              <div class="oq-num">01</div>
              <div class="oq-content">
                <div class="oq-title">Will slipped enterprise deals close in Q3?</div>
                <div class="oq-body">If they slip again, the annual revenue target will be missed.</div>
              </div>
            </div>
            <div class="oq-item">
              <div class="oq-num">02</div>
              <div class="oq-content">
                <div class="oq-title">What will the website redesign cost?</div>
                <div class="oq-body">Architecture review not complete. Contractor spend unapproved until estimate is ready.</div>
              </div>
            </div>
            <div class="oq-item">
              <div class="oq-num">03</div>
              <div class="oq-content">
                <div class="oq-title">Will the August analytics dashboard release on time?</div>
                <div class="oq-body">CTO cannot currently guarantee the August date. Milestone review required first.</div>
              </div>
            </div>
            <div class="oq-item">
              <div class="oq-num">04</div>
              <div class="oq-content">
                <div class="oq-title">Should the dashboard be announced at the conference?</div>
                <div class="oq-body">Depends on engineering milestone review and confidence in August release date.</div>
              </div>
            </div>
            <div class="oq-item">
              <div class="oq-num">05</div>
              <div class="oq-content">
                <div class="oq-title">What headcount will be approved for next year?</div>
                <div class="oq-body">Conflicting requests from department heads. No decision until Q3 forecast is finalized.</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Conflicts -->
  <div class="section">
    <div class="card">
      <div class="card-head">
        <div class="card-head-left">
          <div class="card-icon" style="background:rgba(212,91,245,0.12)">⚡</div>
          <span class="card-title">Conflicts</span>
        </div>
        <span class="count-badge">3</span>
      </div>
      <div class="card-body">
        <div class="conflict-list">
          <div class="conflict-item">
            <div class="risk-title">Website redesign vs. engineering capacity <span class="badge b-conflict" style="margin-left:8px">⚠️ Resource conflict</span></div>
            <div class="risk-body">VP Marketing wants a website redesign to improve conversions. CTO warns engineering is at capacity due to the August analytics dashboard. These priorities compete for the same resource pool.</div>
          </div>
          <div class="conflict-item">
            <div class="risk-title">Reporting performance fix vs. planned feature roadmap <span class="badge b-conflict" style="margin-left:8px">⚠️ Priority conflict</span></div>
            <div class="risk-body">Product Director and Head of Sales both flagged that fixing reporting performance may have more business impact than some planned releases — implying the existing roadmap may need reshuffling.</div>
          </div>
          <div class="conflict-item">
            <div class="risk-title">Conflicting headcount requests <span class="badge b-conflict" style="margin-left:8px">⚠️ Decision conflict</span></div>
            <div class="risk-body">Department heads submitted different headcount numbers. No resolution reached; decision deferred to after Q3 forecast.</div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Speaker Summary -->
  <div class="section">
    <div class="card">
      <div class="card-head">
        <div class="card-head-left">
          <div class="card-icon" style="background:rgba(91,110,245,0.12)">👥</div>
          <span class="card-title">Speaker Summary</span>
        </div>
        <span class="count-badge">7 attendees</span>
      </div>
      <div class="card-body">
        <div class="speaker-grid">
          <div class="speaker-row">
            <div class="avatar av-ceo">CEO</div>
            <div class="speaker-info">
              <div class="speaker-name">CEO <span style="color:var(--dim);font-weight:400;font-size:11.5px">· Chaired</span></div>
              <div class="speaker-items">Flagged 12% vs 18% revenue gap · Deferred hiring until Q3 forecast · Blocked website spend until cost estimate available · Requested milestone review before any public dashboard commitment · Deferred conference budget to next month</div>
            </div>
          </div>
          <div class="speaker-row">
            <div class="avatar av-sales">HoS</div>
            <div class="speaker-info">
              <div class="speaker-name">Head of Sales</div>
              <div class="speaker-items">Reported 9 of 14 enterprise deals closed · Cited procurement delays and security reviews for slippage · Noted prospects raising reporting performance in sales calls · Asked about announcing analytics dashboard at conference</div>
            </div>
          </div>
          <div class="speaker-row">
            <div class="avatar av-cfo">CFO</div>
            <div class="speaker-info">
              <div class="speaker-name">CFO</div>
              <div class="speaker-items">Flagged annual target risk if deals slip again · Raised need for headcount clarity · Awaiting final vendor proposals before approving conference budget · Asked for website redesign cost estimate</div>
            </div>
          </div>
          <div class="speaker-row">
            <div class="avatar av-vpm">VPM</div>
            <div class="speaker-info">
              <div class="speaker-name">VP Marketing</div>
              <div class="speaker-items">Reported +34% website traffic growth · Acknowledged lower-than-expected conversion rates · Plans website redesign and simplified demo-request flow · Raised customer conference budget approval</div>
            </div>
          </div>
          <div class="speaker-row">
            <div class="avatar av-pd">PD</div>
            <div class="speaker-info">
              <div class="speaker-name">Product Director</div>
              <div class="speaker-items">Flagged engineering timeline risk if website work is added · Agreed reporting performance fix may outrank some planned releases · Wants milestone review before committing to August conference announcement</div>
            </div>
          </div>
          <div class="speaker-row">
            <div class="avatar av-cto">CTO</div>
            <div class="speaker-info">
              <div class="speaker-name">CTO</div>
              <div class="speaker-items">Confirmed engineering is near capacity · Website work may require contractors · Architecture review not complete · Cannot guarantee August dashboard date · Confirmed reporting performance investigation has started</div>
            </div>
          </div>
          <div class="speaker-row">
            <div class="avatar av-cs">CSL</div>
            <div class="speaker-info">
              <div class="speaker-name">Customer Success Lead</div>
              <div class="speaker-items">Reported 94% customer retention · Flagged significant increase in support ticket volume driven by reporting performance and dashboard loading times</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <div class="footer">
    <span>Quarterly Growth Strategy Meeting · Brain-dump-action-planner</span>
    <span>All content sourced directly from transcript · Nothing invented or inferred</span>
  </div>

</div>
</body>
</html>
