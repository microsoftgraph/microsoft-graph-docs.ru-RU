---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8765d0dd62579f470133e81005ff995638e00a5d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767101"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="13a5a-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="13a5a-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="13a5a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13a5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13a5a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13a5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a5a-106">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="13a5a-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="13a5a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="13a5a-107">Members</span></span>
|<span data-ttu-id="13a5a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="13a5a-108">Member</span></span>|<span data-ttu-id="13a5a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="13a5a-109">Value</span></span>|<span data-ttu-id="13a5a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13a5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a5a-111">none</span><span class="sxs-lookup"><span data-stu-id="13a5a-111">none</span></span>|<span data-ttu-id="13a5a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="13a5a-112">0</span></span>|<span data-ttu-id="13a5a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="13a5a-113">None.</span></span>|
|<span data-ttu-id="13a5a-114">апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="13a5a-114">appleFailure</span></span>|<span data-ttu-id="13a5a-115">1,1</span><span class="sxs-lookup"><span data-stu-id="13a5a-115">1</span></span>|<span data-ttu-id="13a5a-116">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="13a5a-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="13a5a-117">интерналеррор</span><span class="sxs-lookup"><span data-stu-id="13a5a-117">internalError</span></span>|<span data-ttu-id="13a5a-118">2</span><span class="sxs-lookup"><span data-stu-id="13a5a-118">2</span></span>|<span data-ttu-id="13a5a-119">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="13a5a-119">There was an internal error.</span></span>|
|<span data-ttu-id="13a5a-120">експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="13a5a-120">expiredVppToken</span></span>|<span data-ttu-id="13a5a-121">4</span><span class="sxs-lookup"><span data-stu-id="13a5a-121">3</span></span>|<span data-ttu-id="13a5a-122">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="13a5a-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="13a5a-123">експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="13a5a-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="13a5a-124">4 </span><span class="sxs-lookup"><span data-stu-id="13a5a-124">4</span></span>|<span data-ttu-id="13a5a-125">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="13a5a-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|



