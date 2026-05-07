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
<p style="text-align: left;"><img class="fr-fic fr-dii" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/9ac13702d8cab.png" alt="노션 썸네일 (2).png">
	<br>
</p>

<blockquote style="background-color: #F5F4F8; padding: 25px 30px; border-left: 5px solid #8366EE; border-radius: 8px; margin: 30px 0 30px 0; border-top: none; border-right: none; border-bottom: none; quotes: none;">

	<h2 style="font-size: 22px; font-weight: 700; color: rgb(131, 102, 238); margin-top: 0px; margin-bottom: 15px; display: flex; align-items: center; gap: 8px; line-height: 2;"><span style="font-size: 24px;">💡</span> 핵심 포인트</h2>

	<ul style="list-style: none; padding-left: 0; margin-bottom: 0; font-size: 18px; font-weight: 300; line-height: 1.7;">
		<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px; line-height: 1.15;"><span style="color: #8366EE; font-weight: bold;">✔️</span> <span style="color: rgb(0, 0, 0);">휴가 신청 &rarr; 승인 &rarr; 집계까지 한번에</span></li>
		<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px; line-height: 1.15;"><span style="color: rgb(0, 0, 0);"><span style="font-weight: bold;">✔️</span> 입사일 기준 발생&middot;잔여 연차가 자동 계산</span></li>
		<li style="display: flex; align-items: start; gap: 10px; line-height: 1.15;"><span style="color: rgb(0, 0, 0);"><span style="font-weight: bold;">✔️</span> 개인별 사용 현황과 잔여분을 한눈에 확인</span></li>
	</ul>
</blockquote>

<p style="margin-bottom: 18px; line-height: 2;"><a class="hello-world" href="https://nsdlab.imweb.me/module/?idx=8" rel="noopener noreferrer" style="border-radius: 15px; font-size: 18px; font-weight: 700; text-decoration: none; color: #8366EE;" target="_blank">👉 만들어진 시스템으로 바로 도입하기</a></p>
<section style="margin-bottom: 60px;">

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">
		<br>이 시스템은 실제로 만들어 몇 년간 사용한 사례입니다.
		<br>모든 체계를 갖추기 어려운 소규모 조직에 추천하며,</p>

	<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 18px; font-weight: 300; line-height: 1.7;">
		<li style="display: flex; align-items: center; gap: 10px; margin-bottom: 5px; line-height: 2;">&bull; 조직의 규모가 커지거나</li>
		<li style="display: flex; align-items: center; gap: 10px; margin-bottom: 18px; line-height: 2;">&bull; 근무 유형과 수당 구조가 복잡하다면</li>
		<li style="display: flex; align-items: center; gap: 10px; margin-bottom: 18px; line-height: 2;">전문 HR 솔루션을 함께 검토하는 것이 더 적합할 수 있습니다.</li>
		<li style="display: flex; align-items: center; gap: 10px; margin-bottom: 18px; line-height: 2;">
			<br>
		</li>
	</ul>
</section>
<section style="margin-bottom: 60px;">

	<h2 style="font-size: 24px; font-weight: 700; margin-bottom: 20px; line-height: 2;">1. 휴가 제도를 운영하는 방식</h2>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">어떤 제도를 운영하든, 구성원과의 합의와 기준을 명확히 하는 일은 중요합니다. &lsquo;우린 이렇게 할겁니다 땅땅!&rsquo; 못을 박고 회사도 멤버들도 규칙에 맞게 행동하는 것이죠.
		<br>그래서 모든 멤버가 접근하는 공통 페이지에 연차와 휴가 제도에 대해 최대한 자세히 정리해두었습니다.</p>
	<div style="margin-bottom: 18px; line-height: 2;"><img src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/fc9708dab314a.png" style="max-width: 100%; height: auto;" class="fr-fil fr-dib"></div>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">이 제도는 휴가 신청 페이지에도 한번 더 대문짝만하게 적어줍니다. 관련된 규칙은 무조건 실제로 행동이 일어나는 화면에도 함께 둬야 잘 지키더라구요 ㅎㅎ</p>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">
		<br>
	</p>
</section>
<section style="margin-bottom: 60px;">

	<h2 style="font-size: 24px; font-weight: 700; margin-bottom: 20px; line-height: 2;">2. 휴가 신청&middot;승인&middot;관리 페이지 구조</h2>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">휴가는 아래 두 개의 페이지를 중심으로 운영됩니다. 한 번 승인된 휴가 관리자 승인 없이 삭제할 수 없고, 모든 멤버의 휴가 내역과 잔여 연차는 별도 관리 페이지에서 한 눈에 확인할 수 있도록 구성했습니다.</p>
	<div style="background-color: #F9F9FB; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 18px;">

		<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;"><span style="color: rgb(131, 102, 238);">신청&middot;승인 (모든 멤버 접근 가능)</span></h3>

		<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 18px; font-weight: 300; line-height: 1.7;">
			<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 8px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 멤버가 휴가 신청</li>
			<li style="display: flex; align-items: start; gap: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 팀장이 알림을 받고 확인 후 승인</li>
		</ul>
	</div>
	<div style="margin-bottom: 30px; line-height: 2;"><img src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/0a776e2e00411.png" style="max-width: 100%; height: auto;" class="fr-fil fr-dib"></div>

	<p>
		<br>
	</p>

	<p>
		<br>
	</p>
	<div style="background-color: #F9F9FB; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 18px;">

		<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;"><span style="color: rgb(131, 102, 238);">통합 관리 (관리자만 접근 가능)</span></h3>

		<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 18px; font-weight: 300; line-height: 1.7;">
			<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 8px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 승인된 휴가는 멤버별 사용 리스트에 반영(자동)</li>
			<li style="display: flex; align-items: start; gap: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 멤버별 누적 휴가 현황에 집계(자동)</li>
		</ul>
	</div>
</section>
<section style="margin-bottom: 60px;">
	<div style="margin-bottom: 30px; line-height: 1.5;"><img src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/d5f2190231f3d.png" style="max-width: 100%; height: auto;" class="fr-fil fr-dib"></div>

	<h2 style="font-size: 24px; font-weight: 700; margin-bottom: 30px; line-height: 2;">
		<br>
	</h2>

	<h2 style="font-size: 24px; font-weight: 700; margin-bottom: 30px; line-height: 2;">3. 휴가&middot;연차가 적용되는 구조</h2>

	<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;">✔️ 휴가 및 경조사 종류</h3>
	<hr>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">내부 규정에 맞춰 휴가 유형별로 연차 소진 여부와 일수를 설정할 수 있습니다. 연차가 차감되지 않는 항목도 부재일로 기록해 공백 현황이 보이도록 구성했습니다.</p>
	<div style="margin-bottom: 40px; line-height: 2;"><img src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/5393b09733c8e.png" style="max-width: 100%; height: auto;" class="fr-fil fr-dib"></div>

	<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;">
		<br>
	</h3>

	<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;">✔️ 휴가 신청&middot;승인폼</h3>
	<hr>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">신청자는 아래 테이블을 통해 휴가를 신청하게 되는데요, 다음과 같은 역할을 합니다.</p>
	<div style="background-color: #F9F9FB; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 18px;">

		<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 18px; font-weight: 300; line-height: 1.7;">
			<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 신청자가 휴가 종류와 일자를 선택하면 연차 소진일이 계산됩니다.</li>
			<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 팀장이 승인을 완료하면 신청서에서 사라지고, 멤버별 휴가 사용 현황에 보관됩니다.</li>
			<li style="display: flex; align-items: start; gap: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">✓</span> 승인 요청을 받은 팀장이나, 승인 완료을 받은 신청자 모두 알림으로 알 수 있습니다.</li>
		</ul>
	</div>
	<div style="margin-bottom: 40px; line-height: 2;"><img src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/e6df517df96ba.png" style="max-width: 100%; height: auto;" class="fr-fil fr-dib"></div>

	<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;">
		<br>
	</h3>

	<h3 style="font-size: 20px; font-weight: 700; margin-bottom: 15px; line-height: 2;">✔️ 멤버별 누적 휴가 사용 리스트</h3>
	<hr>

	<p style="font-size: 18px; font-weight: 300; line-height: 2; margin-bottom: 18px;">멤버별로 근속연수에 따른 발생 연차, 사용 연차, 잔여 연차를 한 화면에서 관리할 수 있습니다.</p>
	<div style="background-color: #F9F9FB; border: 1px solid #EAEAEF; padding: 24px 30px; border-radius: 12px; margin-bottom: 18px;">

		<ul style="list-style: none; padding-left: 0; margin: 0; font-size: 18px; font-weight: 300; line-height: 1.7;">
			<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">발생 연차:</span> 입사일과 근속연수를 기준으로 재직 기간에 따른 연차가 자동 계산됩니다.</li>
			<li style="display: flex; align-items: start; gap: 10px; margin-bottom: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">사용 연차:</span> 연차 적용 기간 동안 사용한 모든 연차가 자동으로 집계됩니다.</li>
			<li style="display: flex; align-items: start; gap: 10px; line-height: 1.5;"><span style="color: #8366EE; font-weight: bold;">잔여 연차:</span> 발생 연차에서 사용 연차를 제외한 현재 기준 잔여 연차가 자동으로 계산됩니다.</li>
		</ul>
	</div>
	<div style="margin-bottom: 40px; line-height: 2;"><img src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/81e66832f5bd2.png" style="max-width: 100%; height: auto;" class="fr-fil fr-dib"></div>

	<p>
		<br>
	</p>

	<p>
		<br>
	</p>

	<p style="line-height: 2;"><span style="font-size: 18px;">사실 휴가 신청 관리 사례로 소개했지만,<br>결재 신청, 비용 승인 등 신청&ndash;승인&ndash;관리 흐름이 필요한 모든 프로세스에 그대로 적용할 수 있는 구조입니다.😀</span></p>
</section>

<p><img class="fr-dii" src="https://cdn.imweb.me/upload/S20260317e48e798a6d243/6014cf719f13b.png" style="width: 30px;"></p>

<p>
	<br>
</p>
