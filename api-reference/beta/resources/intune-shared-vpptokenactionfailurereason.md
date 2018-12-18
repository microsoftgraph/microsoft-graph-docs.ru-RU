---
title: Тип перечисления vppTokenActionFailureReason
description: Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.
author: tfitzmac
ms.openlocfilehash: f36b92238b097f50990bbdb2f3c3584b2ff48901
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320966"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="fdc68-103">Тип перечисления vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="fdc68-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="fdc68-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fdc68-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdc68-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdc68-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fdc68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdc68-107">Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="fdc68-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="fdc68-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fdc68-108">Members</span></span>
|<span data-ttu-id="fdc68-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fdc68-109">Member</span></span>|<span data-ttu-id="fdc68-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fdc68-110">Value</span></span>|<span data-ttu-id="fdc68-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc68-112">none</span><span class="sxs-lookup"><span data-stu-id="fdc68-112">none</span></span>|<span data-ttu-id="fdc68-113">0</span><span class="sxs-lookup"><span data-stu-id="fdc68-113">0</span></span>|<span data-ttu-id="fdc68-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fdc68-114">None.</span></span>|
|<span data-ttu-id="fdc68-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="fdc68-115">appleFailure</span></span>|<span data-ttu-id="fdc68-116">1</span><span class="sxs-lookup"><span data-stu-id="fdc68-116">1</span></span>|<span data-ttu-id="fdc68-117">Произошла ошибка службы Apple.</span><span class="sxs-lookup"><span data-stu-id="fdc68-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="fdc68-118">internalError</span><span class="sxs-lookup"><span data-stu-id="fdc68-118">internalError</span></span>|<span data-ttu-id="fdc68-119">2</span><span class="sxs-lookup"><span data-stu-id="fdc68-119">2</span></span>|<span data-ttu-id="fdc68-120">Возникла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="fdc68-120">There was an internal error.</span></span>|
|<span data-ttu-id="fdc68-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="fdc68-121">expiredVppToken</span></span>|<span data-ttu-id="fdc68-122">3</span><span class="sxs-lookup"><span data-stu-id="fdc68-122">3</span></span>|<span data-ttu-id="fdc68-123">Произошла ошибка, так как истекших маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="fdc68-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="fdc68-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="fdc68-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="fdc68-125">4</span><span class="sxs-lookup"><span data-stu-id="fdc68-125">4</span></span>|<span data-ttu-id="fdc68-126">Произошла ошибка истечения срока действия сертификата Push-уведомления Apple тома покупки программы.</span><span class="sxs-lookup"><span data-stu-id="fdc68-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





