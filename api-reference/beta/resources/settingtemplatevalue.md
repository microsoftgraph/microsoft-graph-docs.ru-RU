---
title: Тип ресурса settingTemplateValue
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.
ms.openlocfilehash: afc872f3e3d8d02acae639b967cdaf9375bb60cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078139"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="a533c-103">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="a533c-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="a533c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a533c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a533c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a533c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a533c-106">Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.</span><span class="sxs-lookup"><span data-stu-id="a533c-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="a533c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a533c-107">Properties</span></span>
| <span data-ttu-id="a533c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a533c-108">Property</span></span>     | <span data-ttu-id="a533c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a533c-109">Type</span></span>   |<span data-ttu-id="a533c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a533c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a533c-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a533c-111">defaultValue</span></span>|<span data-ttu-id="a533c-112">string</span><span class="sxs-lookup"><span data-stu-id="a533c-112">string</span></span>|<span data-ttu-id="a533c-113">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="a533c-113">Default value for the setting.</span></span> <span data-ttu-id="a533c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a533c-114">Read-only.</span></span>|
|<span data-ttu-id="a533c-115">description</span><span class="sxs-lookup"><span data-stu-id="a533c-115">description</span></span>|<span data-ttu-id="a533c-116">строка</span><span class="sxs-lookup"><span data-stu-id="a533c-116">string</span></span>|<span data-ttu-id="a533c-117">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="a533c-117">Description of the setting.</span></span> <span data-ttu-id="a533c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a533c-118">Read-only.</span></span>|
|<span data-ttu-id="a533c-119">name</span><span class="sxs-lookup"><span data-stu-id="a533c-119">name</span></span>|<span data-ttu-id="a533c-120">строка</span><span class="sxs-lookup"><span data-stu-id="a533c-120">string</span></span>|<span data-ttu-id="a533c-121">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="a533c-121">Name of the setting.</span></span> <span data-ttu-id="a533c-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a533c-122">Read-only.</span></span>|
|<span data-ttu-id="a533c-123">type</span><span class="sxs-lookup"><span data-stu-id="a533c-123">type</span></span>|<span data-ttu-id="a533c-124">строка</span><span class="sxs-lookup"><span data-stu-id="a533c-124">string</span></span>|<span data-ttu-id="a533c-125">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="a533c-125">Type of the setting.</span></span> <span data-ttu-id="a533c-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a533c-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a533c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a533c-127">JSON representation</span></span>

<span data-ttu-id="a533c-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a533c-128">Here is a JSON representation of the resource.</span></span>

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
