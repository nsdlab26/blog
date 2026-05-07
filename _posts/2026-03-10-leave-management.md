---
layout: post
title: "[운영 체계 #4] 자동 계산되는 휴가 신청·승인 시스템 "
slug: leave-management
category: 운영 시스템
cover: https://cdn.imweb.me/upload/S20260317e48e798a6d243/9ac13702d8cab.png
date: 2026-03-10
meta_title: "[운영 체계 #4] 자동 계산되는 휴가 신청·승인 시스템 "
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
<p style="margin-bottom: 32px;"><a style="font-size: 16px; font-weight: bold; text-decoration: none; color: #8366ee;" href="https://nsdlab.imweb.me/module/?idx=8" target="_blank" rel="noopener noreferrer">👉 만들어진 시스템으로 바로 도입하기</a></p>
<section style="margin-bottom: 60px;">
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">이 시스템은 실제로 만들어 몇 년간 사용한 사례입니다.<br /> 모든 체계를 갖추기 어려운 소규모 조직에 추천하며, 다음과 같은 경우 전문 HR 솔루션을 검토하는 것이 적합할 수 있습니다.</p>
<ul style="list-style: none; padding-left: 15px; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27;">
<li>• 조직의 규모가 커지거나</li>
<li>• 근무 유형과 수당 구조가 복잡한 경우</li>
<li></li>
</ul>
</section>
<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">1. 휴가 제도를 운영하는 방식</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">어떤 제도를 운영하든, 구성원과의 합의와 기준을 명확히 하는 일은 중요합니다. 회사도 멤버들도 규칙에 맞게 행동하도록 모든 멤버가 접근하는 공통 페이지에 연차와 휴가 제도에 대해 최대한 자세히 정리해두었습니다.</p>
<div style="margin-bottom: 18px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/fc9708dab314a.png" alt="" /></div>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 0;">이 제도는 휴가 신청 페이지에도 대문짝만하게 적어줍니다. 관련된 규칙은 무조건 실제로 행동이 일어나는 화면에도 함께 둬야 잘 지키더라고요 ㅎㅎ</p>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 0;"> </p>
</section>
<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 20px; color: #1a1f27; line-height: 1.5;">2. 휴가 신청·승인·관리 페이지 구조</h2>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 24px;">휴가는 아래 두 개의 페이지를 중심으로 운영됩니다. 승인된 휴가는 관리자 권한 없이 삭제할 수 없고, 모든 내역은 별도 관리 페이지에서 한눈에 확인 가능합니다.</p>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #8366ee;">신청·승인 (모든 멤버 접근 가능)</h3>
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.6;">
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 멤버가 휴가 신청</li>
<li style="display: flex; align-items: start; gap: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 팀장이 알림을 받고 확인 후 승인</li>
</ul>
</div>
<div style="margin-bottom: 40px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/0a776e2e00411.png" alt="" /></div>
<div style="margin-bottom: 40px;"> </div>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #8366ee;">통합 관리 (관리자만 접근 가능)</h3>
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.6;">
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 승인된 휴가는 멤버별 사용 리스트에 자동 반영</li>
<li style="display: flex; align-items: start; gap: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 멤버별 누적 휴가 현황에 자동 집계</li>
</ul>
</div>
<div style="margin-bottom: 18px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/d5f2190231f3d.png" alt="" /></div>
</section>
<section style="margin-bottom: 60px;">
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 24px; color: #1a1f27; line-height: 1.5;"> </h2>
<h2 style="font-size: 22px; font-weight: bold; margin-bottom: 24px; color: #1a1f27; line-height: 1.5;">3. 휴가·연차가 적용되는 구조</h2>
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #1a1f27;"> </h3>
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #1a1f27;">✔️ 휴가 및 경조사 종류</h3>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">내부 규정에 맞춰 유형별 소진 여부와 일수를 설정할 수 있습니다. 연차가 차감되지 않는 항목도 부재일로 기록해 공백 현황이 보이도록 구성했습니다.</p>
<div style="margin-bottom: 48px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/5393b09733c8e.png" alt="" /></div>
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #1a1f27;"> </h3>
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #1a1f27;">✔️ 휴가 신청·승인폼</h3>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">신청자가 테이블을 통해 신청하면 다음과 같은 자동화가 일어납니다.</p>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.7;">
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 10px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 휴가 종류와 일자를 선택하면 연차 소진일이 자동 계산됩니다.</li>
<li style="display: flex; align-items: start; gap: 8px; margin-bottom: 10px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 팀장이 승인하면 신청서에서 사라지고 보관함으로 이동합니다.</li>
<li style="display: flex; align-items: start; gap: 8px;"><span style="color: #8366ee; font-weight: bold;">✓</span> 승인 요청 및 완료 시 관계자 모두에게 알림이 전송됩니다.</li>
</ul>
</div>
<div style="margin-bottom: 48px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/e6df517df96ba.png" alt="" /></div>
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #1a1f27;"> </h3>
<h3 style="font-size: 18px; font-weight: bold; margin-bottom: 12px; color: #1a1f27;">✔️ 멤버별 누적 휴가 사용 리스트</h3>
<p style="font-size: 16px; font-weight: 400; line-height: 1.8; color: #1a1f27; margin-bottom: 18px;">근속연수에 따른 발생, 사용, 잔여 연차를 한 화면에서 관리합니다.</p>
<div style="background-color: #f9f9fb; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 24px;">
<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 16px; font-weight: 400; line-height: 1.7;">
<li style="margin-bottom: 10px;"><strong style="color: #8366ee;">발생 연차:</strong> 입사일 기준으로 재직 기간에 따른 연차 자동 계산</li>
<li style="margin-bottom: 10px;"><strong style="color: #8366ee;">사용 연차:</strong> 승인된 모든 연차 내역 자동 집계</li>
<li><strong style="color: #8366ee;">잔여 연차:</strong> 발생에서 사용을 제외한 현재 기준 잔여분 자동 계산</li>
</ul>
</div>
<div style="margin-bottom: 40px;"><img style="width: 100%; border-radius: 8px;" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/81e66832f5bd2.png" alt="" /></div>
<div style="margin-bottom: 40px;"> </div>
<div style="font-size: 16px; line-height: 1.8; color: #1a1f27; background-color: #f5f4f8; padding: 25px 30px; border-radius: 12px; text-align: left; font-weight: 400;">사실 휴가 신청 사례로 소개했지만, 결재 신청이나 비용 승인 등 <strong style="font-weight: bold;">신청-승인-관리 흐름이 필요한 모든 프로세스</strong>에 그대로 적용할 수 있는 구조입니다. 😀</div>
</section>
<p style="margin-top: 32px;"> </p>
</div>
