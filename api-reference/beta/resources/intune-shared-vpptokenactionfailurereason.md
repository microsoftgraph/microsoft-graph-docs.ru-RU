---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 144572ab0d18949ace682681a4939ca17a4538a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347845"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="18b7f-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="18b7f-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="18b7f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18b7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18b7f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18b7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b7f-106">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="18b7f-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="18b7f-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="18b7f-107">Members</span></span>
|<span data-ttu-id="18b7f-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="18b7f-108">Member</span></span>|<span data-ttu-id="18b7f-109">Значение</span><span class="sxs-lookup"><span data-stu-id="18b7f-109">Value</span></span>|<span data-ttu-id="18b7f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18b7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b7f-111">none</span><span class="sxs-lookup"><span data-stu-id="18b7f-111">none</span></span>|<span data-ttu-id="18b7f-112">нуль</span><span class="sxs-lookup"><span data-stu-id="18b7f-112">0</span></span>|<span data-ttu-id="18b7f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="18b7f-113">None.</span></span>|
|<span data-ttu-id="18b7f-114">апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="18b7f-114">appleFailure</span></span>|<span data-ttu-id="18b7f-115">1,1</span><span class="sxs-lookup"><span data-stu-id="18b7f-115">1</span></span>|<span data-ttu-id="18b7f-116">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="18b7f-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="18b7f-117">интерналеррор</span><span class="sxs-lookup"><span data-stu-id="18b7f-117">internalError</span></span>|<span data-ttu-id="18b7f-118">2</span><span class="sxs-lookup"><span data-stu-id="18b7f-118">2</span></span>|<span data-ttu-id="18b7f-119">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="18b7f-119">There was an internal error.</span></span>|
|<span data-ttu-id="18b7f-120">експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="18b7f-120">expiredVppToken</span></span>|<span data-ttu-id="18b7f-121">4</span><span class="sxs-lookup"><span data-stu-id="18b7f-121">3</span></span>|<span data-ttu-id="18b7f-122">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="18b7f-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="18b7f-123">експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="18b7f-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="18b7f-124">SP4</span><span class="sxs-lookup"><span data-stu-id="18b7f-124">4</span></span>|<span data-ttu-id="18b7f-125">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="18b7f-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|



