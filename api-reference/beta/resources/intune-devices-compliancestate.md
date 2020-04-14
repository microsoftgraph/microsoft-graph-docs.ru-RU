---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c088f3a0fc3a4bd4b01f29da5f228920f00a398f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465145"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="dad4c-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="dad4c-103">complianceState enum type</span></span>

<span data-ttu-id="dad4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dad4c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dad4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dad4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad4c-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="dad4c-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="dad4c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dad4c-108">Members</span></span>
|<span data-ttu-id="dad4c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dad4c-109">Member</span></span>|<span data-ttu-id="dad4c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dad4c-110">Value</span></span>|<span data-ttu-id="dad4c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dad4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dad4c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="dad4c-112">unknown</span></span>|<span data-ttu-id="dad4c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="dad4c-113">0</span></span>|<span data-ttu-id="dad4c-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="dad4c-114">Unknown.</span></span>|
|<span data-ttu-id="dad4c-115">совместимо</span><span class="sxs-lookup"><span data-stu-id="dad4c-115">compliant</span></span>|<span data-ttu-id="dad4c-116">1,1</span><span class="sxs-lookup"><span data-stu-id="dad4c-116">1</span></span>|<span data-ttu-id="dad4c-117">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="dad4c-117">Compliant.</span></span>|
|<span data-ttu-id="dad4c-118">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="dad4c-118">noncompliant</span></span>|<span data-ttu-id="dad4c-119">2</span><span class="sxs-lookup"><span data-stu-id="dad4c-119">2</span></span>|<span data-ttu-id="dad4c-120">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dad4c-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="dad4c-121">противоречивы</span><span class="sxs-lookup"><span data-stu-id="dad4c-121">conflict</span></span>|<span data-ttu-id="dad4c-122">4</span><span class="sxs-lookup"><span data-stu-id="dad4c-122">3</span></span>|<span data-ttu-id="dad4c-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="dad4c-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="dad4c-124">error</span><span class="sxs-lookup"><span data-stu-id="dad4c-124">error</span></span>|<span data-ttu-id="dad4c-125">4 </span><span class="sxs-lookup"><span data-stu-id="dad4c-125">4</span></span>|<span data-ttu-id="dad4c-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="dad4c-126">Error.</span></span>|
|<span data-ttu-id="dad4c-127">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="dad4c-127">inGracePeriod</span></span>|<span data-ttu-id="dad4c-128">254</span><span class="sxs-lookup"><span data-stu-id="dad4c-128">254</span></span>|<span data-ttu-id="dad4c-129">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="dad4c-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="dad4c-130">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="dad4c-130">configManager</span></span>|<span data-ttu-id="dad4c-131">255</span><span class="sxs-lookup"><span data-stu-id="dad4c-131">255</span></span>|<span data-ttu-id="dad4c-132">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="dad4c-132">Managed by Config Manager</span></span>|



