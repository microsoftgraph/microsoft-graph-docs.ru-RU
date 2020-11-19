---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a4bff788ff7bed5b06d5efac8247bc55e195c762
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214630"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="e0209-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="e0209-103">complianceState enum type</span></span>

<span data-ttu-id="e0209-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0209-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0209-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0209-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0209-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0209-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0209-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="e0209-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="e0209-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e0209-108">Members</span></span>
|<span data-ttu-id="e0209-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e0209-109">Member</span></span>|<span data-ttu-id="e0209-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e0209-110">Value</span></span>|<span data-ttu-id="e0209-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0209-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0209-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e0209-112">unknown</span></span>|<span data-ttu-id="e0209-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e0209-113">0</span></span>|<span data-ttu-id="e0209-114">Найден.</span><span class="sxs-lookup"><span data-stu-id="e0209-114">Unknown.</span></span>|
|<span data-ttu-id="e0209-115">совместимо</span><span class="sxs-lookup"><span data-stu-id="e0209-115">compliant</span></span>|<span data-ttu-id="e0209-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e0209-116">1</span></span>|<span data-ttu-id="e0209-117">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="e0209-117">Compliant.</span></span>|
|<span data-ttu-id="e0209-118">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="e0209-118">noncompliant</span></span>|<span data-ttu-id="e0209-119">2</span><span class="sxs-lookup"><span data-stu-id="e0209-119">2</span></span>|<span data-ttu-id="e0209-120">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e0209-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="e0209-121">противоречивы</span><span class="sxs-lookup"><span data-stu-id="e0209-121">conflict</span></span>|<span data-ttu-id="e0209-122">4</span><span class="sxs-lookup"><span data-stu-id="e0209-122">3</span></span>|<span data-ttu-id="e0209-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="e0209-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="e0209-124">error</span><span class="sxs-lookup"><span data-stu-id="e0209-124">error</span></span>|<span data-ttu-id="e0209-125">4 </span><span class="sxs-lookup"><span data-stu-id="e0209-125">4</span></span>|<span data-ttu-id="e0209-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="e0209-126">Error.</span></span>|
|<span data-ttu-id="e0209-127">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="e0209-127">inGracePeriod</span></span>|<span data-ttu-id="e0209-128">254</span><span class="sxs-lookup"><span data-stu-id="e0209-128">254</span></span>|<span data-ttu-id="e0209-129">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="e0209-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="e0209-130">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="e0209-130">configManager</span></span>|<span data-ttu-id="e0209-131">255</span><span class="sxs-lookup"><span data-stu-id="e0209-131">255</span></span>|<span data-ttu-id="e0209-132">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="e0209-132">Managed by Config Manager</span></span>|




