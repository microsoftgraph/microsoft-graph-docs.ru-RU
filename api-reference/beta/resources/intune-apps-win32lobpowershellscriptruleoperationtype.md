---
title: тип перечисления win32LobPowerShellScriptRuleOperationType
description: Содержит все поддерживаемые типы обнаружения вывода сценариев PowerShell.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4416e7ea5c1602772aed0ff89ff616cf779bdc4a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789583"
---
# <a name="win32lobpowershellscriptruleoperationtype-enum-type"></a><span data-ttu-id="0e353-103">тип перечисления win32LobPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="0e353-103">win32LobPowerShellScriptRuleOperationType enum type</span></span>

<span data-ttu-id="0e353-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e353-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e353-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e353-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e353-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e353-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e353-107">Содержит все поддерживаемые типы обнаружения вывода сценариев PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0e353-107">Contains all supported Powershell Script output detection type.</span></span>

## <a name="members"></a><span data-ttu-id="0e353-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0e353-108">Members</span></span>
|<span data-ttu-id="0e353-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0e353-109">Member</span></span>|<span data-ttu-id="0e353-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0e353-110">Value</span></span>|<span data-ttu-id="0e353-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0e353-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e353-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0e353-112">notConfigured</span></span>|<span data-ttu-id="0e353-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0e353-113">0</span></span>|<span data-ttu-id="0e353-114">Не настроен.</span><span class="sxs-lookup"><span data-stu-id="0e353-114">Not configured.</span></span>|
|<span data-ttu-id="0e353-115">string</span><span class="sxs-lookup"><span data-stu-id="0e353-115">string</span></span>|<span data-ttu-id="0e353-116">1 </span><span class="sxs-lookup"><span data-stu-id="0e353-116">1</span></span>|<span data-ttu-id="0e353-117">Выходной тип данных String.</span><span class="sxs-lookup"><span data-stu-id="0e353-117">Output data type is string.</span></span>|
|<span data-ttu-id="0e353-118">dateTime</span><span class="sxs-lookup"><span data-stu-id="0e353-118">dateTime</span></span>|<span data-ttu-id="0e353-119">2</span><span class="sxs-lookup"><span data-stu-id="0e353-119">2</span></span>|<span data-ttu-id="0e353-120">Тип выходных данных — Дата и время.</span><span class="sxs-lookup"><span data-stu-id="0e353-120">Output data type is date time.</span></span>|
|<span data-ttu-id="0e353-121">целое</span><span class="sxs-lookup"><span data-stu-id="0e353-121">integer</span></span>|<span data-ttu-id="0e353-122">4</span><span class="sxs-lookup"><span data-stu-id="0e353-122">3</span></span>|<span data-ttu-id="0e353-123">Тип выходных данных — целое число.</span><span class="sxs-lookup"><span data-stu-id="0e353-123">Output data type is integer.</span></span>|
|<span data-ttu-id="0e353-124">с плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="0e353-124">float</span></span>|<span data-ttu-id="0e353-125">4 </span><span class="sxs-lookup"><span data-stu-id="0e353-125">4</span></span>|<span data-ttu-id="0e353-126">Тип выходных данных — float.</span><span class="sxs-lookup"><span data-stu-id="0e353-126">Output data type is float.</span></span>|
|<span data-ttu-id="0e353-127">version</span><span class="sxs-lookup"><span data-stu-id="0e353-127">version</span></span>|<span data-ttu-id="0e353-128">5 </span><span class="sxs-lookup"><span data-stu-id="0e353-128">5</span></span>|<span data-ttu-id="0e353-129">Тип выходных данных — Version.</span><span class="sxs-lookup"><span data-stu-id="0e353-129">Output data type is version.</span></span>|
|<span data-ttu-id="0e353-130">boolean</span><span class="sxs-lookup"><span data-stu-id="0e353-130">boolean</span></span>|<span data-ttu-id="0e353-131">6 </span><span class="sxs-lookup"><span data-stu-id="0e353-131">6</span></span>|<span data-ttu-id="0e353-132">Тип выходных данных — Boolean.</span><span class="sxs-lookup"><span data-stu-id="0e353-132">Output data type is boolean.</span></span>|



