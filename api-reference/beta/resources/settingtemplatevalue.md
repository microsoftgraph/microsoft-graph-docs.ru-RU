---
title: Тип ресурса settingTemplateValue
description: Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если этот параметр не создается.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 15110b88b62352476619501c50457a5bd1db5a89
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131630"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="25365-103">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="25365-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="25365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25365-105">Представляет отдельное определение параметра шаблона, включая значение по умолчанию для параметра, если этот параметр не создается.</span><span class="sxs-lookup"><span data-stu-id="25365-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="25365-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25365-106">Properties</span></span>
| <span data-ttu-id="25365-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25365-107">Property</span></span>     | <span data-ttu-id="25365-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25365-108">Type</span></span>   |<span data-ttu-id="25365-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25365-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25365-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="25365-110">defaultValue</span></span>|<span data-ttu-id="25365-111">string</span><span class="sxs-lookup"><span data-stu-id="25365-111">string</span></span>|<span data-ttu-id="25365-112">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="25365-112">Default value for the setting.</span></span> <span data-ttu-id="25365-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25365-113">Read-only.</span></span>|
|<span data-ttu-id="25365-114">description</span><span class="sxs-lookup"><span data-stu-id="25365-114">description</span></span>|<span data-ttu-id="25365-115">string</span><span class="sxs-lookup"><span data-stu-id="25365-115">string</span></span>|<span data-ttu-id="25365-116">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="25365-116">Description of the setting.</span></span> <span data-ttu-id="25365-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25365-117">Read-only.</span></span>|
|<span data-ttu-id="25365-118">name</span><span class="sxs-lookup"><span data-stu-id="25365-118">name</span></span>|<span data-ttu-id="25365-119">string</span><span class="sxs-lookup"><span data-stu-id="25365-119">string</span></span>|<span data-ttu-id="25365-120">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="25365-120">Name of the setting.</span></span> <span data-ttu-id="25365-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25365-121">Read-only.</span></span>|
|<span data-ttu-id="25365-122">type</span><span class="sxs-lookup"><span data-stu-id="25365-122">type</span></span>|<span data-ttu-id="25365-123">string</span><span class="sxs-lookup"><span data-stu-id="25365-123">string</span></span>|<span data-ttu-id="25365-124">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="25365-124">Type of the setting.</span></span> <span data-ttu-id="25365-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25365-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25365-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25365-126">JSON representation</span></span>

<span data-ttu-id="25365-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25365-127">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


