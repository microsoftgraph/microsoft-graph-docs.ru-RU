---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c462df866b3c711bf4738c70ad4a1b0d68ceeb4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549127"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="3f4b1-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="3f4b1-103">complianceState enum type</span></span>

> <span data-ttu-id="3f4b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f4b1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f4b1-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="3f4b1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3f4b1-107">Members</span></span>
|<span data-ttu-id="3f4b1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3f4b1-108">Member</span></span>|<span data-ttu-id="3f4b1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3f4b1-109">Value</span></span>|<span data-ttu-id="3f4b1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4b1-111">unknown</span><span class="sxs-lookup"><span data-stu-id="3f4b1-111">unknown</span></span>|<span data-ttu-id="3f4b1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3f4b1-112">0</span></span>|<span data-ttu-id="3f4b1-113">Найден.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-113">Unknown.</span></span>|
|<span data-ttu-id="3f4b1-114">совместимо</span><span class="sxs-lookup"><span data-stu-id="3f4b1-114">compliant</span></span>|<span data-ttu-id="3f4b1-115">1 </span><span class="sxs-lookup"><span data-stu-id="3f4b1-115">1</span></span>|<span data-ttu-id="3f4b1-116">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-116">Compliant.</span></span>|
|<span data-ttu-id="3f4b1-117">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="3f4b1-117">noncompliant</span></span>|<span data-ttu-id="3f4b1-118">2 </span><span class="sxs-lookup"><span data-stu-id="3f4b1-118">2</span></span>|<span data-ttu-id="3f4b1-119">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="3f4b1-120">противоречивы</span><span class="sxs-lookup"><span data-stu-id="3f4b1-120">conflict</span></span>|<span data-ttu-id="3f4b1-121">3 </span><span class="sxs-lookup"><span data-stu-id="3f4b1-121">3</span></span>|<span data-ttu-id="3f4b1-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="3f4b1-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="3f4b1-123">error</span><span class="sxs-lookup"><span data-stu-id="3f4b1-123">error</span></span>|<span data-ttu-id="3f4b1-124">4 </span><span class="sxs-lookup"><span data-stu-id="3f4b1-124">4</span></span>|<span data-ttu-id="3f4b1-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="3f4b1-125">Error.</span></span>|
|<span data-ttu-id="3f4b1-126">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="3f4b1-126">inGracePeriod</span></span>|<span data-ttu-id="3f4b1-127">254</span><span class="sxs-lookup"><span data-stu-id="3f4b1-127">254</span></span>|<span data-ttu-id="3f4b1-128">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="3f4b1-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="3f4b1-129">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="3f4b1-129">configManager</span></span>|<span data-ttu-id="3f4b1-130">255</span><span class="sxs-lookup"><span data-stu-id="3f4b1-130">255</span></span>|<span data-ttu-id="3f4b1-131">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="3f4b1-131">Managed by Config Manager</span></span>|





