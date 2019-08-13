---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 18149f0493f1591c59e5bef98dc9a36f148a600c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319211"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="58c12-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="58c12-103">complianceState enum type</span></span>

> <span data-ttu-id="58c12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58c12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58c12-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58c12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58c12-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="58c12-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="58c12-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="58c12-107">Members</span></span>
|<span data-ttu-id="58c12-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="58c12-108">Member</span></span>|<span data-ttu-id="58c12-109">Значение</span><span class="sxs-lookup"><span data-stu-id="58c12-109">Value</span></span>|<span data-ttu-id="58c12-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58c12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c12-111">unknown</span><span class="sxs-lookup"><span data-stu-id="58c12-111">unknown</span></span>|<span data-ttu-id="58c12-112">нуль</span><span class="sxs-lookup"><span data-stu-id="58c12-112">0</span></span>|<span data-ttu-id="58c12-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="58c12-113">Unknown.</span></span>|
|<span data-ttu-id="58c12-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="58c12-114">compliant</span></span>|<span data-ttu-id="58c12-115">1,1</span><span class="sxs-lookup"><span data-stu-id="58c12-115">1</span></span>|<span data-ttu-id="58c12-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="58c12-116">Compliant.</span></span>|
|<span data-ttu-id="58c12-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="58c12-117">noncompliant</span></span>|<span data-ttu-id="58c12-118">2</span><span class="sxs-lookup"><span data-stu-id="58c12-118">2</span></span>|<span data-ttu-id="58c12-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58c12-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="58c12-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="58c12-120">conflict</span></span>|<span data-ttu-id="58c12-121">4</span><span class="sxs-lookup"><span data-stu-id="58c12-121">3</span></span>|<span data-ttu-id="58c12-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="58c12-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="58c12-123">error</span><span class="sxs-lookup"><span data-stu-id="58c12-123">error</span></span>|<span data-ttu-id="58c12-124">SP4</span><span class="sxs-lookup"><span data-stu-id="58c12-124">4</span></span>|<span data-ttu-id="58c12-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="58c12-125">Error.</span></span>|
|<span data-ttu-id="58c12-126">инграцепериод</span><span class="sxs-lookup"><span data-stu-id="58c12-126">inGracePeriod</span></span>|<span data-ttu-id="58c12-127">254</span><span class="sxs-lookup"><span data-stu-id="58c12-127">254</span></span>|<span data-ttu-id="58c12-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="58c12-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="58c12-129">конфигманажер</span><span class="sxs-lookup"><span data-stu-id="58c12-129">configManager</span></span>|<span data-ttu-id="58c12-130">255</span><span class="sxs-lookup"><span data-stu-id="58c12-130">255</span></span>|<span data-ttu-id="58c12-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="58c12-131">Managed by Config Manager</span></span>|



