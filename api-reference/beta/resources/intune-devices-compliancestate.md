---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c462df866b3c711bf4738c70ad4a1b0d68ceeb4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796271"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="fcf0e-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="fcf0e-103">complianceState enum type</span></span>

> <span data-ttu-id="fcf0e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcf0e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcf0e-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="fcf0e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="fcf0e-107">Members</span></span>
|<span data-ttu-id="fcf0e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="fcf0e-108">Member</span></span>|<span data-ttu-id="fcf0e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="fcf0e-109">Value</span></span>|<span data-ttu-id="fcf0e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcf0e-111">unknown</span><span class="sxs-lookup"><span data-stu-id="fcf0e-111">unknown</span></span>|<span data-ttu-id="fcf0e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="fcf0e-112">0</span></span>|<span data-ttu-id="fcf0e-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-113">Unknown.</span></span>|
|<span data-ttu-id="fcf0e-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="fcf0e-114">compliant</span></span>|<span data-ttu-id="fcf0e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="fcf0e-115">1</span></span>|<span data-ttu-id="fcf0e-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-116">Compliant.</span></span>|
|<span data-ttu-id="fcf0e-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="fcf0e-117">noncompliant</span></span>|<span data-ttu-id="fcf0e-118">2</span><span class="sxs-lookup"><span data-stu-id="fcf0e-118">2</span></span>|<span data-ttu-id="fcf0e-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="fcf0e-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="fcf0e-120">conflict</span></span>|<span data-ttu-id="fcf0e-121">4</span><span class="sxs-lookup"><span data-stu-id="fcf0e-121">3</span></span>|<span data-ttu-id="fcf0e-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="fcf0e-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="fcf0e-123">error</span><span class="sxs-lookup"><span data-stu-id="fcf0e-123">error</span></span>|<span data-ttu-id="fcf0e-124">SP4</span><span class="sxs-lookup"><span data-stu-id="fcf0e-124">4</span></span>|<span data-ttu-id="fcf0e-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="fcf0e-125">Error.</span></span>|
|<span data-ttu-id="fcf0e-126">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="fcf0e-126">inGracePeriod</span></span>|<span data-ttu-id="fcf0e-127">254</span><span class="sxs-lookup"><span data-stu-id="fcf0e-127">254</span></span>|<span data-ttu-id="fcf0e-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="fcf0e-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="fcf0e-129">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="fcf0e-129">configManager</span></span>|<span data-ttu-id="fcf0e-130">255</span><span class="sxs-lookup"><span data-stu-id="fcf0e-130">255</span></span>|<span data-ttu-id="fcf0e-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="fcf0e-131">Managed by Config Manager</span></span>|





