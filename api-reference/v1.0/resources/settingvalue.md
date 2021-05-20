---
title: настройкаВью типа ресурса
description: Параметр, представленный парой имени/стоимости.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 171b08d4542af6900dcb6549527e956c4395c947
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547045"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="7a1a7-103">настройкаВью типа ресурса</span><span class="sxs-lookup"><span data-stu-id="7a1a7-103">settingValue resource type</span></span>

<span data-ttu-id="7a1a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a1a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a1a7-105">Параметр, представленный парой имени/стоимости.</span><span class="sxs-lookup"><span data-stu-id="7a1a7-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="7a1a7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a1a7-106">Properties</span></span>

| <span data-ttu-id="7a1a7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a1a7-107">Property</span></span> | <span data-ttu-id="7a1a7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7a1a7-108">Type</span></span> | <span data-ttu-id="7a1a7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7a1a7-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7a1a7-110">name</span><span class="sxs-lookup"><span data-stu-id="7a1a7-110">name</span></span>|<span data-ttu-id="7a1a7-111">String</span><span class="sxs-lookup"><span data-stu-id="7a1a7-111">String</span></span>| <span data-ttu-id="7a1a7-112">Название настройки (определяемо [группойSettingTemplate).](groupsettingtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="7a1a7-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="7a1a7-113">value</span><span class="sxs-lookup"><span data-stu-id="7a1a7-113">value</span></span>|<span data-ttu-id="7a1a7-114">String</span><span class="sxs-lookup"><span data-stu-id="7a1a7-114">String</span></span>| <span data-ttu-id="7a1a7-115">Значение настройки.</span><span class="sxs-lookup"><span data-stu-id="7a1a7-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="7a1a7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a1a7-116">JSON representation</span></span>

<span data-ttu-id="7a1a7-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a1a7-117">Here is a JSON representation of the resource.</span></span>

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

