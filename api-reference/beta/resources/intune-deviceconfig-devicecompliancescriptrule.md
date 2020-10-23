---
title: Тип ресурса Девицекомплианцескриптруле
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60169100f3332ea78c9bf5079e4edba202108069
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729863"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="0fb4a-103">Тип ресурса Девицекомплианцескриптруле</span><span class="sxs-lookup"><span data-stu-id="0fb4a-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="0fb4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fb4a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fb4a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fb4a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0fb4a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0fb4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fb4a-108">Properties</span></span>
|<span data-ttu-id="0fb4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fb4a-109">Property</span></span>|<span data-ttu-id="0fb4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0fb4a-110">Type</span></span>|<span data-ttu-id="0fb4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0fb4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb4a-112">settingName</span><span class="sxs-lookup"><span data-stu-id="0fb4a-112">settingName</span></span>|<span data-ttu-id="0fb4a-113">String</span><span class="sxs-lookup"><span data-stu-id="0fb4a-113">String</span></span>|<span data-ttu-id="0fb4a-114">Имя параметра, указанное в правиле.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="0fb4a-115">operator</span><span class="sxs-lookup"><span data-stu-id="0fb4a-115">operator</span></span>|[<span data-ttu-id="0fb4a-116">operator</span><span class="sxs-lookup"><span data-stu-id="0fb4a-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="0fb4a-117">Оператор, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-117">Operator specified in the rule.</span></span> <span data-ttu-id="0fb4a-118">Возможные значения:,,,,,,,,,,, `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` , `notBeginsWith` ,,, `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` ,, `excludesAll` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="0fb4a-119">dataType</span><span class="sxs-lookup"><span data-stu-id="0fb4a-119">dataType</span></span>|[<span data-ttu-id="0fb4a-120">DataType</span><span class="sxs-lookup"><span data-stu-id="0fb4a-120">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="0fb4a-121">Тип данных, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-121">Data type specified in the rule.</span></span> <span data-ttu-id="0fb4a-122">Возможные значения: `none` , `boolean` ,,,,, `int64` `double` `string` `dateTime` `version` ,,, `base64` `xml` `booleanArray` , `int64Array` , `doubleArray` , `stringArray` , `dateTimeArray` , `versionArray` .</span><span class="sxs-lookup"><span data-stu-id="0fb4a-122">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="0fb4a-123">начинается</span><span class="sxs-lookup"><span data-stu-id="0fb4a-123">operand</span></span>|<span data-ttu-id="0fb4a-124">Строка</span><span class="sxs-lookup"><span data-stu-id="0fb4a-124">String</span></span>|<span data-ttu-id="0fb4a-125">Операнд, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-125">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fb4a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="0fb4a-126">Relationships</span></span>
<span data-ttu-id="0fb4a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0fb4a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fb4a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fb4a-128">JSON Representation</span></span>
<span data-ttu-id="0fb4a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fb4a-129">Here is a JSON representation of the resource.</span></span>
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
  "dataType": "String",
  "operand": "String"
}
```





