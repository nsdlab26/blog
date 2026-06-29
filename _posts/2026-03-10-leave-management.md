---
layout: post
title: "[운영 체계 #4] 유료 HR 툴 없이 휴가 관리를 운영한 방법 "
slug: leave-management
category: 업무 체계
cover: https://cdn.imweb.me/upload/S20260317e48e798a6d243/9ac13702d8cab.png
date: 2026-03-10
meta_title: "[운영 체계 #4] 유료 HR 툴 없이 휴가 관리를 운영한 방법 "
meta_description: "엑셀 시트 대신 워크플로우로, 자동 계산되는 휴가 관리. 휴가 신청–승인–연차 차감–잔여 현황까지 한번에."
---
<div style="font-family: 'Pretendard', sans-serif; color: #1a1f27; letter-spacing: -0.01em;">
<p style="text-align: left; margin-bottom: 32px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/9ac13702d8cab.png" alt="" /></p>
<blockquote style="background-color: #f5f4f8; padding: 25px 30px; border-left: 5px solid #8366EE; border-radius: 8px; margin: 30px 0 40px 0; border-top: none; border-right: none; border-bottom: none; quotes: none;">
<h3 style="font-size: 18px; font-weight: bold; color: #8366ee; margin-top: 0px; margin-bottom: 15px; display: flex; align-items: center; gap: 8px; line-height: 1.4;"><span style="font-size: 20px;">💡</span> 핵심 포인트</h3>
<ul style="list-style: none; padding-left: 0; margin-bottom: 0; font-size: 16px; font-weight: 400; line-height: 1.7; color: #1a1f27;">
<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px;"><span style="color: #8366ee; font-weight: bold; flex-shrink: 0;">✔️</span> 휴가 신청 → 승인 → 집계까지 한번에</li>
<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px;"><span style="color: #8366ee; font-weight: bold; flex-shrink: 0;">✔️</span> 입사일 기준 발생·잔여 연차가 자동 계산</li>
<li style="display: flex; align-items: start; gap: 10px;"><span style="color: #8366ee; font-weight: bold; flex-shrink: 0;">✔️</span> 개인별 사용 현황과 잔여분을 한눈에 확인</li>
</ul>
</blockquote>
<p style="margin-bottom: 32px;"><a style="font-size: 16px; font-weight: bold; text-decoration: none; color: #8366ee;" href="https://www.nsdlab.kr/main/?idx=8" target="_blank" rel="noopener noreferrer">👉 만들어진 시스템으로 바로 도입하기</a></p>

<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">직접 만든 휴가 관리 시스템, 25명 규모 조직에서 몇 년간 운영한 사례</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">팀이 커지다 보면 꼭 한번 이런 순간이 오게 됩니다. 업무가 사람에 대한 의존도가 높고, 히스토리가 쌓이지 않고, 뭔가 정리가 필요하다는 느낌이요.</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">그때 보통 하는 선택이 "툴 도입"인 것 같아요. 그런데 근태, 프로젝트, 문서 관리 툴 ㅡ 하나씩 추가하다 보면 어느새 팀원들은 이리저리 옮겨다니고, 고정비는 쌓이고, 업무는 오히려 더 파편화 됩니다.</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">특히 크지 않은 조직에서는 유연한 업무 관리가 필요할 때도 많은데, 그때마다 새로운 툴을 도입하기는 어렵죠. 그래서 선택한 방법은, 이미 전사적으로 사용하고 있던 노션을 중심으로 업무 체계를 구축하는 거였습니다.</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">휴가 관리 시스템은 그 과정에서 만들어진 체계 중 하나였습니다. 실제로 25명 규모의 조직에서 몇 년간 운영하며 사용했던 사례를 공유합니다.</p>
</section>

<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">노션으로 직접 만든 이유</h2>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.7;">
<li style="margin-bottom: 14px;"><strong style="color: #8366ee; font-size: 17px;">1. 이미 전사적으로 노션을 쓰고 있었다</strong><br><span style="color: #555;">업무마다 새 툴을 추가하면 고정비가 쌓이고, 팀원들은 이리저리 옮겨다니느라 피로해진다.</span></li>
<li style="margin-bottom: 14px;"><strong style="color: #8366ee; font-size: 17px;">2. 예외 케이스가 많지 않았다</strong><br><span style="color: #555;">전 직원 풀타임 구조라 근무 유형이 단순했고, 복잡한 수당 계산이 필요하지 않았다.</span></li>
<li><strong style="color: #8366ee; font-size: 17px;">3. 자유도가 높다</strong><br><span style="color: #555;">데이터베이스, 수식, 권한 설정까지 조합하면 웬만한 업무 시스템은 직접 구축할 수 있다.</span></li>
</ul>
</div>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">결과적으로 만들어진 시스템은 이렇게 작동합니다. 휴가 신청·승인 과정, 입사일 기준 발생·사용·잔여 연차가 자동으로 계산됩니다. "내 휴가가 몇 개 남았지?"를 매번 묻지 않아도 되고, 관리자는 휴가 사용 현황을 엑셀로 정리하거나 잔여 연차를 따로 계산할 필요가 없습니다.</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">다만, 이 방식은 중·소규모 조직에 더 적합합니다. 조직 규모가 크거나, 근무 유형과 수당 구조가 복잡하다면 전문 HR 솔루션이 더 적합할 수 있습니다.</p>
</section>

<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">어떤 구조로 돌아가나?</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">크게 두 페이지로 운영합니다. 전 직원이 접근하는 휴가 신청 페이지와, 관리자만 볼 수 있는 관리자 페이지입니다.</p>
<div style="margin-bottom: 24px;"><img style="width: 100%; border-radius: 8px;" src="/assets/leave_process.png" alt="노션 휴가 관리 시스템 프로세스" /></div>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<ol style="padding-left: 20px; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27;">
<li style="margin-bottom: 8px;"><strong>기본 설정:</strong> 휴가 종류(연차, 반차, 병가 등)와 멤버 정보를 입력</li>
<li style="margin-bottom: 8px;"><strong>신청:</strong> 멤버가 휴가를 신청하면, 팀장에게 자동으로 알림 발송</li>
<li style="margin-bottom: 8px;"><strong>승인:</strong> 팀장이 승인하면, 신청 리스트에서 정리</li>
<li><strong>집계:</strong> 해당 멤버의 휴가 현황에 자동으로 업데이트 되고, 사용·잔여 연차는 실시간 계산되어 반영</li>
</ol>
</div>
</section>

<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">휴가 신청 화면</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">모든 멤버가 접근할 수 있지만, 권한 설정으로 승인된 휴가를 삭제하거나 규정을 임의로 수정할 수 없습니다.</p>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.7;">
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 멤버는 휴가를 신청하고, 관리자는 알림을 받아 승인할 수 있습니다.</li>
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 본인의 연차 사용 내역과 잔여 현황을 확인할 수 있습니다. (다른 멤버의 정보는 보이지 않음)</li>
<li style="display: flex; align-items: start; gap: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 사내 휴가 규정을 언제든 확인할 수 있습니다.</li>
</ul>
</div>
<div style="margin-bottom: 40px;"><img style="width: 100%; border-radius: 8px;" src="/assets/leave_submit.png" alt="노션 휴가 신청 화면 대시보드" /></div>
</section>

<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">관리자 화면</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">관리자만 접근 가능하며, 전 직원의 휴가 현황을 한눈에 파악합니다.</p>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.7;">
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 새 멤버 추가 시 입사일만 입력하면 모든 세팅이 완료됩니다.</li>
<li style="display: flex; align-items: start; gap: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 현재 연차 기간의 발생, 사용, 잔여 연차가 자동 계산됩니다.</li>
</ul>
</div>
<div style="margin-bottom: 40px;"><img style="width: 100%; border-radius: 8px;" src="/assets/leave_mgmt.png" alt="노션 휴가 통합 관리자 화면" /></div>
</section>

<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">툴보다 중요한 것은 체계</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">여러 툴을 써보고 비교한 끝에 내린 결론은, 결국 중요한 것은 툴 자체가 아니라 업무 체계라는 것입니다.</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">노션은 그런 체계를 만들기에 충분히 유연한 도구였습니다. 물론 모든 것을 노션 하나로 해결하기보다는, 노션을 정보의 허브로 두고 구글 워크스페이스처럼 데이터와 파일 관리에 강한 도구를 함께 활용하는 방식이 더 적합했습니다.</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">여기에 Make, Claude 같은 자동화·AI 도구를 더하면 체계 위에 자동화가 자연스럽게 얹히고, 업무 히스토리와 맥락이 쌓이면서 AI 역시 더 효과적으로 활용할 수 있게 됩니다. 😀</p>
</section>

<p style="margin-top: 32px;"> </p>
<div style="background:#16102b; border-radius:16px; padding:36px 40px; display:flex; align-items:center; justify-content:space-between; gap:32px; border:1px solid #2e2250; margin-bottom:60px; flex-wrap:wrap;">
  <div>
    <div style="font-size:11px; font-weight:700; letter-spacing:0.1em; color:#a78bf6; margin-bottom:10px; text-transform:uppercase;">노션 운영 시스템</div>
    <h3 style="margin:0; font-size:20px; font-weight:900; color:#fff; line-height:1.6;">연차 계산부터 차감까지, <br>자동으로 돌아가는 휴가 관리 시스템</h3>
  </div>
  <a href="https://www.nsdlab.kr/main/?idx=8" target="_blank" style="display:inline-block; background:#8366EE; color:#fff; font-size:14px; font-weight:700; padding:14px 28px; border-radius:10px; text-decoration:none; white-space:nowrap; flex-shrink:0;">바로 구매하기 →</a>
</div>
</div>
