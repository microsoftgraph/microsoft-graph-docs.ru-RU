---
title: Тип ресурса emailAddress
description: Имя и электронный адрес контакта или получателя сообщения.
localization_priority: Normal
ms.openlocfilehash: 5ea1919e5c5f389c9b7fece508e8339f722b725a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826888"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="2df28-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="2df28-103">emailAddress resource type</span></span>

<span data-ttu-id="2df28-104">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="2df28-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="2df28-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2df28-105">Properties</span></span>
| <span data-ttu-id="2df28-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2df28-106">Property</span></span>     | <span data-ttu-id="2df28-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2df28-107">Type</span></span>   |<span data-ttu-id="2df28-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2df28-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2df28-109">address</span><span class="sxs-lookup"><span data-stu-id="2df28-109">address</span></span>|<span data-ttu-id="2df28-110">String</span><span class="sxs-lookup"><span data-stu-id="2df28-110">String</span></span>|<span data-ttu-id="2df28-111">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="2df28-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="2df28-112">name</span><span class="sxs-lookup"><span data-stu-id="2df28-112">name</span></span>|<span data-ttu-id="2df28-113">String</span><span class="sxs-lookup"><span data-stu-id="2df28-113">String</span></span>|<span data-ttu-id="2df28-114">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="2df28-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2df28-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2df28-115">JSON representation</span></span>

<span data-ttu-id="2df28-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2df28-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
