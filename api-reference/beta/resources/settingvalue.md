---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 1710bd136391a8c7d6d38217cb1635407570086f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806263"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="523fc-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="523fc-103">settingValue resource type</span></span>

<span data-ttu-id="523fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="523fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="523fc-105">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="523fc-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="523fc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="523fc-106">Properties</span></span>
| <span data-ttu-id="523fc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="523fc-107">Property</span></span>     | <span data-ttu-id="523fc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="523fc-108">Type</span></span>   |<span data-ttu-id="523fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="523fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="523fc-110">name</span><span class="sxs-lookup"><span data-stu-id="523fc-110">name</span></span>|<span data-ttu-id="523fc-111">string</span><span class="sxs-lookup"><span data-stu-id="523fc-111">string</span></span>|<span data-ttu-id="523fc-112">Имя параметра (как определено в Директорисеттингтемплате).</span><span class="sxs-lookup"><span data-stu-id="523fc-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="523fc-113">value</span><span class="sxs-lookup"><span data-stu-id="523fc-113">value</span></span>|<span data-ttu-id="523fc-114">string</span><span class="sxs-lookup"><span data-stu-id="523fc-114">string</span></span>|<span data-ttu-id="523fc-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="523fc-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="523fc-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="523fc-116">JSON representation</span></span>

<span data-ttu-id="523fc-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="523fc-117">Here is a JSON representation of the resource.</span></span>

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
