---
title: Тип ресурса win32LobAppRegistryRule
description: Сложный тип для хранения данных правила реестра для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e4fcce49fde2f1eb8eb33bc320f1204369b09cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790812"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="1b93c-103">Тип ресурса win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="1b93c-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="1b93c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b93c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b93c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b93c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b93c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b93c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b93c-107">Сложный тип для хранения данных правила реестра для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="1b93c-107">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="1b93c-108">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="1b93c-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b93c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b93c-109">Properties</span></span>
|<span data-ttu-id="1b93c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b93c-110">Property</span></span>|<span data-ttu-id="1b93c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1b93c-111">Type</span></span>|<span data-ttu-id="1b93c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1b93c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b93c-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="1b93c-113">ruleType</span></span>|[<span data-ttu-id="1b93c-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="1b93c-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="1b93c-115">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="1b93c-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="1b93c-116">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="1b93c-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="1b93c-117">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="1b93c-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="1b93c-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="1b93c-118">check32BitOn64System</span></span>|<span data-ttu-id="1b93c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b93c-119">Boolean</span></span>|<span data-ttu-id="1b93c-120">Значение, указывающее, следует ли выполнять поиск в 32 — разрядном реестре в 64 — разрядных системах.</span><span class="sxs-lookup"><span data-stu-id="1b93c-120">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="1b93c-121">Ключевой</span><span class="sxs-lookup"><span data-stu-id="1b93c-121">keyPath</span></span>|<span data-ttu-id="1b93c-122">String</span><span class="sxs-lookup"><span data-stu-id="1b93c-122">String</span></span>|<span data-ttu-id="1b93c-123">Полный путь к параметру реестра, содержащему значение для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="1b93c-123">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="1b93c-124">valueName</span><span class="sxs-lookup"><span data-stu-id="1b93c-124">valueName</span></span>|<span data-ttu-id="1b93c-125">String</span><span class="sxs-lookup"><span data-stu-id="1b93c-125">String</span></span>|<span data-ttu-id="1b93c-126">Имя значения реестра для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="1b93c-126">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="1b93c-127">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="1b93c-127">operationType</span></span>|[<span data-ttu-id="1b93c-128">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="1b93c-128">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="1b93c-129">Тип операции в реестре.</span><span class="sxs-lookup"><span data-stu-id="1b93c-129">The registry operation type.</span></span> <span data-ttu-id="1b93c-130">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="1b93c-130">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="1b93c-131">operator</span><span class="sxs-lookup"><span data-stu-id="1b93c-131">operator</span></span>|[<span data-ttu-id="1b93c-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="1b93c-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="1b93c-133">Оператор для обнаружения в реестре.</span><span class="sxs-lookup"><span data-stu-id="1b93c-133">The operator for registry detection.</span></span> <span data-ttu-id="1b93c-134">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="1b93c-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="1b93c-135">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="1b93c-135">comparisonValue</span></span>|<span data-ttu-id="1b93c-136">String</span><span class="sxs-lookup"><span data-stu-id="1b93c-136">String</span></span>|<span data-ttu-id="1b93c-137">Значение сравнения в реестре.</span><span class="sxs-lookup"><span data-stu-id="1b93c-137">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b93c-138">Связи</span><span class="sxs-lookup"><span data-stu-id="1b93c-138">Relationships</span></span>
<span data-ttu-id="1b93c-139">Нет</span><span class="sxs-lookup"><span data-stu-id="1b93c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b93c-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b93c-140">JSON Representation</span></span>
<span data-ttu-id="1b93c-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b93c-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRule",
  "ruleType": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```



