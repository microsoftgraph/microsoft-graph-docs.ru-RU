---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1c243145ee8511edb001ba2a55b3f72dde070297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451288"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="2a7a3-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="2a7a3-103">complianceState enum type</span></span>

<span data-ttu-id="2a7a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a7a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a7a3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a7a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a7a3-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="2a7a3-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="2a7a3-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="2a7a3-107">Members</span></span>
|<span data-ttu-id="2a7a3-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="2a7a3-108">Member</span></span>|<span data-ttu-id="2a7a3-109">Значение</span><span class="sxs-lookup"><span data-stu-id="2a7a3-109">Value</span></span>|<span data-ttu-id="2a7a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a7a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a7a3-111">unknown</span><span class="sxs-lookup"><span data-stu-id="2a7a3-111">unknown</span></span>|<span data-ttu-id="2a7a3-112">нуль</span><span class="sxs-lookup"><span data-stu-id="2a7a3-112">0</span></span>|<span data-ttu-id="2a7a3-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="2a7a3-113">Unknown.</span></span>|
|<span data-ttu-id="2a7a3-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="2a7a3-114">compliant</span></span>|<span data-ttu-id="2a7a3-115">1,1</span><span class="sxs-lookup"><span data-stu-id="2a7a3-115">1</span></span>|<span data-ttu-id="2a7a3-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="2a7a3-116">Compliant.</span></span>|
|<span data-ttu-id="2a7a3-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="2a7a3-117">noncompliant</span></span>|<span data-ttu-id="2a7a3-118">2</span><span class="sxs-lookup"><span data-stu-id="2a7a3-118">2</span></span>|<span data-ttu-id="2a7a3-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2a7a3-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="2a7a3-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="2a7a3-120">conflict</span></span>|<span data-ttu-id="2a7a3-121">4</span><span class="sxs-lookup"><span data-stu-id="2a7a3-121">3</span></span>|<span data-ttu-id="2a7a3-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="2a7a3-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="2a7a3-123">error</span><span class="sxs-lookup"><span data-stu-id="2a7a3-123">error</span></span>|<span data-ttu-id="2a7a3-124">4 </span><span class="sxs-lookup"><span data-stu-id="2a7a3-124">4</span></span>|<span data-ttu-id="2a7a3-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="2a7a3-125">Error.</span></span>|
|<span data-ttu-id="2a7a3-126">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="2a7a3-126">inGracePeriod</span></span>|<span data-ttu-id="2a7a3-127">254</span><span class="sxs-lookup"><span data-stu-id="2a7a3-127">254</span></span>|<span data-ttu-id="2a7a3-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="2a7a3-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="2a7a3-129">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="2a7a3-129">configManager</span></span>|<span data-ttu-id="2a7a3-130">255</span><span class="sxs-lookup"><span data-stu-id="2a7a3-130">255</span></span>|<span data-ttu-id="2a7a3-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="2a7a3-131">Managed by Config Manager</span></span>|







