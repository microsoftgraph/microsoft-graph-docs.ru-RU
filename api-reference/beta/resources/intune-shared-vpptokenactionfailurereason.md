---
title: Тип перечисления vppTokenActionFailureReason
description: Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f488302b7fc701e8a419357ad7d6cbbb6015759b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883722"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="a68e6-103">Тип перечисления vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="a68e6-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="a68e6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a68e6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a68e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a68e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a68e6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a68e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a68e6-107">Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="a68e6-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="a68e6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="a68e6-108">Members</span></span>
|<span data-ttu-id="a68e6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="a68e6-109">Member</span></span>|<span data-ttu-id="a68e6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="a68e6-110">Value</span></span>|<span data-ttu-id="a68e6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a68e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a68e6-112">Нет</span><span class="sxs-lookup"><span data-stu-id="a68e6-112">none</span></span>|<span data-ttu-id="a68e6-113">0</span><span class="sxs-lookup"><span data-stu-id="a68e6-113">0</span></span>|<span data-ttu-id="a68e6-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="a68e6-114">None.</span></span>|
|<span data-ttu-id="a68e6-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="a68e6-115">appleFailure</span></span>|<span data-ttu-id="a68e6-116">1</span><span class="sxs-lookup"><span data-stu-id="a68e6-116">1</span></span>|<span data-ttu-id="a68e6-117">Произошла ошибка службы Apple.</span><span class="sxs-lookup"><span data-stu-id="a68e6-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="a68e6-118">internalError</span><span class="sxs-lookup"><span data-stu-id="a68e6-118">internalError</span></span>|<span data-ttu-id="a68e6-119">2</span><span class="sxs-lookup"><span data-stu-id="a68e6-119">2</span></span>|<span data-ttu-id="a68e6-120">Возникла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="a68e6-120">There was an internal error.</span></span>|
|<span data-ttu-id="a68e6-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="a68e6-121">expiredVppToken</span></span>|<span data-ttu-id="a68e6-122">3</span><span class="sxs-lookup"><span data-stu-id="a68e6-122">3</span></span>|<span data-ttu-id="a68e6-123">Произошла ошибка, так как истекших маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="a68e6-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="a68e6-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a68e6-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="a68e6-125">4</span><span class="sxs-lookup"><span data-stu-id="a68e6-125">4</span></span>|<span data-ttu-id="a68e6-126">Произошла ошибка истечения срока действия сертификата Push-уведомления Apple тома покупки программы.</span><span class="sxs-lookup"><span data-stu-id="a68e6-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





