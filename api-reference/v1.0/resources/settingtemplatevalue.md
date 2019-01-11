---
title: Тип ресурса settingTemplateValue
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828324"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="89d87-103">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="89d87-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="89d87-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.</span><span class="sxs-lookup"><span data-stu-id="89d87-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="89d87-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="89d87-105">Properties</span></span>

| <span data-ttu-id="89d87-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="89d87-106">Property</span></span> | <span data-ttu-id="89d87-107">Тип</span><span class="sxs-lookup"><span data-stu-id="89d87-107">Type</span></span> | <span data-ttu-id="89d87-108">Описание</span><span class="sxs-lookup"><span data-stu-id="89d87-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="89d87-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="89d87-109">defaultValue</span></span>|<span data-ttu-id="89d87-110">String</span><span class="sxs-lookup"><span data-stu-id="89d87-110">String</span></span>| <span data-ttu-id="89d87-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="89d87-111">Default value for the setting.</span></span> |
|<span data-ttu-id="89d87-112">описание</span><span class="sxs-lookup"><span data-stu-id="89d87-112">description</span></span>|<span data-ttu-id="89d87-113">String</span><span class="sxs-lookup"><span data-stu-id="89d87-113">String</span></span>| <span data-ttu-id="89d87-114">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="89d87-114">Description of the setting.</span></span> |
|<span data-ttu-id="89d87-115">name</span><span class="sxs-lookup"><span data-stu-id="89d87-115">name</span></span>|<span data-ttu-id="89d87-116">String</span><span class="sxs-lookup"><span data-stu-id="89d87-116">String</span></span>| <span data-ttu-id="89d87-117">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="89d87-117">Name of the setting.</span></span> |
|<span data-ttu-id="89d87-118">type</span><span class="sxs-lookup"><span data-stu-id="89d87-118">type</span></span>|<span data-ttu-id="89d87-119">String</span><span class="sxs-lookup"><span data-stu-id="89d87-119">String</span></span>| <span data-ttu-id="89d87-120">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="89d87-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="89d87-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89d87-121">JSON representation</span></span>

<span data-ttu-id="89d87-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89d87-122">Here is a JSON representation of the resource.</span></span>

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
