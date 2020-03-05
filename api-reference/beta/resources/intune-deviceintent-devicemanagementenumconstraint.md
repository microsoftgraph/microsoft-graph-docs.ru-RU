---
title: Тип ресурса Девицеманажементенумконстраинт
description: Ограничение, которое задает значение параметра, из разрешенного набора строк
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35dd4a8a4d69125e9bc675644980e5cfa3d90679
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525322"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="9aea2-103">Тип ресурса Девицеманажементенумконстраинт</span><span class="sxs-lookup"><span data-stu-id="9aea2-103">deviceManagementEnumConstraint resource type</span></span>

<span data-ttu-id="9aea2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9aea2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9aea2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9aea2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9aea2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9aea2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9aea2-107">Ограничение, которое задает значение параметра, из разрешенного набора строк</span><span class="sxs-lookup"><span data-stu-id="9aea2-107">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="9aea2-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="9aea2-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9aea2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9aea2-109">Properties</span></span>
|<span data-ttu-id="9aea2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9aea2-110">Property</span></span>|<span data-ttu-id="9aea2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9aea2-111">Type</span></span>|<span data-ttu-id="9aea2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9aea2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aea2-113">values</span><span class="sxs-lookup"><span data-stu-id="9aea2-113">values</span></span>|<span data-ttu-id="9aea2-114">Коллекция [девицеманажементенумвалуе](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9aea2-114">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="9aea2-115">Список допустимых значений для этой строки</span><span class="sxs-lookup"><span data-stu-id="9aea2-115">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aea2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="9aea2-116">Relationships</span></span>
<span data-ttu-id="9aea2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9aea2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aea2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9aea2-118">JSON Representation</span></span>
<span data-ttu-id="9aea2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9aea2-119">Here is a JSON representation of the resource.</span></span>
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



