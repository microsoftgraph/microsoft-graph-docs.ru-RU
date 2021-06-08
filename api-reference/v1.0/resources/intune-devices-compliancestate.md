---
title: тип из переумыка complianceState
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4bae464724712333c81b73bdcd23e57148655624
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757740"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="aa1c7-103">тип из переумыка complianceState</span><span class="sxs-lookup"><span data-stu-id="aa1c7-103">complianceState enum type</span></span>

<span data-ttu-id="aa1c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa1c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa1c7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa1c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa1c7-106">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="aa1c7-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="aa1c7-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="aa1c7-107">Members</span></span>
|<span data-ttu-id="aa1c7-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="aa1c7-108">Member</span></span>|<span data-ttu-id="aa1c7-109">Значение</span><span class="sxs-lookup"><span data-stu-id="aa1c7-109">Value</span></span>|<span data-ttu-id="aa1c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aa1c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa1c7-111">unknown</span><span class="sxs-lookup"><span data-stu-id="aa1c7-111">unknown</span></span>|<span data-ttu-id="aa1c7-112">0</span><span class="sxs-lookup"><span data-stu-id="aa1c7-112">0</span></span>|<span data-ttu-id="aa1c7-113">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="aa1c7-113">Unknown.</span></span>|
|<span data-ttu-id="aa1c7-114">совместимый</span><span class="sxs-lookup"><span data-stu-id="aa1c7-114">compliant</span></span>|<span data-ttu-id="aa1c7-115">1</span><span class="sxs-lookup"><span data-stu-id="aa1c7-115">1</span></span>|<span data-ttu-id="aa1c7-116">Совместимый.</span><span class="sxs-lookup"><span data-stu-id="aa1c7-116">Compliant.</span></span>|
|<span data-ttu-id="aa1c7-117">нескомплиентные</span><span class="sxs-lookup"><span data-stu-id="aa1c7-117">noncompliant</span></span>|<span data-ttu-id="aa1c7-118">2</span><span class="sxs-lookup"><span data-stu-id="aa1c7-118">2</span></span>|<span data-ttu-id="aa1c7-119">Устройство не соответствует требованиям и блокируется из корпоративных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="aa1c7-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="aa1c7-120">конфликт</span><span class="sxs-lookup"><span data-stu-id="aa1c7-120">conflict</span></span>|<span data-ttu-id="aa1c7-121">3</span><span class="sxs-lookup"><span data-stu-id="aa1c7-121">3</span></span>|<span data-ttu-id="aa1c7-122">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="aa1c7-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="aa1c7-123">error</span><span class="sxs-lookup"><span data-stu-id="aa1c7-123">error</span></span>|<span data-ttu-id="aa1c7-124">4 </span><span class="sxs-lookup"><span data-stu-id="aa1c7-124">4</span></span>|<span data-ttu-id="aa1c7-125">Ошибка</span><span class="sxs-lookup"><span data-stu-id="aa1c7-125">Error.</span></span>|
|<span data-ttu-id="aa1c7-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="aa1c7-126">inGracePeriod</span></span>|<span data-ttu-id="aa1c7-127">254</span><span class="sxs-lookup"><span data-stu-id="aa1c7-127">254</span></span>|<span data-ttu-id="aa1c7-128">Устройство не соответствует требованиям, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="aa1c7-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="aa1c7-129">configManager</span><span class="sxs-lookup"><span data-stu-id="aa1c7-129">configManager</span></span>|<span data-ttu-id="aa1c7-130">255</span><span class="sxs-lookup"><span data-stu-id="aa1c7-130">255</span></span>|<span data-ttu-id="aa1c7-131">Управление менеджером Config</span><span class="sxs-lookup"><span data-stu-id="aa1c7-131">Managed by Config Manager</span></span>|




