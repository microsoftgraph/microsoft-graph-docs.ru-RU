---
title: Тип перечисления vppTokenActionFailureReason
description: Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393146"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="57531-103">Тип перечисления vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="57531-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="57531-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57531-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57531-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57531-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57531-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57531-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57531-107">Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="57531-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="57531-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="57531-108">Members</span></span>
|<span data-ttu-id="57531-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="57531-109">Member</span></span>|<span data-ttu-id="57531-110">Значение</span><span class="sxs-lookup"><span data-stu-id="57531-110">Value</span></span>|<span data-ttu-id="57531-111">Описание</span><span class="sxs-lookup"><span data-stu-id="57531-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57531-112">none</span><span class="sxs-lookup"><span data-stu-id="57531-112">none</span></span>|<span data-ttu-id="57531-113">0</span><span class="sxs-lookup"><span data-stu-id="57531-113">0</span></span>|<span data-ttu-id="57531-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="57531-114">None.</span></span>|
|<span data-ttu-id="57531-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="57531-115">appleFailure</span></span>|<span data-ttu-id="57531-116">1</span><span class="sxs-lookup"><span data-stu-id="57531-116">1</span></span>|<span data-ttu-id="57531-117">Произошла ошибка службы Apple.</span><span class="sxs-lookup"><span data-stu-id="57531-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="57531-118">internalError</span><span class="sxs-lookup"><span data-stu-id="57531-118">internalError</span></span>|<span data-ttu-id="57531-119">2</span><span class="sxs-lookup"><span data-stu-id="57531-119">2</span></span>|<span data-ttu-id="57531-120">Возникла внутренняя ошибка.</span><span class="sxs-lookup"><span data-stu-id="57531-120">There was an internal error.</span></span>|
|<span data-ttu-id="57531-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="57531-121">expiredVppToken</span></span>|<span data-ttu-id="57531-122">3</span><span class="sxs-lookup"><span data-stu-id="57531-122">3</span></span>|<span data-ttu-id="57531-123">Произошла ошибка, так как истекших маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="57531-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="57531-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="57531-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="57531-125">4</span><span class="sxs-lookup"><span data-stu-id="57531-125">4</span></span>|<span data-ttu-id="57531-126">Произошла ошибка истечения срока действия сертификата Push-уведомления Apple тома покупки программы.</span><span class="sxs-lookup"><span data-stu-id="57531-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




