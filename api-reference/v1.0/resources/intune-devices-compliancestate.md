---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 24f7a2a62ae45504c03d2fcff49ca8f17bfab28b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091308"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="a5ed2-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="a5ed2-103">complianceState enum type</span></span>

<span data-ttu-id="a5ed2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5ed2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5ed2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5ed2-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="a5ed2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a5ed2-107">Members</span></span>
|<span data-ttu-id="a5ed2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a5ed2-108">Member</span></span>|<span data-ttu-id="a5ed2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a5ed2-109">Value</span></span>|<span data-ttu-id="a5ed2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5ed2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5ed2-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a5ed2-111">unknown</span></span>|<span data-ttu-id="a5ed2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a5ed2-112">0</span></span>|<span data-ttu-id="a5ed2-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-113">Unknown.</span></span>|
|<span data-ttu-id="a5ed2-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="a5ed2-114">compliant</span></span>|<span data-ttu-id="a5ed2-115">1 </span><span class="sxs-lookup"><span data-stu-id="a5ed2-115">1</span></span>|<span data-ttu-id="a5ed2-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-116">Compliant.</span></span>|
|<span data-ttu-id="a5ed2-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="a5ed2-117">noncompliant</span></span>|<span data-ttu-id="a5ed2-118">2 </span><span class="sxs-lookup"><span data-stu-id="a5ed2-118">2</span></span>|<span data-ttu-id="a5ed2-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="a5ed2-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="a5ed2-120">conflict</span></span>|<span data-ttu-id="a5ed2-121">4</span><span class="sxs-lookup"><span data-stu-id="a5ed2-121">3</span></span>|<span data-ttu-id="a5ed2-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="a5ed2-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="a5ed2-123">error</span><span class="sxs-lookup"><span data-stu-id="a5ed2-123">error</span></span>|<span data-ttu-id="a5ed2-124">4 </span><span class="sxs-lookup"><span data-stu-id="a5ed2-124">4</span></span>|<span data-ttu-id="a5ed2-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="a5ed2-125">Error.</span></span>|
|<span data-ttu-id="a5ed2-126">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="a5ed2-126">inGracePeriod</span></span>|<span data-ttu-id="a5ed2-127">254</span><span class="sxs-lookup"><span data-stu-id="a5ed2-127">254</span></span>|<span data-ttu-id="a5ed2-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="a5ed2-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="a5ed2-129">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="a5ed2-129">configManager</span></span>|<span data-ttu-id="a5ed2-130">255</span><span class="sxs-lookup"><span data-stu-id="a5ed2-130">255</span></span>|<span data-ttu-id="a5ed2-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="a5ed2-131">Managed by Config Manager</span></span>|









