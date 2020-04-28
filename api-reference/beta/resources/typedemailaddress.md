---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7d6c064e7a87b0e9c776a5691f24b48dfff56422
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519633"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="4e037-103">Тип ресурса Типедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="4e037-103">typedEmailAddress resource type</span></span>

<span data-ttu-id="4e037-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e037-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e037-105">Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).</span><span class="sxs-lookup"><span data-stu-id="4e037-105">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4e037-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e037-106">Properties</span></span>
| <span data-ttu-id="4e037-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e037-107">Property</span></span>     | <span data-ttu-id="4e037-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4e037-108">Type</span></span>   |<span data-ttu-id="4e037-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e037-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e037-110">address</span><span class="sxs-lookup"><span data-stu-id="4e037-110">address</span></span>|<span data-ttu-id="4e037-111">String</span><span class="sxs-lookup"><span data-stu-id="4e037-111">String</span></span>|<span data-ttu-id="4e037-112">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="4e037-112">The email address of a contact.</span></span>|
|<span data-ttu-id="4e037-113">name</span><span class="sxs-lookup"><span data-stu-id="4e037-113">name</span></span>|<span data-ttu-id="4e037-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4e037-114">String</span></span>|<span data-ttu-id="4e037-115">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="4e037-115">The display name of a contact.</span></span>|
|<span data-ttu-id="4e037-116">type</span><span class="sxs-lookup"><span data-stu-id="4e037-116">type</span></span> |<span data-ttu-id="4e037-117">String</span><span class="sxs-lookup"><span data-stu-id="4e037-117">String</span></span> |<span data-ttu-id="4e037-118">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4e037-118">The type of email address.</span></span> <span data-ttu-id="4e037-119">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="4e037-119">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="4e037-120">Значение по умолчанию `unknown`—, то есть **адрес** не был задан как определенный тип.</span><span class="sxs-lookup"><span data-stu-id="4e037-120">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="4e037-121">осерлабел</span><span class="sxs-lookup"><span data-stu-id="4e037-121">otherLabel</span></span> |<span data-ttu-id="4e037-122">String</span><span class="sxs-lookup"><span data-stu-id="4e037-122">String</span></span>  |<span data-ttu-id="4e037-123">Чтобы указать настраиваемый тип адреса электронной почты, задайте **type** для `other`параметра Тип значение и назначьте **осерлабел** настраиваемой строке.</span><span class="sxs-lookup"><span data-stu-id="4e037-123">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="4e037-124">Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий.</span><span class="sxs-lookup"><span data-stu-id="4e037-124">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="4e037-125">Задайте **type** для `other`параметра Type значение, а для параметра **осерлабел** — настраиваемую `Volunteer work`строку (например,).</span><span class="sxs-lookup"><span data-stu-id="4e037-125">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e037-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e037-126">JSON representation</span></span>

<span data-ttu-id="4e037-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e037-127">Here is a JSON representation of the resource</span></span>

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
