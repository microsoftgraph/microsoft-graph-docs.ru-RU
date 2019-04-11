---
title: тип перечисления Впптокенактионфаилуререасон
description: Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9adb896d384be99496c016ef3bd39b02ff1a28e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798532"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="53f86-103">тип перечисления Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="53f86-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="53f86-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53f86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53f86-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f86-106">Возможные типы причин сбоя действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="53f86-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="53f86-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="53f86-107">Members</span></span>
|<span data-ttu-id="53f86-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="53f86-108">Member</span></span>|<span data-ttu-id="53f86-109">Значение</span><span class="sxs-lookup"><span data-stu-id="53f86-109">Value</span></span>|<span data-ttu-id="53f86-110">Описание</span><span class="sxs-lookup"><span data-stu-id="53f86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f86-111">нет</span><span class="sxs-lookup"><span data-stu-id="53f86-111">none</span></span>|<span data-ttu-id="53f86-112">нуль</span><span class="sxs-lookup"><span data-stu-id="53f86-112">0</span></span>|<span data-ttu-id="53f86-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="53f86-113">None.</span></span>|
|<span data-ttu-id="53f86-114">Апплефаилуре</span><span class="sxs-lookup"><span data-stu-id="53f86-114">appleFailure</span></span>|<span data-ttu-id="53f86-115">1,1</span><span class="sxs-lookup"><span data-stu-id="53f86-115">1</span></span>|<span data-ttu-id="53f86-116">В службе Apple возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="53f86-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="53f86-117">Интерналеррор</span><span class="sxs-lookup"><span data-stu-id="53f86-117">internalError</span></span>|<span data-ttu-id="53f86-118">2</span><span class="sxs-lookup"><span data-stu-id="53f86-118">2</span></span>|<span data-ttu-id="53f86-119">Произошла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="53f86-119">There was an internal error.</span></span>|
|<span data-ttu-id="53f86-120">Експиредвпптокен</span><span class="sxs-lookup"><span data-stu-id="53f86-120">expiredVppToken</span></span>|<span data-ttu-id="53f86-121">4</span><span class="sxs-lookup"><span data-stu-id="53f86-121">3</span></span>|<span data-ttu-id="53f86-122">Произошла ошибка из-за истечения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="53f86-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="53f86-123">Експиредапплепушнотификатионцертификате</span><span class="sxs-lookup"><span data-stu-id="53f86-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="53f86-124">SP4</span><span class="sxs-lookup"><span data-stu-id="53f86-124">4</span></span>|<span data-ttu-id="53f86-125">Произошла ошибка из-за истечения срока действия сертификата push-уведомлений Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="53f86-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





