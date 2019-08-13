---
title: Тип ресурса Девицехеалсскрипткомплианцеруле
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371561"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a><span data-ttu-id="27dcb-103">Тип ресурса Девицехеалсскрипткомплианцеруле</span><span class="sxs-lookup"><span data-stu-id="27dcb-103">deviceHealthScriptComplianceRule resource type</span></span>

> <span data-ttu-id="27dcb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27dcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27dcb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27dcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27dcb-106">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="27dcb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="27dcb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="27dcb-107">Properties</span></span>
|<span data-ttu-id="27dcb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="27dcb-108">Property</span></span>|<span data-ttu-id="27dcb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="27dcb-109">Type</span></span>|<span data-ttu-id="27dcb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27dcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27dcb-111">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="27dcb-111">detectionType</span></span>|[<span data-ttu-id="27dcb-112">девицехеалсскриптдетектионтипе</span><span class="sxs-lookup"><span data-stu-id="27dcb-112">deviceHealthScriptDetectionType</span></span>](../resources/intune-devices-devicehealthscriptdetectiontype.md)|<span data-ttu-id="27dcb-113">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27dcb-113">Not yet documented.</span></span> <span data-ttu-id="27dcb-114">Возможные значения: `notConfigured`, `string`.</span><span class="sxs-lookup"><span data-stu-id="27dcb-114">Possible values are: `notConfigured`, `string`.</span></span>|
|<span data-ttu-id="27dcb-115">operator</span><span class="sxs-lookup"><span data-stu-id="27dcb-115">operator</span></span>|[<span data-ttu-id="27dcb-116">девицехеалсскрипткомплианцерулеоператор</span><span class="sxs-lookup"><span data-stu-id="27dcb-116">deviceHealthScriptComplianceRuleOperator</span></span>](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|<span data-ttu-id="27dcb-117">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="27dcb-117">Not yet documented.</span></span> <span data-ttu-id="27dcb-118">Возможные значения: `notConfigured`, `equal`, `notEqual`.</span><span class="sxs-lookup"><span data-stu-id="27dcb-118">Possible values are: `notConfigured`, `equal`, `notEqual`.</span></span>|
|<span data-ttu-id="27dcb-119">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="27dcb-119">detectionValue</span></span>|<span data-ttu-id="27dcb-120">String</span><span class="sxs-lookup"><span data-stu-id="27dcb-120">String</span></span>|<span data-ttu-id="27dcb-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="27dcb-121">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="27dcb-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="27dcb-122">Relationships</span></span>
<span data-ttu-id="27dcb-123">Нет</span><span class="sxs-lookup"><span data-stu-id="27dcb-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27dcb-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27dcb-124">JSON Representation</span></span>
<span data-ttu-id="27dcb-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27dcb-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



