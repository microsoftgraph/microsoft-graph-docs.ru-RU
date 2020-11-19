---
title: тип перечисления win32LobAppPowerShellScriptDetectionType
description: Содержит все поддерживаемые типы обнаружения вывода сценариев PowerShell.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0cd50a6c1ab03cfe3a09859baadd8ec62c5ec667
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273916"
---
# <a name="win32lobapppowershellscriptdetectiontype-enum-type"></a><span data-ttu-id="9ae37-103">тип перечисления win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="9ae37-103">win32LobAppPowerShellScriptDetectionType enum type</span></span>

<span data-ttu-id="9ae37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ae37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ae37-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ae37-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ae37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ae37-107">Содержит все поддерживаемые типы обнаружения вывода сценариев PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ae37-107">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="9ae37-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9ae37-108">Members</span></span>
|<span data-ttu-id="9ae37-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9ae37-109">Member</span></span>|<span data-ttu-id="9ae37-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9ae37-110">Value</span></span>|<span data-ttu-id="9ae37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9ae37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ae37-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9ae37-112">notConfigured</span></span>|<span data-ttu-id="9ae37-113">нуль</span><span class="sxs-lookup"><span data-stu-id="9ae37-113">0</span></span>|<span data-ttu-id="9ae37-114">Не настроен.</span><span class="sxs-lookup"><span data-stu-id="9ae37-114">Not configured.</span></span>|
|<span data-ttu-id="9ae37-115">строка</span><span class="sxs-lookup"><span data-stu-id="9ae37-115">string</span></span>|<span data-ttu-id="9ae37-116">1,1</span><span class="sxs-lookup"><span data-stu-id="9ae37-116">1</span></span>|<span data-ttu-id="9ae37-117">Выходной тип данных String.</span><span class="sxs-lookup"><span data-stu-id="9ae37-117">Output data type is string.</span></span>|
|<span data-ttu-id="9ae37-118">dateTime</span><span class="sxs-lookup"><span data-stu-id="9ae37-118">dateTime</span></span>|<span data-ttu-id="9ae37-119">2</span><span class="sxs-lookup"><span data-stu-id="9ae37-119">2</span></span>|<span data-ttu-id="9ae37-120">Тип выходных данных — Дата и время.</span><span class="sxs-lookup"><span data-stu-id="9ae37-120">Output data type is date time.</span></span>|
|<span data-ttu-id="9ae37-121">integer</span><span class="sxs-lookup"><span data-stu-id="9ae37-121">integer</span></span>|<span data-ttu-id="9ae37-122">4</span><span class="sxs-lookup"><span data-stu-id="9ae37-122">3</span></span>|<span data-ttu-id="9ae37-123">Тип выходных данных — целое число.</span><span class="sxs-lookup"><span data-stu-id="9ae37-123">Output data type is integer.</span></span>|
|<span data-ttu-id="9ae37-124">float</span><span class="sxs-lookup"><span data-stu-id="9ae37-124">float</span></span>|<span data-ttu-id="9ae37-125">4 </span><span class="sxs-lookup"><span data-stu-id="9ae37-125">4</span></span>|<span data-ttu-id="9ae37-126">Тип выходных данных — float.</span><span class="sxs-lookup"><span data-stu-id="9ae37-126">Output data type is float.</span></span>|
|<span data-ttu-id="9ae37-127">version</span><span class="sxs-lookup"><span data-stu-id="9ae37-127">version</span></span>|<span data-ttu-id="9ae37-128">5 </span><span class="sxs-lookup"><span data-stu-id="9ae37-128">5</span></span>|<span data-ttu-id="9ae37-129">Тип выходных данных — Version.</span><span class="sxs-lookup"><span data-stu-id="9ae37-129">Output data type is version.</span></span>|
|<span data-ttu-id="9ae37-130">логический</span><span class="sxs-lookup"><span data-stu-id="9ae37-130">boolean</span></span>|<span data-ttu-id="9ae37-131">6 </span><span class="sxs-lookup"><span data-stu-id="9ae37-131">6</span></span>|<span data-ttu-id="9ae37-132">Тип выходных данных — Boolean.</span><span class="sxs-lookup"><span data-stu-id="9ae37-132">Output data type is boolean.</span></span>|




