---
title: Тип ресурса settingTemplateValue
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.
localization_priority: Normal
ms.openlocfilehash: e941630ab72363db1c4be40079cf2af9e40ff002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811867"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="6b8a5-103">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="6b8a5-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="6b8a5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b8a5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b8a5-106">Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="6b8a5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b8a5-107">Properties</span></span>
| <span data-ttu-id="6b8a5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b8a5-108">Property</span></span>     | <span data-ttu-id="6b8a5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6b8a5-109">Type</span></span>   |<span data-ttu-id="6b8a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b8a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b8a5-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="6b8a5-111">defaultValue</span></span>|<span data-ttu-id="6b8a5-112">string</span><span class="sxs-lookup"><span data-stu-id="6b8a5-112">string</span></span>|<span data-ttu-id="6b8a5-113">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-113">Default value for the setting.</span></span> <span data-ttu-id="6b8a5-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-114">Read-only.</span></span>|
|<span data-ttu-id="6b8a5-115">description</span><span class="sxs-lookup"><span data-stu-id="6b8a5-115">description</span></span>|<span data-ttu-id="6b8a5-116">строка</span><span class="sxs-lookup"><span data-stu-id="6b8a5-116">string</span></span>|<span data-ttu-id="6b8a5-117">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-117">Description of the setting.</span></span> <span data-ttu-id="6b8a5-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-118">Read-only.</span></span>|
|<span data-ttu-id="6b8a5-119">name</span><span class="sxs-lookup"><span data-stu-id="6b8a5-119">name</span></span>|<span data-ttu-id="6b8a5-120">строка</span><span class="sxs-lookup"><span data-stu-id="6b8a5-120">string</span></span>|<span data-ttu-id="6b8a5-121">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-121">Name of the setting.</span></span> <span data-ttu-id="6b8a5-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-122">Read-only.</span></span>|
|<span data-ttu-id="6b8a5-123">type</span><span class="sxs-lookup"><span data-stu-id="6b8a5-123">type</span></span>|<span data-ttu-id="6b8a5-124">строка</span><span class="sxs-lookup"><span data-stu-id="6b8a5-124">string</span></span>|<span data-ttu-id="6b8a5-125">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-125">Type of the setting.</span></span> <span data-ttu-id="6b8a5-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b8a5-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b8a5-127">JSON representation</span></span>

<span data-ttu-id="6b8a5-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b8a5-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
