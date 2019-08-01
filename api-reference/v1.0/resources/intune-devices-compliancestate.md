---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20890001aee15a56d5338964b931047033cf4a72
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030886"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="6afb3-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="6afb3-103">complianceState enum type</span></span>

> <span data-ttu-id="6afb3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6afb3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6afb3-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="6afb3-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="6afb3-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="6afb3-106">Members</span></span>
|<span data-ttu-id="6afb3-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="6afb3-107">Member</span></span>|<span data-ttu-id="6afb3-108">Значение</span><span class="sxs-lookup"><span data-stu-id="6afb3-108">Value</span></span>|<span data-ttu-id="6afb3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6afb3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6afb3-110">unknown</span><span class="sxs-lookup"><span data-stu-id="6afb3-110">unknown</span></span>|<span data-ttu-id="6afb3-111">нуль</span><span class="sxs-lookup"><span data-stu-id="6afb3-111">0</span></span>|<span data-ttu-id="6afb3-112">Найден.</span><span class="sxs-lookup"><span data-stu-id="6afb3-112">Unknown.</span></span>|
|<span data-ttu-id="6afb3-113">совместимо</span><span class="sxs-lookup"><span data-stu-id="6afb3-113">compliant</span></span>|<span data-ttu-id="6afb3-114">1,1</span><span class="sxs-lookup"><span data-stu-id="6afb3-114">1</span></span>|<span data-ttu-id="6afb3-115">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="6afb3-115">Compliant.</span></span>|
|<span data-ttu-id="6afb3-116">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="6afb3-116">noncompliant</span></span>|<span data-ttu-id="6afb3-117">2</span><span class="sxs-lookup"><span data-stu-id="6afb3-117">2</span></span>|<span data-ttu-id="6afb3-118">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6afb3-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="6afb3-119">противоречивы</span><span class="sxs-lookup"><span data-stu-id="6afb3-119">conflict</span></span>|<span data-ttu-id="6afb3-120">4</span><span class="sxs-lookup"><span data-stu-id="6afb3-120">3</span></span>|<span data-ttu-id="6afb3-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="6afb3-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="6afb3-122">error</span><span class="sxs-lookup"><span data-stu-id="6afb3-122">error</span></span>|<span data-ttu-id="6afb3-123">SP4</span><span class="sxs-lookup"><span data-stu-id="6afb3-123">4</span></span>|<span data-ttu-id="6afb3-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="6afb3-124">Error.</span></span>|
|<span data-ttu-id="6afb3-125">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="6afb3-125">inGracePeriod</span></span>|<span data-ttu-id="6afb3-126">254</span><span class="sxs-lookup"><span data-stu-id="6afb3-126">254</span></span>|<span data-ttu-id="6afb3-127">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="6afb3-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="6afb3-128">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="6afb3-128">configManager</span></span>|<span data-ttu-id="6afb3-129">255</span><span class="sxs-lookup"><span data-stu-id="6afb3-129">255</span></span>|<span data-ttu-id="6afb3-130">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="6afb3-130">Managed by Config Manager</span></span>|



