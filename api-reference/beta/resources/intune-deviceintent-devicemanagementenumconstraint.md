---
title: Тип ресурса Девицеманажементенумконстраинт
description: Ограничение, которое задает значение параметра, из разрешенного набора строк
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab02e07fa9e7b83daa620b370403796bde949105
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366646"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="3e4af-103">Тип ресурса Девицеманажементенумконстраинт</span><span class="sxs-lookup"><span data-stu-id="3e4af-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="3e4af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e4af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e4af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e4af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e4af-106">Ограничение, которое задает значение параметра, из разрешенного набора строк</span><span class="sxs-lookup"><span data-stu-id="3e4af-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="3e4af-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3e4af-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e4af-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e4af-108">Properties</span></span>
|<span data-ttu-id="3e4af-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e4af-109">Property</span></span>|<span data-ttu-id="3e4af-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e4af-110">Type</span></span>|<span data-ttu-id="3e4af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e4af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e4af-112">values</span><span class="sxs-lookup"><span data-stu-id="3e4af-112">values</span></span>|<span data-ttu-id="3e4af-113">Коллекция [девицеманажементенумвалуе](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3e4af-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="3e4af-114">Список допустимых значений для этой строки</span><span class="sxs-lookup"><span data-stu-id="3e4af-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e4af-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="3e4af-115">Relationships</span></span>
<span data-ttu-id="3e4af-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3e4af-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e4af-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e4af-117">JSON Representation</span></span>
<span data-ttu-id="3e4af-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e4af-118">Here is a JSON representation of the resource.</span></span>
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



