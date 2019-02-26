---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253360"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="ccc15-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="ccc15-103">complianceState enum type</span></span>

> <span data-ttu-id="ccc15-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccc15-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc15-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="ccc15-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="ccc15-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="ccc15-106">Members</span></span>
|<span data-ttu-id="ccc15-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="ccc15-107">Member</span></span>|<span data-ttu-id="ccc15-108">Значение</span><span class="sxs-lookup"><span data-stu-id="ccc15-108">Value</span></span>|<span data-ttu-id="ccc15-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ccc15-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccc15-110">unknown</span><span class="sxs-lookup"><span data-stu-id="ccc15-110">unknown</span></span>|<span data-ttu-id="ccc15-111">нуль</span><span class="sxs-lookup"><span data-stu-id="ccc15-111">0</span></span>|<span data-ttu-id="ccc15-112">Найден.</span><span class="sxs-lookup"><span data-stu-id="ccc15-112">Unknown.</span></span>|
|<span data-ttu-id="ccc15-113">совместимо</span><span class="sxs-lookup"><span data-stu-id="ccc15-113">compliant</span></span>|<span data-ttu-id="ccc15-114">1,1</span><span class="sxs-lookup"><span data-stu-id="ccc15-114">1</span></span>|<span data-ttu-id="ccc15-115">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="ccc15-115">Compliant.</span></span>|
|<span data-ttu-id="ccc15-116">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="ccc15-116">noncompliant</span></span>|<span data-ttu-id="ccc15-117">2</span><span class="sxs-lookup"><span data-stu-id="ccc15-117">2</span></span>|<span data-ttu-id="ccc15-118">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ccc15-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="ccc15-119">противоречивы</span><span class="sxs-lookup"><span data-stu-id="ccc15-119">conflict</span></span>|<span data-ttu-id="ccc15-120">4</span><span class="sxs-lookup"><span data-stu-id="ccc15-120">3</span></span>|<span data-ttu-id="ccc15-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="ccc15-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="ccc15-122">error</span><span class="sxs-lookup"><span data-stu-id="ccc15-122">error</span></span>|<span data-ttu-id="ccc15-123">4</span><span class="sxs-lookup"><span data-stu-id="ccc15-123">4</span></span>|<span data-ttu-id="ccc15-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="ccc15-124">Error.</span></span>|
|<span data-ttu-id="ccc15-125">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="ccc15-125">inGracePeriod</span></span>|<span data-ttu-id="ccc15-126">254</span><span class="sxs-lookup"><span data-stu-id="ccc15-126">254</span></span>|<span data-ttu-id="ccc15-127">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="ccc15-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="ccc15-128">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="ccc15-128">configManager</span></span>|<span data-ttu-id="ccc15-129">255</span><span class="sxs-lookup"><span data-stu-id="ccc15-129">255</span></span>|<span data-ttu-id="ccc15-130">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="ccc15-130">Managed by Config Manager</span></span>|



