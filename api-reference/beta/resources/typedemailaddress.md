---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 8ce8ebdd0cb5b8b2113a80dacf72617d0f361356
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993013"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="2bdb3-103">Тип ресурса Типедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="2bdb3-103">typedEmailAddress resource type</span></span>

<span data-ttu-id="2bdb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bdb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bdb3-105">Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).</span><span class="sxs-lookup"><span data-stu-id="2bdb3-105">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2bdb3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bdb3-106">Properties</span></span>
| <span data-ttu-id="2bdb3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bdb3-107">Property</span></span>     | <span data-ttu-id="2bdb3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2bdb3-108">Type</span></span>   |<span data-ttu-id="2bdb3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2bdb3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bdb3-110">address</span><span class="sxs-lookup"><span data-stu-id="2bdb3-110">address</span></span>|<span data-ttu-id="2bdb3-111">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-111">String</span></span>|<span data-ttu-id="2bdb3-112">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-112">The email address of a contact.</span></span>|
|<span data-ttu-id="2bdb3-113">name</span><span class="sxs-lookup"><span data-stu-id="2bdb3-113">name</span></span>|<span data-ttu-id="2bdb3-114">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-114">String</span></span>|<span data-ttu-id="2bdb3-115">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-115">The display name of a contact.</span></span>|
|<span data-ttu-id="2bdb3-116">type</span><span class="sxs-lookup"><span data-stu-id="2bdb3-116">type</span></span> |<span data-ttu-id="2bdb3-117">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-117">String</span></span> |<span data-ttu-id="2bdb3-118">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-118">The type of email address.</span></span> <span data-ttu-id="2bdb3-119">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-119">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="2bdb3-120">Значение по умолчанию —, то есть `unknown` **адрес** не был задан как определенный тип.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-120">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="2bdb3-121">осерлабел</span><span class="sxs-lookup"><span data-stu-id="2bdb3-121">otherLabel</span></span> |<span data-ttu-id="2bdb3-122">String</span><span class="sxs-lookup"><span data-stu-id="2bdb3-122">String</span></span>  |<span data-ttu-id="2bdb3-123">Чтобы указать настраиваемый тип адреса электронной почты, задайте для параметра **тип** значение `other` и назначьте **осерлабел** настраиваемой строке.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-123">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="2bdb3-124">Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-124">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="2bdb3-125">Задайте для параметра **Type** значение `other` , а для параметра **осерлабел** — настраиваемую строку (например,) `Volunteer work` .</span><span class="sxs-lookup"><span data-stu-id="2bdb3-125">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2bdb3-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bdb3-126">JSON representation</span></span>

<span data-ttu-id="2bdb3-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bdb3-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


