---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f8aacb6fc6f95b8c8085a78ed2851b16622357
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990990"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="c3077-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="c3077-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="c3077-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3077-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3077-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3077-106">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="c3077-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="c3077-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="c3077-107">Members</span></span>
|<span data-ttu-id="c3077-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="c3077-108">Member</span></span>|<span data-ttu-id="c3077-109">Значение</span><span class="sxs-lookup"><span data-stu-id="c3077-109">Value</span></span>|<span data-ttu-id="c3077-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3077-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3077-111">none</span><span class="sxs-lookup"><span data-stu-id="c3077-111">none</span></span>|<span data-ttu-id="c3077-112">нуль</span><span class="sxs-lookup"><span data-stu-id="c3077-112">0</span></span>|<span data-ttu-id="c3077-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="c3077-113">None.</span></span>|
|<span data-ttu-id="c3077-114">Апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="c3077-114">appleFailure</span></span>|<span data-ttu-id="c3077-115">1,1</span><span class="sxs-lookup"><span data-stu-id="c3077-115">1</span></span>|<span data-ttu-id="c3077-116">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="c3077-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="c3077-117">Интерналеррор</span><span class="sxs-lookup"><span data-stu-id="c3077-117">internalError</span></span>|<span data-ttu-id="c3077-118">2</span><span class="sxs-lookup"><span data-stu-id="c3077-118">2</span></span>|<span data-ttu-id="c3077-119">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="c3077-119">There was an internal error.</span></span>|
|<span data-ttu-id="c3077-120">Експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="c3077-120">expiredVppToken</span></span>|<span data-ttu-id="c3077-121">4</span><span class="sxs-lookup"><span data-stu-id="c3077-121">3</span></span>|<span data-ttu-id="c3077-122">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="c3077-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="c3077-123">Експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="c3077-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="c3077-124">SP4</span><span class="sxs-lookup"><span data-stu-id="c3077-124">4</span></span>|<span data-ttu-id="c3077-125">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="c3077-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





