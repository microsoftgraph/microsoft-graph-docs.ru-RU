---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83f39e4c795d57b6bb5aa5633ed481963419e041
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983290"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="856cd-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="856cd-103">complianceState enum type</span></span>

> <span data-ttu-id="856cd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="856cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="856cd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="856cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="856cd-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="856cd-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="856cd-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="856cd-107">Members</span></span>
|<span data-ttu-id="856cd-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="856cd-108">Member</span></span>|<span data-ttu-id="856cd-109">Значение</span><span class="sxs-lookup"><span data-stu-id="856cd-109">Value</span></span>|<span data-ttu-id="856cd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="856cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="856cd-111">unknown</span><span class="sxs-lookup"><span data-stu-id="856cd-111">unknown</span></span>|<span data-ttu-id="856cd-112">нуль</span><span class="sxs-lookup"><span data-stu-id="856cd-112">0</span></span>|<span data-ttu-id="856cd-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="856cd-113">Unknown.</span></span>|
|<span data-ttu-id="856cd-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="856cd-114">compliant</span></span>|<span data-ttu-id="856cd-115">1,1</span><span class="sxs-lookup"><span data-stu-id="856cd-115">1</span></span>|<span data-ttu-id="856cd-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="856cd-116">Compliant.</span></span>|
|<span data-ttu-id="856cd-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="856cd-117">noncompliant</span></span>|<span data-ttu-id="856cd-118">2</span><span class="sxs-lookup"><span data-stu-id="856cd-118">2</span></span>|<span data-ttu-id="856cd-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="856cd-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="856cd-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="856cd-120">conflict</span></span>|<span data-ttu-id="856cd-121">4</span><span class="sxs-lookup"><span data-stu-id="856cd-121">3</span></span>|<span data-ttu-id="856cd-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="856cd-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="856cd-123">error</span><span class="sxs-lookup"><span data-stu-id="856cd-123">error</span></span>|<span data-ttu-id="856cd-124">SP4</span><span class="sxs-lookup"><span data-stu-id="856cd-124">4</span></span>|<span data-ttu-id="856cd-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="856cd-125">Error.</span></span>|
|<span data-ttu-id="856cd-126">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="856cd-126">inGracePeriod</span></span>|<span data-ttu-id="856cd-127">254</span><span class="sxs-lookup"><span data-stu-id="856cd-127">254</span></span>|<span data-ttu-id="856cd-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="856cd-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="856cd-129">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="856cd-129">configManager</span></span>|<span data-ttu-id="856cd-130">255</span><span class="sxs-lookup"><span data-stu-id="856cd-130">255</span></span>|<span data-ttu-id="856cd-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="856cd-131">Managed by Config Manager</span></span>|





