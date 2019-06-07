---
title: Тип ресурса Едукатиононпремисесинфо
description: Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c147755aea584674e17f2de913e039b7d3e0cf82
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764781"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="a16c3-103">Тип ресурса Едукатиононпремисесинфо</span><span class="sxs-lookup"><span data-stu-id="a16c3-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="a16c3-104">Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a16c3-104">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="a16c3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a16c3-105">Properties</span></span>

| <span data-ttu-id="a16c3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a16c3-106">Property</span></span>    | <span data-ttu-id="a16c3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a16c3-107">Type</span></span>   | <span data-ttu-id="a16c3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a16c3-108">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="a16c3-109">Значения свойств ImmutableId</span><span class="sxs-lookup"><span data-stu-id="a16c3-109">immutableId</span></span> | <span data-ttu-id="a16c3-110">String</span><span class="sxs-lookup"><span data-stu-id="a16c3-110">String</span></span> | <span data-ttu-id="a16c3-111">Уникальный идентификатор объекта пользователя в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a16c3-111">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a16c3-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a16c3-112">JSON representation</span></span>

<span data-ttu-id="a16c3-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a16c3-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOnPremisesInfo"
}-->

```json
{
  "immutableId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOnPremisesInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
