---
title: Тип ресурса win32LobAppRegistryRule
description: Сложный тип для хранения данных правила реестра для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74de895fccb70a96a5f6e80b15bd89453869096b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706214"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="32547-103">Тип ресурса win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="32547-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="32547-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32547-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32547-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32547-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32547-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32547-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32547-107">Сложный тип для хранения данных правила реестра для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="32547-107">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="32547-108">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="32547-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32547-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="32547-109">Properties</span></span>
|<span data-ttu-id="32547-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="32547-110">Property</span></span>|<span data-ttu-id="32547-111">Тип</span><span class="sxs-lookup"><span data-stu-id="32547-111">Type</span></span>|<span data-ttu-id="32547-112">Описание</span><span class="sxs-lookup"><span data-stu-id="32547-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32547-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="32547-113">ruleType</span></span>|[<span data-ttu-id="32547-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="32547-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="32547-115">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="32547-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="32547-116">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="32547-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="32547-117">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="32547-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="32547-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="32547-118">check32BitOn64System</span></span>|<span data-ttu-id="32547-119">Логический</span><span class="sxs-lookup"><span data-stu-id="32547-119">Boolean</span></span>|<span data-ttu-id="32547-120">Значение, указывающее, следует ли выполнять поиск в 32 — разрядном реестре в 64 — разрядных системах.</span><span class="sxs-lookup"><span data-stu-id="32547-120">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="32547-121">Ключевой</span><span class="sxs-lookup"><span data-stu-id="32547-121">keyPath</span></span>|<span data-ttu-id="32547-122">Строка</span><span class="sxs-lookup"><span data-stu-id="32547-122">String</span></span>|<span data-ttu-id="32547-123">Полный путь к параметру реестра, содержащему значение для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="32547-123">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="32547-124">valueName</span><span class="sxs-lookup"><span data-stu-id="32547-124">valueName</span></span>|<span data-ttu-id="32547-125">Строка</span><span class="sxs-lookup"><span data-stu-id="32547-125">String</span></span>|<span data-ttu-id="32547-126">Имя значения реестра для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="32547-126">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="32547-127">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="32547-127">operationType</span></span>|[<span data-ttu-id="32547-128">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="32547-128">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="32547-129">Тип операции в реестре.</span><span class="sxs-lookup"><span data-stu-id="32547-129">The registry operation type.</span></span> <span data-ttu-id="32547-130">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="32547-130">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="32547-131">operator</span><span class="sxs-lookup"><span data-stu-id="32547-131">operator</span></span>|[<span data-ttu-id="32547-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="32547-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="32547-133">Оператор для обнаружения в реестре.</span><span class="sxs-lookup"><span data-stu-id="32547-133">The operator for registry detection.</span></span> <span data-ttu-id="32547-134">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="32547-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="32547-135">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="32547-135">comparisonValue</span></span>|<span data-ttu-id="32547-136">Строка</span><span class="sxs-lookup"><span data-stu-id="32547-136">String</span></span>|<span data-ttu-id="32547-137">Значение сравнения в реестре.</span><span class="sxs-lookup"><span data-stu-id="32547-137">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32547-138">Связи</span><span class="sxs-lookup"><span data-stu-id="32547-138">Relationships</span></span>
<span data-ttu-id="32547-139">Нет</span><span class="sxs-lookup"><span data-stu-id="32547-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32547-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32547-140">JSON Representation</span></span>
<span data-ttu-id="32547-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32547-141">Here is a JSON representation of the resource.</span></span>
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





