---
title: Тип ресурса Девицеманажементенумконстраинт
description: Ограничение, которое задает значение параметра, из разрешенного набора строк
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64c07f663d034cf6fa758155294730015ca6e3b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964103"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="28354-103">Тип ресурса Девицеманажементенумконстраинт</span><span class="sxs-lookup"><span data-stu-id="28354-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="28354-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28354-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28354-106">Ограничение, которое задает значение параметра, из разрешенного набора строк</span><span class="sxs-lookup"><span data-stu-id="28354-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="28354-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="28354-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28354-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="28354-108">Properties</span></span>
|<span data-ttu-id="28354-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="28354-109">Property</span></span>|<span data-ttu-id="28354-110">Тип</span><span class="sxs-lookup"><span data-stu-id="28354-110">Type</span></span>|<span data-ttu-id="28354-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28354-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28354-112">values</span><span class="sxs-lookup"><span data-stu-id="28354-112">values</span></span>|<span data-ttu-id="28354-113">Коллекция [девицеманажементенумвалуе](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="28354-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="28354-114">Список допустимых значений для этой строки</span><span class="sxs-lookup"><span data-stu-id="28354-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="28354-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="28354-115">Relationships</span></span>
<span data-ttu-id="28354-116">Нет</span><span class="sxs-lookup"><span data-stu-id="28354-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28354-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28354-117">JSON Representation</span></span>
<span data-ttu-id="28354-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28354-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```





