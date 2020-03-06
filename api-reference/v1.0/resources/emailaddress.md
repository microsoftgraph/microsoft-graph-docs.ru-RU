---
title: Тип ресурса emailAddress
description: Имя и электронный адрес контакта или получателя сообщения.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5e22b568ba05808fc9a87257686afd540145b3ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531484"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="e076f-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="e076f-103">emailAddress resource type</span></span>

<span data-ttu-id="e076f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e076f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e076f-105">Имя и электронный адрес контакта или получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="e076f-105">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="e076f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e076f-106">Properties</span></span>
| <span data-ttu-id="e076f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e076f-107">Property</span></span>     | <span data-ttu-id="e076f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e076f-108">Type</span></span>   |<span data-ttu-id="e076f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e076f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e076f-110">address</span><span class="sxs-lookup"><span data-stu-id="e076f-110">address</span></span>|<span data-ttu-id="e076f-111">String</span><span class="sxs-lookup"><span data-stu-id="e076f-111">String</span></span>|<span data-ttu-id="e076f-112">Электронный адрес человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="e076f-112">The email address of the person or entity.</span></span>|
|<span data-ttu-id="e076f-113">name</span><span class="sxs-lookup"><span data-stu-id="e076f-113">name</span></span>|<span data-ttu-id="e076f-114">String</span><span class="sxs-lookup"><span data-stu-id="e076f-114">String</span></span>|<span data-ttu-id="e076f-115">Отображаемое имя человека или объекта.</span><span class="sxs-lookup"><span data-stu-id="e076f-115">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e076f-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e076f-116">JSON representation</span></span>

<span data-ttu-id="e076f-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e076f-117">Here is a JSON representation of the resource</span></span>

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
