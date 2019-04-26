---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568140"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="661da-103">тип перечисления Комплианцестате</span><span class="sxs-lookup"><span data-stu-id="661da-103">complianceState enum type</span></span>

> <span data-ttu-id="661da-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="661da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="661da-105">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="661da-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="661da-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="661da-106">Members</span></span>
|<span data-ttu-id="661da-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="661da-107">Member</span></span>|<span data-ttu-id="661da-108">Значение</span><span class="sxs-lookup"><span data-stu-id="661da-108">Value</span></span>|<span data-ttu-id="661da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="661da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="661da-110">unknown</span><span class="sxs-lookup"><span data-stu-id="661da-110">unknown</span></span>|<span data-ttu-id="661da-111">нуль</span><span class="sxs-lookup"><span data-stu-id="661da-111">0</span></span>|<span data-ttu-id="661da-112">Найден.</span><span class="sxs-lookup"><span data-stu-id="661da-112">Unknown.</span></span>|
|<span data-ttu-id="661da-113">совместимо</span><span class="sxs-lookup"><span data-stu-id="661da-113">compliant</span></span>|<span data-ttu-id="661da-114">1 </span><span class="sxs-lookup"><span data-stu-id="661da-114">1</span></span>|<span data-ttu-id="661da-115">Совместимо.</span><span class="sxs-lookup"><span data-stu-id="661da-115">Compliant.</span></span>|
|<span data-ttu-id="661da-116">несоответствующих</span><span class="sxs-lookup"><span data-stu-id="661da-116">noncompliant</span></span>|<span data-ttu-id="661da-117">2 </span><span class="sxs-lookup"><span data-stu-id="661da-117">2</span></span>|<span data-ttu-id="661da-118">Устройство не совместимо и заблокировано из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="661da-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="661da-119">противоречивы</span><span class="sxs-lookup"><span data-stu-id="661da-119">conflict</span></span>|<span data-ttu-id="661da-120">3 </span><span class="sxs-lookup"><span data-stu-id="661da-120">3</span></span>|<span data-ttu-id="661da-121">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="661da-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="661da-122">error</span><span class="sxs-lookup"><span data-stu-id="661da-122">error</span></span>|<span data-ttu-id="661da-123">4 </span><span class="sxs-lookup"><span data-stu-id="661da-123">4</span></span>|<span data-ttu-id="661da-124">Ошибка</span><span class="sxs-lookup"><span data-stu-id="661da-124">Error.</span></span>|
|<span data-ttu-id="661da-125">Инграцепериод</span><span class="sxs-lookup"><span data-stu-id="661da-125">inGracePeriod</span></span>|<span data-ttu-id="661da-126">254</span><span class="sxs-lookup"><span data-stu-id="661da-126">254</span></span>|<span data-ttu-id="661da-127">Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="661da-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="661da-128">Конфигманажер</span><span class="sxs-lookup"><span data-stu-id="661da-128">configManager</span></span>|<span data-ttu-id="661da-129">255</span><span class="sxs-lookup"><span data-stu-id="661da-129">255</span></span>|<span data-ttu-id="661da-130">Управление с помощью диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="661da-130">Managed by Config Manager</span></span>|



