---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e652501f8cd96e3e820e61b4ad9d353b61f3fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008476"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="6e0ee-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="6e0ee-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e0ee-104">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="6e0ee-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="6e0ee-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e0ee-105">Properties</span></span>
| <span data-ttu-id="6e0ee-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e0ee-106">Property</span></span>     | <span data-ttu-id="6e0ee-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6e0ee-107">Type</span></span>   |<span data-ttu-id="6e0ee-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6e0ee-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e0ee-109">name</span><span class="sxs-lookup"><span data-stu-id="6e0ee-109">name</span></span>|<span data-ttu-id="6e0ee-110">string</span><span class="sxs-lookup"><span data-stu-id="6e0ee-110">string</span></span>|<span data-ttu-id="6e0ee-111">Имя параметра (как определено в Директорисеттингтемплате).</span><span class="sxs-lookup"><span data-stu-id="6e0ee-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="6e0ee-112">value</span><span class="sxs-lookup"><span data-stu-id="6e0ee-112">value</span></span>|<span data-ttu-id="6e0ee-113">string</span><span class="sxs-lookup"><span data-stu-id="6e0ee-113">string</span></span>|<span data-ttu-id="6e0ee-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="6e0ee-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e0ee-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e0ee-115">JSON representation</span></span>

<span data-ttu-id="6e0ee-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e0ee-116">Here is a JSON representation of the resource.</span></span>

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
