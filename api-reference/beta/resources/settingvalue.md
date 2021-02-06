---
title: Тип ресурса settingValue
description: Параметр, представленный парой "имя-значение".
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: d1be40f6ad2046895c1a14f3395185662ae0ff62
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133380"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="c7060-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="c7060-103">settingValue resource type</span></span>

<span data-ttu-id="c7060-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7060-105">Параметр, представленный парой "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="c7060-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="c7060-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7060-106">Properties</span></span>
| <span data-ttu-id="c7060-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7060-107">Property</span></span>     | <span data-ttu-id="c7060-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c7060-108">Type</span></span>   |<span data-ttu-id="c7060-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c7060-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7060-110">name</span><span class="sxs-lookup"><span data-stu-id="c7060-110">name</span></span>|<span data-ttu-id="c7060-111">string</span><span class="sxs-lookup"><span data-stu-id="c7060-111">string</span></span>|<span data-ttu-id="c7060-112">Имя параметра (определяется directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="c7060-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="c7060-113">value</span><span class="sxs-lookup"><span data-stu-id="c7060-113">value</span></span>|<span data-ttu-id="c7060-114">string</span><span class="sxs-lookup"><span data-stu-id="c7060-114">string</span></span>|<span data-ttu-id="c7060-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="c7060-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7060-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7060-116">JSON representation</span></span>

<span data-ttu-id="c7060-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7060-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


