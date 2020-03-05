---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78dc7dfee02a1b1670a2259d20465d4660e73a08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525154"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="2f582-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="2f582-103">complianceState enum type</span></span>

<span data-ttu-id="2f582-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2f582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f582-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f582-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f582-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f582-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f582-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="2f582-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="2f582-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2f582-108">Members</span></span>
|<span data-ttu-id="2f582-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2f582-109">Member</span></span>|<span data-ttu-id="2f582-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2f582-110">Value</span></span>|<span data-ttu-id="2f582-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f582-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f582-112">unknown</span><span class="sxs-lookup"><span data-stu-id="2f582-112">unknown</span></span>|<span data-ttu-id="2f582-113">нуль</span><span class="sxs-lookup"><span data-stu-id="2f582-113">0</span></span>|<span data-ttu-id="2f582-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="2f582-114">Unknown.</span></span>|
|<span data-ttu-id="2f582-115">совместимо</span><span class="sxs-lookup"><span data-stu-id="2f582-115">compliant</span></span>|<span data-ttu-id="2f582-116">1 </span><span class="sxs-lookup"><span data-stu-id="2f582-116">1</span></span>|<span data-ttu-id="2f582-117">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="2f582-117">Compliant.</span></span>|
|<span data-ttu-id="2f582-118">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="2f582-118">noncompliant</span></span>|<span data-ttu-id="2f582-119">2 </span><span class="sxs-lookup"><span data-stu-id="2f582-119">2</span></span>|<span data-ttu-id="2f582-120">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2f582-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="2f582-121">противоречивы</span><span class="sxs-lookup"><span data-stu-id="2f582-121">conflict</span></span>|<span data-ttu-id="2f582-122">3 </span><span class="sxs-lookup"><span data-stu-id="2f582-122">3</span></span>|<span data-ttu-id="2f582-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="2f582-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="2f582-124">error</span><span class="sxs-lookup"><span data-stu-id="2f582-124">error</span></span>|<span data-ttu-id="2f582-125">4 </span><span class="sxs-lookup"><span data-stu-id="2f582-125">4</span></span>|<span data-ttu-id="2f582-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="2f582-126">Error.</span></span>|
|<span data-ttu-id="2f582-127">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="2f582-127">inGracePeriod</span></span>|<span data-ttu-id="2f582-128">254</span><span class="sxs-lookup"><span data-stu-id="2f582-128">254</span></span>|<span data-ttu-id="2f582-129">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="2f582-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="2f582-130">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="2f582-130">configManager</span></span>|<span data-ttu-id="2f582-131">255</span><span class="sxs-lookup"><span data-stu-id="2f582-131">255</span></span>|<span data-ttu-id="2f582-132">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="2f582-132">Managed by Config Manager</span></span>|



