---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c39762290577c6279a4ecb52bd832ac9c961dbdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009200"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="74631-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="74631-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="74631-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74631-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74631-105">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="74631-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="74631-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="74631-106">Properties</span></span>

| <span data-ttu-id="74631-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="74631-107">Property</span></span> | <span data-ttu-id="74631-108">Тип</span><span class="sxs-lookup"><span data-stu-id="74631-108">Type</span></span> | <span data-ttu-id="74631-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74631-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="74631-110">Значение</span><span class="sxs-lookup"><span data-stu-id="74631-110">defaultValue</span></span>|<span data-ttu-id="74631-111">String</span><span class="sxs-lookup"><span data-stu-id="74631-111">String</span></span>| <span data-ttu-id="74631-112">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="74631-112">Default value for the setting.</span></span> |
|<span data-ttu-id="74631-113">description</span><span class="sxs-lookup"><span data-stu-id="74631-113">description</span></span>|<span data-ttu-id="74631-114">String</span><span class="sxs-lookup"><span data-stu-id="74631-114">String</span></span>| <span data-ttu-id="74631-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="74631-115">Description of the setting.</span></span> |
|<span data-ttu-id="74631-116">name</span><span class="sxs-lookup"><span data-stu-id="74631-116">name</span></span>|<span data-ttu-id="74631-117">String</span><span class="sxs-lookup"><span data-stu-id="74631-117">String</span></span>| <span data-ttu-id="74631-118">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="74631-118">Name of the setting.</span></span> |
|<span data-ttu-id="74631-119">type</span><span class="sxs-lookup"><span data-stu-id="74631-119">type</span></span>|<span data-ttu-id="74631-120">String</span><span class="sxs-lookup"><span data-stu-id="74631-120">String</span></span>| <span data-ttu-id="74631-121">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="74631-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="74631-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74631-122">JSON representation</span></span>

<span data-ttu-id="74631-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74631-123">Here is a JSON representation of the resource.</span></span>

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

