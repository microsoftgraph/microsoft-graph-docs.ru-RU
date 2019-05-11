---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6dc39839754f24ae25044b0aa249d61fe2655d68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943035"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="7231d-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="7231d-103">complianceState enum type</span></span>

> <span data-ttu-id="7231d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7231d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7231d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7231d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7231d-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="7231d-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="7231d-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7231d-107">Members</span></span>
|<span data-ttu-id="7231d-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7231d-108">Member</span></span>|<span data-ttu-id="7231d-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7231d-109">Value</span></span>|<span data-ttu-id="7231d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7231d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7231d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="7231d-111">unknown</span></span>|<span data-ttu-id="7231d-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7231d-112">0</span></span>|<span data-ttu-id="7231d-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="7231d-113">Unknown.</span></span>|
|<span data-ttu-id="7231d-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="7231d-114">compliant</span></span>|<span data-ttu-id="7231d-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7231d-115">1</span></span>|<span data-ttu-id="7231d-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="7231d-116">Compliant.</span></span>|
|<span data-ttu-id="7231d-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="7231d-117">noncompliant</span></span>|<span data-ttu-id="7231d-118">2</span><span class="sxs-lookup"><span data-stu-id="7231d-118">2</span></span>|<span data-ttu-id="7231d-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7231d-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="7231d-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="7231d-120">conflict</span></span>|<span data-ttu-id="7231d-121">4</span><span class="sxs-lookup"><span data-stu-id="7231d-121">3</span></span>|<span data-ttu-id="7231d-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="7231d-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="7231d-123">error</span><span class="sxs-lookup"><span data-stu-id="7231d-123">error</span></span>|<span data-ttu-id="7231d-124">SP4</span><span class="sxs-lookup"><span data-stu-id="7231d-124">4</span></span>|<span data-ttu-id="7231d-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="7231d-125">Error.</span></span>|
|<span data-ttu-id="7231d-126">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="7231d-126">inGracePeriod</span></span>|<span data-ttu-id="7231d-127">254</span><span class="sxs-lookup"><span data-stu-id="7231d-127">254</span></span>|<span data-ttu-id="7231d-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="7231d-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="7231d-129">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="7231d-129">configManager</span></span>|<span data-ttu-id="7231d-130">255</span><span class="sxs-lookup"><span data-stu-id="7231d-130">255</span></span>|<span data-ttu-id="7231d-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="7231d-131">Managed by Config Manager</span></span>|




