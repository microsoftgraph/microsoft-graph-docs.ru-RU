---
title: Тип ресурса settingValue
description: Параметр, представленный парой "имя-значение".
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834036"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="51428-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="51428-103">settingValue resource type</span></span>

<span data-ttu-id="51428-104">Параметр, представленный парой "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="51428-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="51428-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51428-105">Properties</span></span>

| <span data-ttu-id="51428-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51428-106">Property</span></span> | <span data-ttu-id="51428-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51428-107">Type</span></span> | <span data-ttu-id="51428-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51428-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51428-109">name</span><span class="sxs-lookup"><span data-stu-id="51428-109">name</span></span>|<span data-ttu-id="51428-110">String</span><span class="sxs-lookup"><span data-stu-id="51428-110">String</span></span>| <span data-ttu-id="51428-111">Имя параметра, определенное [groupSettingTemplate](groupsettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="51428-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="51428-112">value</span><span class="sxs-lookup"><span data-stu-id="51428-112">value</span></span>|<span data-ttu-id="51428-113">String</span><span class="sxs-lookup"><span data-stu-id="51428-113">String</span></span>| <span data-ttu-id="51428-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="51428-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="51428-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="51428-115">JSON representation</span></span>

<span data-ttu-id="51428-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51428-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
