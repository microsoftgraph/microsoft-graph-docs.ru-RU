---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b7d236aa9b3cc0b6e20a90b646ba3a95eaf0d3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463325"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="d22e8-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="d22e8-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="d22e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d22e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d22e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d22e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d22e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d22e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d22e8-107">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d22e8-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="d22e8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d22e8-108">Members</span></span>
|<span data-ttu-id="d22e8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d22e8-109">Member</span></span>|<span data-ttu-id="d22e8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d22e8-110">Value</span></span>|<span data-ttu-id="d22e8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d22e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d22e8-112">Нет</span><span class="sxs-lookup"><span data-stu-id="d22e8-112">none</span></span>|<span data-ttu-id="d22e8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d22e8-113">0</span></span>|<span data-ttu-id="d22e8-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="d22e8-114">None.</span></span>|
|<span data-ttu-id="d22e8-115">апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="d22e8-115">appleFailure</span></span>|<span data-ttu-id="d22e8-116">1,1</span><span class="sxs-lookup"><span data-stu-id="d22e8-116">1</span></span>|<span data-ttu-id="d22e8-117">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="d22e8-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="d22e8-118">интерналеррор</span><span class="sxs-lookup"><span data-stu-id="d22e8-118">internalError</span></span>|<span data-ttu-id="d22e8-119">2</span><span class="sxs-lookup"><span data-stu-id="d22e8-119">2</span></span>|<span data-ttu-id="d22e8-120">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="d22e8-120">There was an internal error.</span></span>|
|<span data-ttu-id="d22e8-121">експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="d22e8-121">expiredVppToken</span></span>|<span data-ttu-id="d22e8-122">4</span><span class="sxs-lookup"><span data-stu-id="d22e8-122">3</span></span>|<span data-ttu-id="d22e8-123">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d22e8-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="d22e8-124">експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="d22e8-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="d22e8-125">4 </span><span class="sxs-lookup"><span data-stu-id="d22e8-125">4</span></span>|<span data-ttu-id="d22e8-126">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d22e8-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|



