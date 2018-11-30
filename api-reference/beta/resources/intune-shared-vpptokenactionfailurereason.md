---
title: Тип перечисления vppTokenActionFailureReason
description: Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.
ms.openlocfilehash: 0fece0417a5585540f15e3f8a8631fd30eaa414e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077417"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="523fd-103">Тип перечисления vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="523fd-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="523fd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="523fd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="523fd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="523fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="523fd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="523fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="523fd-107">Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="523fd-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="523fd-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="523fd-108">Members</span></span>
|<span data-ttu-id="523fd-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="523fd-109">Member</span></span>|<span data-ttu-id="523fd-110">Значение</span><span class="sxs-lookup"><span data-stu-id="523fd-110">Value</span></span>|<span data-ttu-id="523fd-111">Description</span><span class="sxs-lookup"><span data-stu-id="523fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="523fd-112">Нет</span><span class="sxs-lookup"><span data-stu-id="523fd-112">none</span></span>|<span data-ttu-id="523fd-113">0</span><span class="sxs-lookup"><span data-stu-id="523fd-113">0</span></span>|<span data-ttu-id="523fd-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="523fd-114">None.</span></span>|
|<span data-ttu-id="523fd-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="523fd-115">appleFailure</span></span>|<span data-ttu-id="523fd-116">1</span><span class="sxs-lookup"><span data-stu-id="523fd-116">1</span></span>|<span data-ttu-id="523fd-117">Произошла ошибка службы Apple.</span><span class="sxs-lookup"><span data-stu-id="523fd-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="523fd-118">internalError</span><span class="sxs-lookup"><span data-stu-id="523fd-118">internalError</span></span>|<span data-ttu-id="523fd-119">2</span><span class="sxs-lookup"><span data-stu-id="523fd-119">2</span></span>|<span data-ttu-id="523fd-120">Возникла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="523fd-120">There was an internal error.</span></span>|
|<span data-ttu-id="523fd-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="523fd-121">expiredVppToken</span></span>|<span data-ttu-id="523fd-122">3</span><span class="sxs-lookup"><span data-stu-id="523fd-122">3</span></span>|<span data-ttu-id="523fd-123">Произошла ошибка, так как истекших маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="523fd-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="523fd-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="523fd-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="523fd-125">4</span><span class="sxs-lookup"><span data-stu-id="523fd-125">4</span></span>|<span data-ttu-id="523fd-126">Произошла ошибка истечения срока действия сертификата Push-уведомления Apple тома покупки программы.</span><span class="sxs-lookup"><span data-stu-id="523fd-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





