---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 024007ef05edbb4c3e2e9f8cc901d654734a39ab
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806270"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="c0e30-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="c0e30-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="c0e30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0e30-105">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="c0e30-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="c0e30-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0e30-106">Properties</span></span>
| <span data-ttu-id="c0e30-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0e30-107">Property</span></span>     | <span data-ttu-id="c0e30-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e30-108">Type</span></span>   |<span data-ttu-id="c0e30-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e30-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0e30-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c0e30-110">defaultValue</span></span>|<span data-ttu-id="c0e30-111">string</span><span class="sxs-lookup"><span data-stu-id="c0e30-111">string</span></span>|<span data-ttu-id="c0e30-112">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="c0e30-112">Default value for the setting.</span></span> <span data-ttu-id="c0e30-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0e30-113">Read-only.</span></span>|
|<span data-ttu-id="c0e30-114">description</span><span class="sxs-lookup"><span data-stu-id="c0e30-114">description</span></span>|<span data-ttu-id="c0e30-115">string</span><span class="sxs-lookup"><span data-stu-id="c0e30-115">string</span></span>|<span data-ttu-id="c0e30-116">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="c0e30-116">Description of the setting.</span></span> <span data-ttu-id="c0e30-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0e30-117">Read-only.</span></span>|
|<span data-ttu-id="c0e30-118">name</span><span class="sxs-lookup"><span data-stu-id="c0e30-118">name</span></span>|<span data-ttu-id="c0e30-119">string</span><span class="sxs-lookup"><span data-stu-id="c0e30-119">string</span></span>|<span data-ttu-id="c0e30-120">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="c0e30-120">Name of the setting.</span></span> <span data-ttu-id="c0e30-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0e30-121">Read-only.</span></span>|
|<span data-ttu-id="c0e30-122">type</span><span class="sxs-lookup"><span data-stu-id="c0e30-122">type</span></span>|<span data-ttu-id="c0e30-123">string</span><span class="sxs-lookup"><span data-stu-id="c0e30-123">string</span></span>|<span data-ttu-id="c0e30-124">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="c0e30-124">Type of the setting.</span></span> <span data-ttu-id="c0e30-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0e30-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0e30-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0e30-126">JSON representation</span></span>

<span data-ttu-id="c0e30-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0e30-127">Here is a JSON representation of the resource.</span></span>

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
