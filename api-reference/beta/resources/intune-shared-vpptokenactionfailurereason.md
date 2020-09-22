---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 883772d99077e8587ba5467ec8c9492eddfb62e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070676"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="10739-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="10739-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="10739-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10739-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10739-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10739-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10739-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10739-107">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="10739-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="10739-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="10739-108">Members</span></span>
|<span data-ttu-id="10739-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="10739-109">Member</span></span>|<span data-ttu-id="10739-110">Значение</span><span class="sxs-lookup"><span data-stu-id="10739-110">Value</span></span>|<span data-ttu-id="10739-111">Описание</span><span class="sxs-lookup"><span data-stu-id="10739-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10739-112">Нет</span><span class="sxs-lookup"><span data-stu-id="10739-112">none</span></span>|<span data-ttu-id="10739-113">нуль</span><span class="sxs-lookup"><span data-stu-id="10739-113">0</span></span>|<span data-ttu-id="10739-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="10739-114">None.</span></span>|
|<span data-ttu-id="10739-115">апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="10739-115">appleFailure</span></span>|<span data-ttu-id="10739-116">1 </span><span class="sxs-lookup"><span data-stu-id="10739-116">1</span></span>|<span data-ttu-id="10739-117">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="10739-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="10739-118">интерналеррор</span><span class="sxs-lookup"><span data-stu-id="10739-118">internalError</span></span>|<span data-ttu-id="10739-119">2 </span><span class="sxs-lookup"><span data-stu-id="10739-119">2</span></span>|<span data-ttu-id="10739-120">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="10739-120">There was an internal error.</span></span>|
|<span data-ttu-id="10739-121">експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="10739-121">expiredVppToken</span></span>|<span data-ttu-id="10739-122">4</span><span class="sxs-lookup"><span data-stu-id="10739-122">3</span></span>|<span data-ttu-id="10739-123">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="10739-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="10739-124">експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="10739-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="10739-125">4 </span><span class="sxs-lookup"><span data-stu-id="10739-125">4</span></span>|<span data-ttu-id="10739-126">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="10739-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|






