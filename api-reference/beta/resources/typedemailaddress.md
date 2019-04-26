---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
ms.openlocfilehash: 92f3f1f89c73fe968c7fb06f7c5ed4b0eff883fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345476"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="c68ad-103">Тип ресурса Типедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="c68ad-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c68ad-104">Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).</span><span class="sxs-lookup"><span data-stu-id="c68ad-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c68ad-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c68ad-105">Properties</span></span>
| <span data-ttu-id="c68ad-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c68ad-106">Property</span></span>     | <span data-ttu-id="c68ad-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c68ad-107">Type</span></span>   |<span data-ttu-id="c68ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c68ad-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c68ad-109">address</span><span class="sxs-lookup"><span data-stu-id="c68ad-109">address</span></span>|<span data-ttu-id="c68ad-110">String</span><span class="sxs-lookup"><span data-stu-id="c68ad-110">String</span></span>|<span data-ttu-id="c68ad-111">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="c68ad-111">The email address of a contact.</span></span>|
|<span data-ttu-id="c68ad-112">name</span><span class="sxs-lookup"><span data-stu-id="c68ad-112">name</span></span>|<span data-ttu-id="c68ad-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c68ad-113">String</span></span>|<span data-ttu-id="c68ad-114">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c68ad-114">The display name of a contact.</span></span>|
|<span data-ttu-id="c68ad-115">type</span><span class="sxs-lookup"><span data-stu-id="c68ad-115">type</span></span> |<span data-ttu-id="c68ad-116">String</span><span class="sxs-lookup"><span data-stu-id="c68ad-116">String</span></span> |<span data-ttu-id="c68ad-117">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c68ad-117">The type of email address.</span></span> <span data-ttu-id="c68ad-118">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="c68ad-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="c68ad-119">Значение по умолчанию `unknown`—, то есть **адрес** не был задан как определенный тип.</span><span class="sxs-lookup"><span data-stu-id="c68ad-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="c68ad-120">Осерлабел</span><span class="sxs-lookup"><span data-stu-id="c68ad-120">otherLabel</span></span> |<span data-ttu-id="c68ad-121">String</span><span class="sxs-lookup"><span data-stu-id="c68ad-121">String</span></span>  |<span data-ttu-id="c68ad-122">Чтобы указать настраиваемый тип адреса электронной почты, задайте \*\*\*\* для `other`параметра Тип значение и назначьте **осерлабел** настраиваемой строке.</span><span class="sxs-lookup"><span data-stu-id="c68ad-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="c68ad-123">Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий.</span><span class="sxs-lookup"><span data-stu-id="c68ad-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="c68ad-124">Задайте \*\*\*\* для `other`параметра Type значение, а для параметра **осерлабел** — настраиваемую `Volunteer work`строку (например,).</span><span class="sxs-lookup"><span data-stu-id="c68ad-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c68ad-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c68ad-125">JSON representation</span></span>

<span data-ttu-id="c68ad-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c68ad-126">Here is a JSON representation of the resource</span></span>

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
