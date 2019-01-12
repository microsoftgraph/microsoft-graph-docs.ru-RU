---
title: Тип ресурса emailAddress
description: Имя и электронный адрес контакта или получателя сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7af23418132c4d1c20097899f870c7d25be119bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951756"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="f1df5-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="f1df5-103">emailAddress resource type</span></span>

<span data-ttu-id="f1df5-104">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="f1df5-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="f1df5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1df5-105">Properties</span></span>
| <span data-ttu-id="f1df5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1df5-106">Property</span></span>     | <span data-ttu-id="f1df5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f1df5-107">Type</span></span>   |<span data-ttu-id="f1df5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f1df5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1df5-109">address</span><span class="sxs-lookup"><span data-stu-id="f1df5-109">address</span></span>|<span data-ttu-id="f1df5-110">String</span><span class="sxs-lookup"><span data-stu-id="f1df5-110">String</span></span>|<span data-ttu-id="f1df5-111">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="f1df5-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="f1df5-112">name</span><span class="sxs-lookup"><span data-stu-id="f1df5-112">name</span></span>|<span data-ttu-id="f1df5-113">String</span><span class="sxs-lookup"><span data-stu-id="f1df5-113">String</span></span>|<span data-ttu-id="f1df5-114">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="f1df5-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1df5-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1df5-115">JSON representation</span></span>

<span data-ttu-id="f1df5-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1df5-116">Here is a JSON representation of the resource</span></span>

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
