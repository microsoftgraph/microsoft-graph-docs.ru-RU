---
title: Тип ресурса Девицеманажементенумконстраинт
description: Ограничение, которое задает значение параметра, из разрешенного набора строк
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 202365368c17d22cf33ea78320ac2a2604a59194
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061478"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="683ca-103">Тип ресурса Девицеманажементенумконстраинт</span><span class="sxs-lookup"><span data-stu-id="683ca-103">deviceManagementEnumConstraint resource type</span></span>

<span data-ttu-id="683ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="683ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="683ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="683ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="683ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="683ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="683ca-107">Ограничение, которое задает значение параметра, из разрешенного набора строк</span><span class="sxs-lookup"><span data-stu-id="683ca-107">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="683ca-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="683ca-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="683ca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="683ca-109">Properties</span></span>
|<span data-ttu-id="683ca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="683ca-110">Property</span></span>|<span data-ttu-id="683ca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="683ca-111">Type</span></span>|<span data-ttu-id="683ca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="683ca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="683ca-113">values</span><span class="sxs-lookup"><span data-stu-id="683ca-113">values</span></span>|<span data-ttu-id="683ca-114">Коллекция [девицеманажементенумвалуе](../resources/intune-deviceintent-devicemanagementenumvalue.md)</span><span class="sxs-lookup"><span data-stu-id="683ca-114">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="683ca-115">Список допустимых значений для этой строки</span><span class="sxs-lookup"><span data-stu-id="683ca-115">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="683ca-116">Связи</span><span class="sxs-lookup"><span data-stu-id="683ca-116">Relationships</span></span>
<span data-ttu-id="683ca-117">Нет</span><span class="sxs-lookup"><span data-stu-id="683ca-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="683ca-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="683ca-118">JSON Representation</span></span>
<span data-ttu-id="683ca-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="683ca-119">Here is a JSON representation of the resource.</span></span>
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






