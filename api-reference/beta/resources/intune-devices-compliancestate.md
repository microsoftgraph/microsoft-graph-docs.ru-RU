---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1b0ba44c95a49d7646008ac4664926e257c02a19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785107"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="200ec-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="200ec-103">complianceState enum type</span></span>

> <span data-ttu-id="200ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="200ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="200ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="200ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="200ec-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="200ec-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="200ec-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="200ec-107">Members</span></span>
|<span data-ttu-id="200ec-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="200ec-108">Member</span></span>|<span data-ttu-id="200ec-109">Значение</span><span class="sxs-lookup"><span data-stu-id="200ec-109">Value</span></span>|<span data-ttu-id="200ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="200ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="200ec-111">unknown</span><span class="sxs-lookup"><span data-stu-id="200ec-111">unknown</span></span>|<span data-ttu-id="200ec-112">нуль</span><span class="sxs-lookup"><span data-stu-id="200ec-112">0</span></span>|<span data-ttu-id="200ec-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="200ec-113">Unknown.</span></span>|
|<span data-ttu-id="200ec-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="200ec-114">compliant</span></span>|<span data-ttu-id="200ec-115">1,1</span><span class="sxs-lookup"><span data-stu-id="200ec-115">1</span></span>|<span data-ttu-id="200ec-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="200ec-116">Compliant.</span></span>|
|<span data-ttu-id="200ec-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="200ec-117">noncompliant</span></span>|<span data-ttu-id="200ec-118">2</span><span class="sxs-lookup"><span data-stu-id="200ec-118">2</span></span>|<span data-ttu-id="200ec-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="200ec-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="200ec-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="200ec-120">conflict</span></span>|<span data-ttu-id="200ec-121">4</span><span class="sxs-lookup"><span data-stu-id="200ec-121">3</span></span>|<span data-ttu-id="200ec-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="200ec-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="200ec-123">error</span><span class="sxs-lookup"><span data-stu-id="200ec-123">error</span></span>|<span data-ttu-id="200ec-124">4 </span><span class="sxs-lookup"><span data-stu-id="200ec-124">4</span></span>|<span data-ttu-id="200ec-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="200ec-125">Error.</span></span>|
|<span data-ttu-id="200ec-126">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="200ec-126">inGracePeriod</span></span>|<span data-ttu-id="200ec-127">254</span><span class="sxs-lookup"><span data-stu-id="200ec-127">254</span></span>|<span data-ttu-id="200ec-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="200ec-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="200ec-129">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="200ec-129">configManager</span></span>|<span data-ttu-id="200ec-130">255</span><span class="sxs-lookup"><span data-stu-id="200ec-130">255</span></span>|<span data-ttu-id="200ec-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="200ec-131">Managed by Config Manager</span></span>|



