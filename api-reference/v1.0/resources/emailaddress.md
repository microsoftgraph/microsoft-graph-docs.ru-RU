---
title: Тип ресурса emailAddress
description: Имя и электронный адрес контакта или получателя сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3b6bddb5436408fa38c931cd7e1e1f5503979e5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032594"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="ae957-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="ae957-103">emailAddress resource type</span></span>

<span data-ttu-id="ae957-104">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="ae957-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="ae957-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae957-105">Properties</span></span>
| <span data-ttu-id="ae957-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae957-106">Property</span></span>     | <span data-ttu-id="ae957-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ae957-107">Type</span></span>   |<span data-ttu-id="ae957-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ae957-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae957-109">address</span><span class="sxs-lookup"><span data-stu-id="ae957-109">address</span></span>|<span data-ttu-id="ae957-110">String</span><span class="sxs-lookup"><span data-stu-id="ae957-110">String</span></span>|<span data-ttu-id="ae957-111">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="ae957-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="ae957-112">name</span><span class="sxs-lookup"><span data-stu-id="ae957-112">name</span></span>|<span data-ttu-id="ae957-113">String</span><span class="sxs-lookup"><span data-stu-id="ae957-113">String</span></span>|<span data-ttu-id="ae957-114">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="ae957-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae957-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae957-115">JSON representation</span></span>

<span data-ttu-id="ae957-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae957-116">Here is a JSON representation of the resource</span></span>

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
