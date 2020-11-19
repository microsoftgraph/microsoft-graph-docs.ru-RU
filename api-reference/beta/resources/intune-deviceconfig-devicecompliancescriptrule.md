---
title: Тип ресурса Девицекомплианцескриптруле
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29264e89f3c935d473161edb2c4fbad3bb88849b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260265"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="10cf1-103">Тип ресурса Девицекомплианцескриптруле</span><span class="sxs-lookup"><span data-stu-id="10cf1-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="10cf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10cf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10cf1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10cf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10cf1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10cf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10cf1-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="10cf1-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="10cf1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="10cf1-108">Properties</span></span>
|<span data-ttu-id="10cf1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="10cf1-109">Property</span></span>|<span data-ttu-id="10cf1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="10cf1-110">Type</span></span>|<span data-ttu-id="10cf1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="10cf1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10cf1-112">settingName</span><span class="sxs-lookup"><span data-stu-id="10cf1-112">settingName</span></span>|<span data-ttu-id="10cf1-113">String</span><span class="sxs-lookup"><span data-stu-id="10cf1-113">String</span></span>|<span data-ttu-id="10cf1-114">Имя параметра, указанное в правиле.</span><span class="sxs-lookup"><span data-stu-id="10cf1-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="10cf1-115">operator</span><span class="sxs-lookup"><span data-stu-id="10cf1-115">operator</span></span>|[<span data-ttu-id="10cf1-116">operator</span><span class="sxs-lookup"><span data-stu-id="10cf1-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="10cf1-117">Оператор, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="10cf1-117">Operator specified in the rule.</span></span> <span data-ttu-id="10cf1-118">Возможные значения:,,,,,,,,,,, `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` , `notBeginsWith` ,,, `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` ,, `excludesAll` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="10cf1-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="10cf1-119">dataType</span><span class="sxs-lookup"><span data-stu-id="10cf1-119">dataType</span></span>|[<span data-ttu-id="10cf1-120">DataType</span><span class="sxs-lookup"><span data-stu-id="10cf1-120">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="10cf1-121">Тип данных, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="10cf1-121">Data type specified in the rule.</span></span> <span data-ttu-id="10cf1-122">Возможные значения: `none` , `boolean` ,,,,, `int64` `double` `string` `dateTime` `version` ,,, `base64` `xml` `booleanArray` , `int64Array` , `doubleArray` , `stringArray` , `dateTimeArray` , `versionArray` .</span><span class="sxs-lookup"><span data-stu-id="10cf1-122">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="10cf1-123">начинается</span><span class="sxs-lookup"><span data-stu-id="10cf1-123">operand</span></span>|<span data-ttu-id="10cf1-124">String</span><span class="sxs-lookup"><span data-stu-id="10cf1-124">String</span></span>|<span data-ttu-id="10cf1-125">Операнд, указанный в правиле.</span><span class="sxs-lookup"><span data-stu-id="10cf1-125">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10cf1-126">Связи</span><span class="sxs-lookup"><span data-stu-id="10cf1-126">Relationships</span></span>
<span data-ttu-id="10cf1-127">Нет</span><span class="sxs-lookup"><span data-stu-id="10cf1-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10cf1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10cf1-128">JSON Representation</span></span>
<span data-ttu-id="10cf1-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10cf1-129">Here is a JSON representation of the resource.</span></span>
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




