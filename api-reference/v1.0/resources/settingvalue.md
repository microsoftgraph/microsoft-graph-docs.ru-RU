---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f37a429fd9bb8e8d3cf65aef55d6af5033f4a598
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034358"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="27057-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="27057-103">settingValue resource type</span></span>

<span data-ttu-id="27057-104">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="27057-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="27057-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="27057-105">Properties</span></span>

| <span data-ttu-id="27057-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="27057-106">Property</span></span> | <span data-ttu-id="27057-107">Тип</span><span class="sxs-lookup"><span data-stu-id="27057-107">Type</span></span> | <span data-ttu-id="27057-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27057-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="27057-109">name</span><span class="sxs-lookup"><span data-stu-id="27057-109">name</span></span>|<span data-ttu-id="27057-110">String</span><span class="sxs-lookup"><span data-stu-id="27057-110">String</span></span>| <span data-ttu-id="27057-111">Имя параметра (как определено в [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="27057-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="27057-112">value</span><span class="sxs-lookup"><span data-stu-id="27057-112">value</span></span>|<span data-ttu-id="27057-113">String</span><span class="sxs-lookup"><span data-stu-id="27057-113">String</span></span>| <span data-ttu-id="27057-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="27057-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="27057-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27057-115">JSON representation</span></span>

<span data-ttu-id="27057-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27057-116">Here is a JSON representation of the resource.</span></span>

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
