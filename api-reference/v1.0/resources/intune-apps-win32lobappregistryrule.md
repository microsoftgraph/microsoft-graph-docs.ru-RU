---
title: Тип ресурса win32LobAppRegistryRule
description: Сложный тип для хранения данных правила реестра для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64343873093428849462cbdc12fc078a7a028e2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080123"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="2161c-103">Тип ресурса win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="2161c-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="2161c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2161c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2161c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2161c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2161c-106">Сложный тип для хранения данных правила реестра для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="2161c-106">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="2161c-107">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="2161c-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2161c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2161c-108">Properties</span></span>
|<span data-ttu-id="2161c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2161c-109">Property</span></span>|<span data-ttu-id="2161c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2161c-110">Type</span></span>|<span data-ttu-id="2161c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2161c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2161c-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="2161c-112">ruleType</span></span>|[<span data-ttu-id="2161c-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="2161c-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="2161c-114">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="2161c-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="2161c-115">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="2161c-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="2161c-116">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="2161c-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="2161c-117">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="2161c-117">check32BitOn64System</span></span>|<span data-ttu-id="2161c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2161c-118">Boolean</span></span>|<span data-ttu-id="2161c-119">Значение, указывающее, следует ли выполнять поиск в 32 — разрядном реестре в 64 — разрядных системах.</span><span class="sxs-lookup"><span data-stu-id="2161c-119">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="2161c-120">Ключевой</span><span class="sxs-lookup"><span data-stu-id="2161c-120">keyPath</span></span>|<span data-ttu-id="2161c-121">Строка</span><span class="sxs-lookup"><span data-stu-id="2161c-121">String</span></span>|<span data-ttu-id="2161c-122">Полный путь к параметру реестра, содержащему значение для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="2161c-122">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="2161c-123">valueName</span><span class="sxs-lookup"><span data-stu-id="2161c-123">valueName</span></span>|<span data-ttu-id="2161c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="2161c-124">String</span></span>|<span data-ttu-id="2161c-125">Имя значения реестра для обнаружения.</span><span class="sxs-lookup"><span data-stu-id="2161c-125">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="2161c-126">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="2161c-126">operationType</span></span>|[<span data-ttu-id="2161c-127">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="2161c-127">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="2161c-128">Тип операции в реестре.</span><span class="sxs-lookup"><span data-stu-id="2161c-128">The registry operation type.</span></span> <span data-ttu-id="2161c-129">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="2161c-129">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="2161c-130">operator</span><span class="sxs-lookup"><span data-stu-id="2161c-130">operator</span></span>|[<span data-ttu-id="2161c-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="2161c-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="2161c-132">Оператор для обнаружения в реестре.</span><span class="sxs-lookup"><span data-stu-id="2161c-132">The operator for registry detection.</span></span> <span data-ttu-id="2161c-133">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="2161c-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2161c-134">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="2161c-134">comparisonValue</span></span>|<span data-ttu-id="2161c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="2161c-135">String</span></span>|<span data-ttu-id="2161c-136">Значение сравнения в реестре.</span><span class="sxs-lookup"><span data-stu-id="2161c-136">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2161c-137">Связи</span><span class="sxs-lookup"><span data-stu-id="2161c-137">Relationships</span></span>
<span data-ttu-id="2161c-138">Нет</span><span class="sxs-lookup"><span data-stu-id="2161c-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2161c-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2161c-139">JSON Representation</span></span>
<span data-ttu-id="2161c-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2161c-140">Here is a JSON representation of the resource.</span></span>
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





