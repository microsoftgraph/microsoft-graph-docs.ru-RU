---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
ms.openlocfilehash: dd2cb58c63ff560850bde285a17a06da2399711f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343178"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="d3ebc-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="d3ebc-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3ebc-104">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="d3ebc-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="d3ebc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3ebc-105">Properties</span></span>
| <span data-ttu-id="d3ebc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3ebc-106">Property</span></span>     | <span data-ttu-id="d3ebc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d3ebc-107">Type</span></span>   |<span data-ttu-id="d3ebc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d3ebc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3ebc-109">name</span><span class="sxs-lookup"><span data-stu-id="d3ebc-109">name</span></span>|<span data-ttu-id="d3ebc-110">string</span><span class="sxs-lookup"><span data-stu-id="d3ebc-110">string</span></span>|<span data-ttu-id="d3ebc-111">Имя параметра (как определено в Директорисеттингтемплате).</span><span class="sxs-lookup"><span data-stu-id="d3ebc-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="d3ebc-112">value</span><span class="sxs-lookup"><span data-stu-id="d3ebc-112">value</span></span>|<span data-ttu-id="d3ebc-113">string</span><span class="sxs-lookup"><span data-stu-id="d3ebc-113">string</span></span>|<span data-ttu-id="d3ebc-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="d3ebc-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3ebc-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3ebc-115">JSON representation</span></span>

<span data-ttu-id="d3ebc-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3ebc-116">Here is a JSON representation of the resource.</span></span>

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
