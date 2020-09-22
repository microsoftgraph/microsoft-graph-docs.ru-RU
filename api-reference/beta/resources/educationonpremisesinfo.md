---
title: Тип ресурса Едукатиононпремисесинфо
description: Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ff575398f3829c5d2adbe92799f5b9dca953aa4e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998826"
---
# <a name="educationonpremisesinfo-resource-type"></a><span data-ttu-id="0f65e-103">Тип ресурса Едукатиононпремисесинфо</span><span class="sxs-lookup"><span data-stu-id="0f65e-103">educationOnPremisesInfo resource type</span></span>

<span data-ttu-id="0f65e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f65e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f65e-105">Дополнительные сведения, используемые для сопоставления локальной учетной записи пользователя Active Directory с их объектом пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0f65e-105">Additional information used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span>

## <a name="properties"></a><span data-ttu-id="0f65e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f65e-106">Properties</span></span>

| <span data-ttu-id="0f65e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f65e-107">Property</span></span>    | <span data-ttu-id="0f65e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f65e-108">Type</span></span>   | <span data-ttu-id="0f65e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f65e-109">Description</span></span>                                               |
| :---------- | :----- | :-------------------------------------------------------- |
| <span data-ttu-id="0f65e-110">Значения свойств ImmutableId</span><span class="sxs-lookup"><span data-stu-id="0f65e-110">immutableId</span></span> | <span data-ttu-id="0f65e-111">String</span><span class="sxs-lookup"><span data-stu-id="0f65e-111">String</span></span> | <span data-ttu-id="0f65e-112">Уникальный идентификатор объекта пользователя в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0f65e-112">Unique identifier for the user object in Active Directory.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f65e-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f65e-113">JSON representation</span></span>

<span data-ttu-id="0f65e-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f65e-114">The following is a JSON representation of the resource.</span></span>

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


