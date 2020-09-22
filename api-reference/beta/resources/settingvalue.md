---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 86f796b03afe55242a53be8803d9ff4a15d8a6e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033545"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="4580e-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="4580e-103">settingValue resource type</span></span>

<span data-ttu-id="4580e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4580e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4580e-105">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="4580e-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="4580e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4580e-106">Properties</span></span>
| <span data-ttu-id="4580e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4580e-107">Property</span></span>     | <span data-ttu-id="4580e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4580e-108">Type</span></span>   |<span data-ttu-id="4580e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4580e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4580e-110">name</span><span class="sxs-lookup"><span data-stu-id="4580e-110">name</span></span>|<span data-ttu-id="4580e-111">string</span><span class="sxs-lookup"><span data-stu-id="4580e-111">string</span></span>|<span data-ttu-id="4580e-112">Имя параметра (как определено в Директорисеттингтемплате).</span><span class="sxs-lookup"><span data-stu-id="4580e-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="4580e-113">value</span><span class="sxs-lookup"><span data-stu-id="4580e-113">value</span></span>|<span data-ttu-id="4580e-114">string</span><span class="sxs-lookup"><span data-stu-id="4580e-114">string</span></span>|<span data-ttu-id="4580e-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="4580e-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4580e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4580e-116">JSON representation</span></span>

<span data-ttu-id="4580e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4580e-117">Here is a JSON representation of the resource.</span></span>

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


