---
title: Тип ресурса emailAddress
description: Имя и электронный адрес контакта или получателя сообщения.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 055f4d426e475156469f3b3cd8ba9eca87102495
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132809"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="1c345-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="1c345-103">emailAddress resource type</span></span>

<span data-ttu-id="1c345-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c345-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1c345-105">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="1c345-105">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="1c345-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c345-106">Properties</span></span>
| <span data-ttu-id="1c345-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c345-107">Property</span></span>     | <span data-ttu-id="1c345-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1c345-108">Type</span></span>   |<span data-ttu-id="1c345-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1c345-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c345-110">address</span><span class="sxs-lookup"><span data-stu-id="1c345-110">address</span></span>|<span data-ttu-id="1c345-111">String</span><span class="sxs-lookup"><span data-stu-id="1c345-111">String</span></span>|<span data-ttu-id="1c345-112">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="1c345-112">The email address of the person or entity.</span></span>|
|<span data-ttu-id="1c345-113">name</span><span class="sxs-lookup"><span data-stu-id="1c345-113">name</span></span>|<span data-ttu-id="1c345-114">String</span><span class="sxs-lookup"><span data-stu-id="1c345-114">String</span></span>|<span data-ttu-id="1c345-115">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="1c345-115">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c345-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c345-116">JSON representation</span></span>

<span data-ttu-id="1c345-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c345-117">Here is a JSON representation of the resource</span></span>

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

