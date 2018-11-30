---
title: Тип ресурса settingTemplateValue
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.
ms.openlocfilehash: 00e424e36338855d8ef603d06c7a9ee52a99c621
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027886"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="78fce-103">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="78fce-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="78fce-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.</span><span class="sxs-lookup"><span data-stu-id="78fce-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="78fce-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="78fce-105">Properties</span></span>

| <span data-ttu-id="78fce-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="78fce-106">Property</span></span> | <span data-ttu-id="78fce-107">Тип</span><span class="sxs-lookup"><span data-stu-id="78fce-107">Type</span></span> | <span data-ttu-id="78fce-108">Описание</span><span class="sxs-lookup"><span data-stu-id="78fce-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="78fce-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="78fce-109">defaultValue</span></span>|<span data-ttu-id="78fce-110">String</span><span class="sxs-lookup"><span data-stu-id="78fce-110">String</span></span>| <span data-ttu-id="78fce-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="78fce-111">Default value for the setting.</span></span> |
|<span data-ttu-id="78fce-112">описание</span><span class="sxs-lookup"><span data-stu-id="78fce-112">description</span></span>|<span data-ttu-id="78fce-113">String</span><span class="sxs-lookup"><span data-stu-id="78fce-113">String</span></span>| <span data-ttu-id="78fce-114">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="78fce-114">Description of the setting.</span></span> |
|<span data-ttu-id="78fce-115">name</span><span class="sxs-lookup"><span data-stu-id="78fce-115">name</span></span>|<span data-ttu-id="78fce-116">String</span><span class="sxs-lookup"><span data-stu-id="78fce-116">String</span></span>| <span data-ttu-id="78fce-117">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="78fce-117">Name of the setting.</span></span> |
|<span data-ttu-id="78fce-118">type</span><span class="sxs-lookup"><span data-stu-id="78fce-118">type</span></span>|<span data-ttu-id="78fce-119">String</span><span class="sxs-lookup"><span data-stu-id="78fce-119">String</span></span>| <span data-ttu-id="78fce-120">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="78fce-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="78fce-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="78fce-121">JSON representation</span></span>

<span data-ttu-id="78fce-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78fce-122">Here is a JSON representation of the resource.</span></span>

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