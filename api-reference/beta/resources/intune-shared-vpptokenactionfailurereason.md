---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 250b1d3939cb06947b60ea45de71d0843830effc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727119"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="84ea6-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="84ea6-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="84ea6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ea6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84ea6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84ea6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84ea6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84ea6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ea6-107">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="84ea6-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="84ea6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="84ea6-108">Members</span></span>
|<span data-ttu-id="84ea6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="84ea6-109">Member</span></span>|<span data-ttu-id="84ea6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="84ea6-110">Value</span></span>|<span data-ttu-id="84ea6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84ea6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ea6-112">none</span><span class="sxs-lookup"><span data-stu-id="84ea6-112">none</span></span>|<span data-ttu-id="84ea6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="84ea6-113">0</span></span>|<span data-ttu-id="84ea6-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="84ea6-114">None.</span></span>|
|<span data-ttu-id="84ea6-115">апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="84ea6-115">appleFailure</span></span>|<span data-ttu-id="84ea6-116">1,1</span><span class="sxs-lookup"><span data-stu-id="84ea6-116">1</span></span>|<span data-ttu-id="84ea6-117">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="84ea6-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="84ea6-118">интерналеррор</span><span class="sxs-lookup"><span data-stu-id="84ea6-118">internalError</span></span>|<span data-ttu-id="84ea6-119">2</span><span class="sxs-lookup"><span data-stu-id="84ea6-119">2</span></span>|<span data-ttu-id="84ea6-120">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="84ea6-120">There was an internal error.</span></span>|
|<span data-ttu-id="84ea6-121">експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="84ea6-121">expiredVppToken</span></span>|<span data-ttu-id="84ea6-122">4</span><span class="sxs-lookup"><span data-stu-id="84ea6-122">3</span></span>|<span data-ttu-id="84ea6-123">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="84ea6-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="84ea6-124">експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="84ea6-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="84ea6-125">4 </span><span class="sxs-lookup"><span data-stu-id="84ea6-125">4</span></span>|<span data-ttu-id="84ea6-126">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="84ea6-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





