---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ba9b6321ad443d9538d9c539435c62f50149b330
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446893"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="c38f1-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="c38f1-103">settingValue resource type</span></span>

<span data-ttu-id="c38f1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c38f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c38f1-105">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="c38f1-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="c38f1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c38f1-106">Properties</span></span>

| <span data-ttu-id="c38f1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c38f1-107">Property</span></span> | <span data-ttu-id="c38f1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c38f1-108">Type</span></span> | <span data-ttu-id="c38f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c38f1-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c38f1-110">name</span><span class="sxs-lookup"><span data-stu-id="c38f1-110">name</span></span>|<span data-ttu-id="c38f1-111">String</span><span class="sxs-lookup"><span data-stu-id="c38f1-111">String</span></span>| <span data-ttu-id="c38f1-112">Имя параметра (как определено в [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="c38f1-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="c38f1-113">value</span><span class="sxs-lookup"><span data-stu-id="c38f1-113">value</span></span>|<span data-ttu-id="c38f1-114">String</span><span class="sxs-lookup"><span data-stu-id="c38f1-114">String</span></span>| <span data-ttu-id="c38f1-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="c38f1-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="c38f1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c38f1-116">JSON representation</span></span>

<span data-ttu-id="c38f1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c38f1-117">Here is a JSON representation of the resource.</span></span>

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
