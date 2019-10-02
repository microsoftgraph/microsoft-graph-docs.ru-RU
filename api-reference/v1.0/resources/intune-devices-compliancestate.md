---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01c0a3443eae87fb69b4b6482a2da2c2e067c5d1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357061"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="24302-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="24302-103">complianceState enum type</span></span>

> <span data-ttu-id="24302-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24302-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24302-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="24302-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="24302-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="24302-106">Members</span></span>
|<span data-ttu-id="24302-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="24302-107">Member</span></span>|<span data-ttu-id="24302-108">Значение</span><span class="sxs-lookup"><span data-stu-id="24302-108">Value</span></span>|<span data-ttu-id="24302-109">Описание</span><span class="sxs-lookup"><span data-stu-id="24302-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24302-110">unknown</span><span class="sxs-lookup"><span data-stu-id="24302-110">unknown</span></span>|<span data-ttu-id="24302-111">нуль</span><span class="sxs-lookup"><span data-stu-id="24302-111">0</span></span>|<span data-ttu-id="24302-112">Найден.</span><span class="sxs-lookup"><span data-stu-id="24302-112">Unknown.</span></span>|
|<span data-ttu-id="24302-113">совместимо</span><span class="sxs-lookup"><span data-stu-id="24302-113">compliant</span></span>|<span data-ttu-id="24302-114">1,1</span><span class="sxs-lookup"><span data-stu-id="24302-114">1</span></span>|<span data-ttu-id="24302-115">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="24302-115">Compliant.</span></span>|
|<span data-ttu-id="24302-116">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="24302-116">noncompliant</span></span>|<span data-ttu-id="24302-117">2</span><span class="sxs-lookup"><span data-stu-id="24302-117">2</span></span>|<span data-ttu-id="24302-118">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="24302-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="24302-119">противоречивы</span><span class="sxs-lookup"><span data-stu-id="24302-119">conflict</span></span>|<span data-ttu-id="24302-120">4</span><span class="sxs-lookup"><span data-stu-id="24302-120">3</span></span>|<span data-ttu-id="24302-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="24302-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="24302-122">error</span><span class="sxs-lookup"><span data-stu-id="24302-122">error</span></span>|<span data-ttu-id="24302-123">SP4</span><span class="sxs-lookup"><span data-stu-id="24302-123">4</span></span>|<span data-ttu-id="24302-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="24302-124">Error.</span></span>|
|<span data-ttu-id="24302-125">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="24302-125">inGracePeriod</span></span>|<span data-ttu-id="24302-126">254</span><span class="sxs-lookup"><span data-stu-id="24302-126">254</span></span>|<span data-ttu-id="24302-127">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="24302-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="24302-128">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="24302-128">configManager</span></span>|<span data-ttu-id="24302-129">255</span><span class="sxs-lookup"><span data-stu-id="24302-129">255</span></span>|<span data-ttu-id="24302-130">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="24302-130">Managed by Config Manager</span></span>|




