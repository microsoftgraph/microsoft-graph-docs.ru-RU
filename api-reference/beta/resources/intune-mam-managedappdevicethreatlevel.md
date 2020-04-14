---
title: тип перечисления Манажедаппдевицесреатлевел
description: Уровень угроз максиум, разрешенный для приложения в соответствии с требованиями.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbecc5777380d69fd1b8ca64c84637d8d5490007
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43373078"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="6fc42-103">тип перечисления Манажедаппдевицесреатлевел</span><span class="sxs-lookup"><span data-stu-id="6fc42-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="6fc42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fc42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fc42-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fc42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fc42-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fc42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc42-107">Уровень угроз максиум, разрешенный для приложения в соответствии с требованиями.</span><span class="sxs-lookup"><span data-stu-id="6fc42-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="6fc42-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="6fc42-108">Members</span></span>
|<span data-ttu-id="6fc42-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="6fc42-109">Member</span></span>|<span data-ttu-id="6fc42-110">Значение</span><span class="sxs-lookup"><span data-stu-id="6fc42-110">Value</span></span>|<span data-ttu-id="6fc42-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6fc42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc42-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6fc42-112">notConfigured</span></span>|<span data-ttu-id="6fc42-113">нуль</span><span class="sxs-lookup"><span data-stu-id="6fc42-113">0</span></span>|<span data-ttu-id="6fc42-114">Значение не задано</span><span class="sxs-lookup"><span data-stu-id="6fc42-114">Value not configured</span></span>|
|<span data-ttu-id="6fc42-115">входящего</span><span class="sxs-lookup"><span data-stu-id="6fc42-115">secured</span></span>|<span data-ttu-id="6fc42-116">1,1</span><span class="sxs-lookup"><span data-stu-id="6fc42-116">1</span></span>|<span data-ttu-id="6fc42-117">Устройство не должно иметь угроз</span><span class="sxs-lookup"><span data-stu-id="6fc42-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="6fc42-118">потребление</span><span class="sxs-lookup"><span data-stu-id="6fc42-118">low</span></span>|<span data-ttu-id="6fc42-119">2</span><span class="sxs-lookup"><span data-stu-id="6fc42-119">2</span></span>|<span data-ttu-id="6fc42-120">Устройство должно иметь низкую угрозу.</span><span class="sxs-lookup"><span data-stu-id="6fc42-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="6fc42-121">medium</span><span class="sxs-lookup"><span data-stu-id="6fc42-121">medium</span></span>|<span data-ttu-id="6fc42-122">4</span><span class="sxs-lookup"><span data-stu-id="6fc42-122">3</span></span>|<span data-ttu-id="6fc42-123">Устройство должно иметь не более средней угрозы.</span><span class="sxs-lookup"><span data-stu-id="6fc42-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="6fc42-124">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="6fc42-124">high</span></span>|<span data-ttu-id="6fc42-125">4 </span><span class="sxs-lookup"><span data-stu-id="6fc42-125">4</span></span>|<span data-ttu-id="6fc42-126">Устройство должно иметь не более высоких угроз</span><span class="sxs-lookup"><span data-stu-id="6fc42-126">Device needs to have not more than high threat</span></span>|



