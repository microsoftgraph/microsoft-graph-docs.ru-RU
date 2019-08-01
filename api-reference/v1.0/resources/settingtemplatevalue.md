---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4ac39001e260d7f65b3a593d90976f94acd4693
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034393"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="48877-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="48877-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="48877-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="48877-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="48877-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="48877-105">Properties</span></span>

| <span data-ttu-id="48877-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="48877-106">Property</span></span> | <span data-ttu-id="48877-107">Тип</span><span class="sxs-lookup"><span data-stu-id="48877-107">Type</span></span> | <span data-ttu-id="48877-108">Описание</span><span class="sxs-lookup"><span data-stu-id="48877-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="48877-109">Значение</span><span class="sxs-lookup"><span data-stu-id="48877-109">defaultValue</span></span>|<span data-ttu-id="48877-110">String</span><span class="sxs-lookup"><span data-stu-id="48877-110">String</span></span>| <span data-ttu-id="48877-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="48877-111">Default value for the setting.</span></span> |
|<span data-ttu-id="48877-112">description</span><span class="sxs-lookup"><span data-stu-id="48877-112">description</span></span>|<span data-ttu-id="48877-113">String</span><span class="sxs-lookup"><span data-stu-id="48877-113">String</span></span>| <span data-ttu-id="48877-114">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="48877-114">Description of the setting.</span></span> |
|<span data-ttu-id="48877-115">name</span><span class="sxs-lookup"><span data-stu-id="48877-115">name</span></span>|<span data-ttu-id="48877-116">String</span><span class="sxs-lookup"><span data-stu-id="48877-116">String</span></span>| <span data-ttu-id="48877-117">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="48877-117">Name of the setting.</span></span> |
|<span data-ttu-id="48877-118">type</span><span class="sxs-lookup"><span data-stu-id="48877-118">type</span></span>|<span data-ttu-id="48877-119">String</span><span class="sxs-lookup"><span data-stu-id="48877-119">String</span></span>| <span data-ttu-id="48877-120">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="48877-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="48877-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48877-121">JSON representation</span></span>

<span data-ttu-id="48877-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48877-122">Here is a JSON representation of the resource.</span></span>

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
