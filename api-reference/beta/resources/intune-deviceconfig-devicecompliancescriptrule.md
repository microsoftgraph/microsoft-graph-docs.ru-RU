---
title: Тип ресурса deviceComplianceScriptRule
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 169c286043e4c1ec7b9b16e45fa6fb4520781211
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154903"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="e7cea-103">Тип ресурса deviceComplianceScriptRule</span><span class="sxs-lookup"><span data-stu-id="e7cea-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="e7cea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7cea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7cea-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7cea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7cea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7cea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7cea-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e7cea-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e7cea-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7cea-108">Properties</span></span>
|<span data-ttu-id="e7cea-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7cea-109">Property</span></span>|<span data-ttu-id="e7cea-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e7cea-110">Type</span></span>|<span data-ttu-id="e7cea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7cea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7cea-112">settingName</span><span class="sxs-lookup"><span data-stu-id="e7cea-112">settingName</span></span>|<span data-ttu-id="e7cea-113">String</span><span class="sxs-lookup"><span data-stu-id="e7cea-113">String</span></span>|<span data-ttu-id="e7cea-114">Имя параметра, указанное в правиле.</span><span class="sxs-lookup"><span data-stu-id="e7cea-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="e7cea-115">operator</span><span class="sxs-lookup"><span data-stu-id="e7cea-115">operator</span></span>|[<span data-ttu-id="e7cea-116">operator</span><span class="sxs-lookup"><span data-stu-id="e7cea-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="e7cea-117">Оператор, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="e7cea-117">Operator specified in the rule.</span></span> <span data-ttu-id="e7cea-118">Возможные значения: `none` , , , `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` , `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` .</span><span class="sxs-lookup"><span data-stu-id="e7cea-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="e7cea-119">deviceComplianceScriptRulOperator</span><span class="sxs-lookup"><span data-stu-id="e7cea-119">deviceComplianceScriptRulOperator</span></span>|[<span data-ttu-id="e7cea-120">deviceComplianceScriptRulOperator</span><span class="sxs-lookup"><span data-stu-id="e7cea-120">deviceComplianceScriptRulOperator</span></span>](../resources/intune-deviceconfig-devicecompliancescriptruloperator.md)|<span data-ttu-id="e7cea-121">Оператор, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="e7cea-121">Operator specified in the rule.</span></span> <span data-ttu-id="e7cea-122">Возможные значения: `none` , , , `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` , `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` .</span><span class="sxs-lookup"><span data-stu-id="e7cea-122">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="e7cea-123">dataType</span><span class="sxs-lookup"><span data-stu-id="e7cea-123">dataType</span></span>|[<span data-ttu-id="e7cea-124">DataType</span><span class="sxs-lookup"><span data-stu-id="e7cea-124">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="e7cea-125">Тип данных, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="e7cea-125">Data type specified in the rule.</span></span> <span data-ttu-id="e7cea-126">Возможные значения: `none` , , , , , , , `boolean` , , `int64` , `double` `string` , `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` . `versionArray`</span><span class="sxs-lookup"><span data-stu-id="e7cea-126">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="e7cea-127">deviceComplianceScriptRuleDataType</span><span class="sxs-lookup"><span data-stu-id="e7cea-127">deviceComplianceScriptRuleDataType</span></span>|[<span data-ttu-id="e7cea-128">deviceComplianceScriptRuleDataType</span><span class="sxs-lookup"><span data-stu-id="e7cea-128">deviceComplianceScriptRuleDataType</span></span>](../resources/intune-deviceconfig-devicecompliancescriptruledatatype.md)|<span data-ttu-id="e7cea-129">Тип данных, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="e7cea-129">Data type specified in the rule.</span></span> <span data-ttu-id="e7cea-130">Возможные значения: `none` , , , , , , , `boolean` , , `int64` , `double` `string` , `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` . `versionArray`</span><span class="sxs-lookup"><span data-stu-id="e7cea-130">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="e7cea-131">operand</span><span class="sxs-lookup"><span data-stu-id="e7cea-131">operand</span></span>|<span data-ttu-id="e7cea-132">String</span><span class="sxs-lookup"><span data-stu-id="e7cea-132">String</span></span>|<span data-ttu-id="e7cea-133">Операнд, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="e7cea-133">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7cea-134">Связи</span><span class="sxs-lookup"><span data-stu-id="e7cea-134">Relationships</span></span>
<span data-ttu-id="e7cea-135">Нет</span><span class="sxs-lookup"><span data-stu-id="e7cea-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7cea-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7cea-136">JSON Representation</span></span>
<span data-ttu-id="e7cea-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7cea-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "deviceComplianceScriptRulOperator": "String",
  "dataType": "String",
  "deviceComplianceScriptRuleDataType": "String",
  "operand": "String"
}
```




