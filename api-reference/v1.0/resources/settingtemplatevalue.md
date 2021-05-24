---
title: параметрTemplateValue типа ресурса
description: Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.
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
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="847bb-103">параметрTemplateValue типа ресурса</span><span class="sxs-lookup"><span data-stu-id="847bb-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="847bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="847bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="847bb-105">Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если параметр не является мгновенным.</span><span class="sxs-lookup"><span data-stu-id="847bb-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="847bb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="847bb-106">Properties</span></span>

| <span data-ttu-id="847bb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="847bb-107">Property</span></span> | <span data-ttu-id="847bb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="847bb-108">Type</span></span> | <span data-ttu-id="847bb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="847bb-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="847bb-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="847bb-110">defaultValue</span></span>|<span data-ttu-id="847bb-111">Строка</span><span class="sxs-lookup"><span data-stu-id="847bb-111">String</span></span>| <span data-ttu-id="847bb-112">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="847bb-112">Default value for the setting.</span></span> |
|<span data-ttu-id="847bb-113">description</span><span class="sxs-lookup"><span data-stu-id="847bb-113">description</span></span>|<span data-ttu-id="847bb-114">Строка</span><span class="sxs-lookup"><span data-stu-id="847bb-114">String</span></span>| <span data-ttu-id="847bb-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="847bb-115">Description of the setting.</span></span> |
|<span data-ttu-id="847bb-116">name</span><span class="sxs-lookup"><span data-stu-id="847bb-116">name</span></span>|<span data-ttu-id="847bb-117">String</span><span class="sxs-lookup"><span data-stu-id="847bb-117">String</span></span>| <span data-ttu-id="847bb-118">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="847bb-118">Name of the setting.</span></span> |
|<span data-ttu-id="847bb-119">type</span><span class="sxs-lookup"><span data-stu-id="847bb-119">type</span></span>|<span data-ttu-id="847bb-120">Строка</span><span class="sxs-lookup"><span data-stu-id="847bb-120">String</span></span>| <span data-ttu-id="847bb-121">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="847bb-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="847bb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="847bb-122">JSON representation</span></span>

<span data-ttu-id="847bb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="847bb-123">Here is a JSON representation of the resource.</span></span>

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

