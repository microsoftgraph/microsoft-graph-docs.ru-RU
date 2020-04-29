---
title: Тип ресурса Phone
description: Представляет номер телефона.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2e20932285f7009ee470ba66a6a9cd78c50d65ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447187"
---
# <a name="phone-resource-type"></a><span data-ttu-id="ead69-103">Тип ресурса Phone</span><span class="sxs-lookup"><span data-stu-id="ead69-103">phone resource type</span></span>

<span data-ttu-id="ead69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ead69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ead69-105">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="ead69-105">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="ead69-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ead69-106">Properties</span></span>
| <span data-ttu-id="ead69-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ead69-107">Property</span></span>     | <span data-ttu-id="ead69-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ead69-108">Type</span></span>   |<span data-ttu-id="ead69-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ead69-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ead69-110">число</span><span class="sxs-lookup"><span data-stu-id="ead69-110">number</span></span>|<span data-ttu-id="ead69-111">string</span><span class="sxs-lookup"><span data-stu-id="ead69-111">string</span></span>|<span data-ttu-id="ead69-112">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="ead69-112">The phone number.</span></span>|
|<span data-ttu-id="ead69-113">type</span><span class="sxs-lookup"><span data-stu-id="ead69-113">type</span></span>|<span data-ttu-id="ead69-114">фонетипе</span><span class="sxs-lookup"><span data-stu-id="ead69-114">phoneType</span></span>|<span data-ttu-id="ead69-115">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="ead69-115">The type of phone number.</span></span> <span data-ttu-id="ead69-116">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="ead69-116">The possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ead69-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ead69-117">JSON representation</span></span>

<span data-ttu-id="ead69-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ead69-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
