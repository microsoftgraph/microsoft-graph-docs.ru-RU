---
title: Тип ресурса phone
description: Представляет номер телефона.
ms.openlocfilehash: d47f2c36f9913eb75868077bdd5bb2d599055c59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074712"
---
# <a name="phone-resource-type"></a><span data-ttu-id="0fb07-103">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="0fb07-103">phone resource type</span></span>

> <span data-ttu-id="0fb07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0fb07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fb07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb07-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fb07-106">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="0fb07-106">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="0fb07-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fb07-107">Properties</span></span>
| <span data-ttu-id="0fb07-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fb07-108">Property</span></span>     | <span data-ttu-id="0fb07-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0fb07-109">Type</span></span>   |<span data-ttu-id="0fb07-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0fb07-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fb07-111">number</span><span class="sxs-lookup"><span data-stu-id="0fb07-111">number</span></span>|<span data-ttu-id="0fb07-112">string</span><span class="sxs-lookup"><span data-stu-id="0fb07-112">string</span></span>|<span data-ttu-id="0fb07-113">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="0fb07-113">The phone number.</span></span>|
|<span data-ttu-id="0fb07-114">type</span><span class="sxs-lookup"><span data-stu-id="0fb07-114">type</span></span>|<span data-ttu-id="0fb07-115">String</span><span class="sxs-lookup"><span data-stu-id="0fb07-115">String</span></span>|<span data-ttu-id="0fb07-p102">Тип номера телефона. Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="0fb07-p102">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fb07-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0fb07-118">JSON representation</span></span>

<span data-ttu-id="0fb07-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fb07-119">Here is a JSON representation of the resource.</span></span>

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