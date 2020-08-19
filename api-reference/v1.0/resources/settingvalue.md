---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 211609f81bf2ff8123783660b50e1bdd06cb3d56
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808125"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="70dcd-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="70dcd-103">settingValue resource type</span></span>

<span data-ttu-id="70dcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70dcd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70dcd-105">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="70dcd-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="70dcd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="70dcd-106">Properties</span></span>

| <span data-ttu-id="70dcd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="70dcd-107">Property</span></span> | <span data-ttu-id="70dcd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="70dcd-108">Type</span></span> | <span data-ttu-id="70dcd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70dcd-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="70dcd-110">name</span><span class="sxs-lookup"><span data-stu-id="70dcd-110">name</span></span>|<span data-ttu-id="70dcd-111">String</span><span class="sxs-lookup"><span data-stu-id="70dcd-111">String</span></span>| <span data-ttu-id="70dcd-112">Имя параметра (как определено в [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="70dcd-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="70dcd-113">value</span><span class="sxs-lookup"><span data-stu-id="70dcd-113">value</span></span>|<span data-ttu-id="70dcd-114">String</span><span class="sxs-lookup"><span data-stu-id="70dcd-114">String</span></span>| <span data-ttu-id="70dcd-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="70dcd-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="70dcd-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="70dcd-116">JSON representation</span></span>

<span data-ttu-id="70dcd-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70dcd-117">Here is a JSON representation of the resource.</span></span>

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
