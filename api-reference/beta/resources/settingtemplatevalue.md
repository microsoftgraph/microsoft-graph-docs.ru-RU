---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
ms.openlocfilehash: 2277f4b7bb66839164a1b09011d20886baf2bd1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343187"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="65bdd-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="65bdd-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65bdd-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="65bdd-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="65bdd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="65bdd-105">Properties</span></span>
| <span data-ttu-id="65bdd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="65bdd-106">Property</span></span>     | <span data-ttu-id="65bdd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="65bdd-107">Type</span></span>   |<span data-ttu-id="65bdd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="65bdd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65bdd-109">Значение</span><span class="sxs-lookup"><span data-stu-id="65bdd-109">defaultValue</span></span>|<span data-ttu-id="65bdd-110">string</span><span class="sxs-lookup"><span data-stu-id="65bdd-110">string</span></span>|<span data-ttu-id="65bdd-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="65bdd-111">Default value for the setting.</span></span> <span data-ttu-id="65bdd-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65bdd-112">Read-only.</span></span>|
|<span data-ttu-id="65bdd-113">description</span><span class="sxs-lookup"><span data-stu-id="65bdd-113">description</span></span>|<span data-ttu-id="65bdd-114">string</span><span class="sxs-lookup"><span data-stu-id="65bdd-114">string</span></span>|<span data-ttu-id="65bdd-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="65bdd-115">Description of the setting.</span></span> <span data-ttu-id="65bdd-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65bdd-116">Read-only.</span></span>|
|<span data-ttu-id="65bdd-117">name</span><span class="sxs-lookup"><span data-stu-id="65bdd-117">name</span></span>|<span data-ttu-id="65bdd-118">строка</span><span class="sxs-lookup"><span data-stu-id="65bdd-118">string</span></span>|<span data-ttu-id="65bdd-119">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="65bdd-119">Name of the setting.</span></span> <span data-ttu-id="65bdd-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65bdd-120">Read-only.</span></span>|
|<span data-ttu-id="65bdd-121">type</span><span class="sxs-lookup"><span data-stu-id="65bdd-121">type</span></span>|<span data-ttu-id="65bdd-122">string</span><span class="sxs-lookup"><span data-stu-id="65bdd-122">string</span></span>|<span data-ttu-id="65bdd-123">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="65bdd-123">Type of the setting.</span></span> <span data-ttu-id="65bdd-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65bdd-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65bdd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65bdd-125">JSON representation</span></span>

<span data-ttu-id="65bdd-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65bdd-126">Here is a JSON representation of the resource.</span></span>

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
