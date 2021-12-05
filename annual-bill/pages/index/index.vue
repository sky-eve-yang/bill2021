<template>
	<view class="content">
		<view class="img"></view>
		<view class="text-area">
			
			<swiper vertical="true" style="height: 100vh;width: 100vw;">
				<!-- 起始 -->
				<swiper-item class="startPage">
					<view style="height: 20vh;width: 100vw;;position: absolute;z-index: 2;display: flex;justify-content: center;align-items: center;">{{pagesElements.eatingPage.copywritingData.modifyingClause.lessCost}}</view>
					<image :src="pagesElements.eatingPage.imgsUrl.cateen3" style="position: absolute;z-index: 1;width: 100vw;height: 100vh;"  mode="aspectFit"></image>
					<image :src="pagesElements.eatingPage.imgsUrl.custom" style="position: relative;z-index: 5;width: 100vw;height: 100vh;"  mode="aspectFit"></image>
				</swiper-item>
				<!-- 吃饭 -->
				<swiper-item class="" style="width: 100vw;">
					22
				</swiper-item>
				<!-- 喝水 -->
				<swiper-item class="" style="width: 100vw;">
					21
				</swiper-item>
				<!-- 洗浴 -->
				<swiper-item class="" style="width: 100vw;">
					33
				</swiper-item>
				<!-- 校车 -->
				<swiper-item class="">
					<image :src="pagesElements.busPage.imgsUrl.custom"></image>
				</swiper-item>
				<!-- 超市 -->
				<swiper-item class="">
					
				</swiper-item>
				<!-- 游泳 -->
				<swiper-item class="">
					
				</swiper-item>
				<!-- 早晚 -->
				<swiper-item class="">
					
				</swiper-item>
				<!-- 多少 -->
				<swiper-item class="">
					
				</swiper-item>
				<!-- 总结 -->
				<swiper-item class="">
					
				</swiper-item>
			</swiper>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				pagesElements: {
					startingPage: {
						copywritingData: {
							modifyingClause: '嘀，点击猫爪进入年度账单',
						}
						
					},
					eatingPage: {
						copywritingData: {
							spendAmount: '',
							modifyingClause: {
								lessCost: '本喵靠意念吃饭  注定是食堂得不到的猫',
								averageCost: '小橘是一个合理进食  控制身材的好猫猫',
								muchCost: '干饭是本喵猫生的终极意义  有好吃的地方就一定有小橘',
							},
						},
						imgsUrl: {
							cateen1: '../../static/bill2021/eating/cateen1.png',
							cateen2: '../../static/bill2021/eating/cateen2.png',
							cateen3: '../../static/bill2021/eating/cateen3.png',
							custom: '../../static/bill2021/eating/custom cat.png',
							mush: '../../static/bill2021/eating/fat cat.png'
						}
						
					},
					drinkingPage: {
						copywritingData: {
							spendAmount: '',
							modifyingClause: {
								lessCost: '喝水在精不在多——  小橘说的对吧？',
								averageCost: '吨吨吨  本喵干了，你随意',
								muchCost: '猫不可一日无水  水乃猫身之源',
							},
						},
						imgsUrl: {
							less: '../../static/bill2021/drinking/little.png',
							custom: '../../static/bill2021/drinking/custom.png',
							mush: '../../static/bill2021/drinking/mush.png',
							tank: '../../static/bill2021/drinking/Water tank.png'
						},
						
					},
					bathingPage: {
						copywritingData: {
							spendAmount: '',
							modifyingClause: {
								lessCost: '洗浴这件事  随缘嘛~',
								averageCost: '有时间的时候  本喵就会来浴室视察一番哦',
								muchCost: '我爱洗澡，身体好好！  据说爱洗澡的喵运气都不会差哦~',
							},
						},
						imgsUrl: {
							lying: '../../static/bill2021/bathing/Lying cat.png',
							sitting: '../../static/bill2021/bathing/Sitting cat.png',
							bathtub: '../../static/bill2021/bathing/less/bathtub.png',
							cat: '../../static/bill2021/bathing/less/cat.png',
						},
						
					},
					busPage: {
						copywritingData: {
							spendAmount: '',
							modifyingClause: {
								lessCost: '非必要不出校  宅喵存在的意义就是“宅”',
								averageCost: '吃饱喝足不坐着校车去逛逛  是对猫生的浪费',
								muchCost: '走遍全世界  从坐着校车去兰州开始！',
							},
						},
						imgsUrl: {
							less: '../../static/bill2021/bus/little.png',
							custom: '../../static/bill2021/bus/custom.png',
							mush: '../../static/bill2021/bus/mush.png',
						},
						
					},
					marketPage: {
						copywritingData: {
							spendAmount: '',
							modifyingClause: {
								lessCost: '合理消费  是本喵矢志不渝的购物追求',
								averageCost: '好吃的~  都进本喵肚子里来吧！',
								muchCost: '这是一个让本喵来了就不想走的地方  下次一定控制自己，一定！',
							},
						},
						imgsUrlimgsUrl: {
							small: '../../static/bill2021/market/small back cat.png',
							big: '../../static/bill2021/market/big back cat.png',
							flying: '../../static/bill2021/market/flying Cat.png',
							pushing: '../../static/bill2021/market/pushing cat.png',
							road: '../../static/bill2021/market/road.png',
						},
						
					},
					swimmingPage: {
						copywritingData: {
							spendAmount: '',
							modifyingClause: {
								lessCost: '2021又是当废喵的一年  明年一定好好锻炼！',
								averageCost: '本喵兴致大发时  就要去玩水~',
								muchCost: '生命的意义在于运动  本喵要强身健体，做一只健康喵',
							},
						},
						imgsUrl: {
							pool: '../../static/bill2021/swimming/pool.png',
						},
						
					},
					dawnAndMidnightPage: {
						copywritingData: {
							spendAmountDawn: '',
							spendAmoutMidnight: '',
							modifyingClause: {
								DawnCost: '',
								MidnightCost: '',
							},
						},
						imgsUrl: {
							curtains: '../../static/bill2021/dawn-and-midnight/curtains.png'
						},
						
					},
					MostAndLeastPage: {
						copywritingData: {
							spendAmountLeast: '',
							spendAmountMost: '',
							modifyingClause: {
								leastCost: '',
								mostCost: '',
							},
						},
						imgsUrl: {
							least: '../../static/bill2021/min-and-max/min.png',
							most: '../../static/bill2021/min-and-max/max.png',
						},
						
					},
					summaryPage: {
						copywritingData: {
							spendAmount: '',
							modifyingTags: {
								eating: ['干饭喵','食堂得不到的喵'],
								drinking: ['吨吨喵','爱水喵','没水也行喵'],
								bathing: ['年度洗浴达人喵','浴室常驻喵','随缘洗浴喵'],
								bus: ['浪迹天涯喵','热爱出行喵','宅喵'],
								market: ['野性消费喵','购物达人喵','合理消费喵'],
								swimming: ['运动达人喵','强身健体喵','懒喵']
							},
						},
						imgsUrl: {
							circle: '../../static/bill2021/summary/circle.png',
							paws: '../../static/bill2021/summary/paws.png',
							QR: '../../static/bill2021/summary/QR code.png',
							male: '../../static/bill2021/summary/Male characters.png',
							female: '../../static/bill2021/summary/Female characters.png',
						},
						
					},
				}
			}
		},
		onLoad() {
			
		},
		methods: {
			
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		
	}

	.img{
	      width: 100rpx;
	      height: 100rpx;
		  bottom: 20rpx;
		  left: 20rpx;
	      position: absolute;
	      background-image: url('goat.gif');
		  transform: rotateY(180deg);
	      background-size: cover;
	      z-index: 100;
	      background-color: transparent;
	}
	
	.startPage {
		
	}
</style>
