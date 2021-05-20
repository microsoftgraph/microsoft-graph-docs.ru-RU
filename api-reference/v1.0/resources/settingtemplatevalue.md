---
title: настройка Тип ресурсаTemplateValue
description: Представляет индивидуальное определение параметра шаблона, включая значение по умолчанию для настройки, если параметр не мгновенно.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e53a8f07f325b023deea32e01fe217feeb35f49d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547052"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="7e731-103">настройка Тип ресурсаTemplateValue</span><span class="sxs-lookup"><span data-stu-id="7e731-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="7e731-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e731-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e731-105">Представляет индивидуальное определение параметра шаблона, включая значение по умолчанию для настройки, если параметр не мгновенно.</span><span class="sxs-lookup"><span data-stu-id="7e731-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="7e731-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e731-106">Properties</span></span>

| <span data-ttu-id="7e731-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e731-107">Property</span></span> | <span data-ttu-id="7e731-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7e731-108">Type</span></span> | <span data-ttu-id="7e731-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7e731-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7e731-110">по умолчаниюВалю</span><span class="sxs-lookup"><span data-stu-id="7e731-110">defaultValue</span></span>|<span data-ttu-id="7e731-111">String</span><span class="sxs-lookup"><span data-stu-id="7e731-111">String</span></span>| <span data-ttu-id="7e731-112">Значение по умолчанию для настройки.</span><span class="sxs-lookup"><span data-stu-id="7e731-112">Default value for the setting.</span></span> |
|<span data-ttu-id="7e731-113">description</span><span class="sxs-lookup"><span data-stu-id="7e731-113">description</span></span>|<span data-ttu-id="7e731-114">String</span><span class="sxs-lookup"><span data-stu-id="7e731-114">String</span></span>| <span data-ttu-id="7e731-115">Описание настройки.</span><span class="sxs-lookup"><span data-stu-id="7e731-115">Description of the setting.</span></span> |
|<span data-ttu-id="7e731-116">name</span><span class="sxs-lookup"><span data-stu-id="7e731-116">name</span></span>|<span data-ttu-id="7e731-117">String</span><span class="sxs-lookup"><span data-stu-id="7e731-117">String</span></span>| <span data-ttu-id="7e731-118">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="7e731-118">Name of the setting.</span></span> |
|<span data-ttu-id="7e731-119">type</span><span class="sxs-lookup"><span data-stu-id="7e731-119">type</span></span>|<span data-ttu-id="7e731-120">String</span><span class="sxs-lookup"><span data-stu-id="7e731-120">String</span></span>| <span data-ttu-id="7e731-121">Тип настройки.</span><span class="sxs-lookup"><span data-stu-id="7e731-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="7e731-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e731-122">JSON representation</span></span>

<span data-ttu-id="7e731-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e731-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
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

