---
title: Тип ресурса emailAddress
description: Имя и электронный адрес контакта или получателя сообщения.
ms.openlocfilehash: 962b2f36af9e292125edc3da8606cd532b8c2ec0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024733"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="e6c99-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="e6c99-103">emailAddress resource type</span></span>

<span data-ttu-id="e6c99-104">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="e6c99-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="e6c99-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6c99-105">Properties</span></span>
| <span data-ttu-id="e6c99-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6c99-106">Property</span></span>     | <span data-ttu-id="e6c99-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e6c99-107">Type</span></span>   |<span data-ttu-id="e6c99-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c99-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6c99-109">address</span><span class="sxs-lookup"><span data-stu-id="e6c99-109">address</span></span>|<span data-ttu-id="e6c99-110">String</span><span class="sxs-lookup"><span data-stu-id="e6c99-110">String</span></span>|<span data-ttu-id="e6c99-111">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="e6c99-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="e6c99-112">name</span><span class="sxs-lookup"><span data-stu-id="e6c99-112">name</span></span>|<span data-ttu-id="e6c99-113">String</span><span class="sxs-lookup"><span data-stu-id="e6c99-113">String</span></span>|<span data-ttu-id="e6c99-114">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="e6c99-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6c99-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6c99-115">JSON representation</span></span>

<span data-ttu-id="e6c99-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6c99-116">Here is a JSON representation of the resource</span></span>

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
