---
title: Тип ресурса Девицеманажементенумконстраинт
description: Ограничение, которое задает значение параметра, из разрешенного набора строк
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71af621a27830695bf4638715573299a163fda58
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523681"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="dd81a-103">Тип ресурса Девицеманажементенумконстраинт</span><span class="sxs-lookup"><span data-stu-id="dd81a-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="dd81a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd81a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd81a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd81a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd81a-106">Ограничение, которое задает значение параметра, из разрешенного набора строк</span><span class="sxs-lookup"><span data-stu-id="dd81a-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="dd81a-107">НаСледуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="dd81a-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dd81a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd81a-108">Properties</span></span>
|<span data-ttu-id="dd81a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd81a-109">Property</span></span>|<span data-ttu-id="dd81a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dd81a-110">Type</span></span>|<span data-ttu-id="dd81a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dd81a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd81a-112">values</span><span class="sxs-lookup"><span data-stu-id="dd81a-112">values</span></span>|<span data-ttu-id="dd81a-113">Коллекция [девицеманажементенумвалуе](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="dd81a-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="dd81a-114">Список допустимых значений для этой строки</span><span class="sxs-lookup"><span data-stu-id="dd81a-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd81a-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="dd81a-115">Relationships</span></span>
<span data-ttu-id="dd81a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="dd81a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd81a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd81a-117">JSON Representation</span></span>
<span data-ttu-id="dd81a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd81a-118">Here is a JSON representation of the resource.</span></span>
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







