---
title: Тип ресурса settingValue
description: Параметр, представленный парой "имя-значение".
localization_priority: Normal
ms.openlocfilehash: 0ddd6388e14ea3deff99e927541694a97c594195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815528"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="79aa6-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="79aa6-103">settingValue resource type</span></span>

> <span data-ttu-id="79aa6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79aa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79aa6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79aa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79aa6-106">Параметр, представленный парой "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="79aa6-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="79aa6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="79aa6-107">Properties</span></span>
| <span data-ttu-id="79aa6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="79aa6-108">Property</span></span>     | <span data-ttu-id="79aa6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="79aa6-109">Type</span></span>   |<span data-ttu-id="79aa6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="79aa6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79aa6-111">name</span><span class="sxs-lookup"><span data-stu-id="79aa6-111">name</span></span>|<span data-ttu-id="79aa6-112">строка</span><span class="sxs-lookup"><span data-stu-id="79aa6-112">string</span></span>|<span data-ttu-id="79aa6-113">Имя удаляемого параметра (как определено directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="79aa6-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="79aa6-114">value</span><span class="sxs-lookup"><span data-stu-id="79aa6-114">value</span></span>|<span data-ttu-id="79aa6-115">строка</span><span class="sxs-lookup"><span data-stu-id="79aa6-115">string</span></span>|<span data-ttu-id="79aa6-116">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="79aa6-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79aa6-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="79aa6-117">JSON representation</span></span>

<span data-ttu-id="79aa6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79aa6-118">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
