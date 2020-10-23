---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ed1a1ad0d6aee843eed4c1349dd2668f277e6c7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697772"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="64977-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="64977-103">complianceState enum type</span></span>

<span data-ttu-id="64977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64977-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64977-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64977-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64977-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64977-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64977-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="64977-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="64977-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="64977-108">Members</span></span>
|<span data-ttu-id="64977-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="64977-109">Member</span></span>|<span data-ttu-id="64977-110">Значение</span><span class="sxs-lookup"><span data-stu-id="64977-110">Value</span></span>|<span data-ttu-id="64977-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64977-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64977-112">unknown</span><span class="sxs-lookup"><span data-stu-id="64977-112">unknown</span></span>|<span data-ttu-id="64977-113">нуль</span><span class="sxs-lookup"><span data-stu-id="64977-113">0</span></span>|<span data-ttu-id="64977-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="64977-114">Unknown.</span></span>|
|<span data-ttu-id="64977-115">совместимо</span><span class="sxs-lookup"><span data-stu-id="64977-115">compliant</span></span>|<span data-ttu-id="64977-116">1,1</span><span class="sxs-lookup"><span data-stu-id="64977-116">1</span></span>|<span data-ttu-id="64977-117">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="64977-117">Compliant.</span></span>|
|<span data-ttu-id="64977-118">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="64977-118">noncompliant</span></span>|<span data-ttu-id="64977-119">2</span><span class="sxs-lookup"><span data-stu-id="64977-119">2</span></span>|<span data-ttu-id="64977-120">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="64977-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="64977-121">противоречивы</span><span class="sxs-lookup"><span data-stu-id="64977-121">conflict</span></span>|<span data-ttu-id="64977-122">4</span><span class="sxs-lookup"><span data-stu-id="64977-122">3</span></span>|<span data-ttu-id="64977-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="64977-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="64977-124">error</span><span class="sxs-lookup"><span data-stu-id="64977-124">error</span></span>|<span data-ttu-id="64977-125">4 </span><span class="sxs-lookup"><span data-stu-id="64977-125">4</span></span>|<span data-ttu-id="64977-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="64977-126">Error.</span></span>|
|<span data-ttu-id="64977-127">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="64977-127">inGracePeriod</span></span>|<span data-ttu-id="64977-128">254</span><span class="sxs-lookup"><span data-stu-id="64977-128">254</span></span>|<span data-ttu-id="64977-129">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="64977-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="64977-130">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="64977-130">configManager</span></span>|<span data-ttu-id="64977-131">255</span><span class="sxs-lookup"><span data-stu-id="64977-131">255</span></span>|<span data-ttu-id="64977-132">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="64977-132">Managed by Config Manager</span></span>|





