---
title: Тип ресурса typedEmailAddress
description: Представляет имя, адреса электронной почты и соответствующий тип адреса электронной почты контакта.
localization_priority: Normal
ms.openlocfilehash: c77d3dddc3e2bfcac47e6ed245dad9223fe7f08c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871269"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="03170-103">Тип ресурса typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="03170-103">typedEmailAddress resource type</span></span>

> <span data-ttu-id="03170-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03170-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03170-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03170-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03170-106">Представляет имя, адреса электронной почты и их соответствующий тип адреса электронной почты [контакта](contact.md).</span><span class="sxs-lookup"><span data-stu-id="03170-106">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="03170-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="03170-107">Properties</span></span>
| <span data-ttu-id="03170-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="03170-108">Property</span></span>     | <span data-ttu-id="03170-109">Тип</span><span class="sxs-lookup"><span data-stu-id="03170-109">Type</span></span>   |<span data-ttu-id="03170-110">Описание</span><span class="sxs-lookup"><span data-stu-id="03170-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03170-111">address</span><span class="sxs-lookup"><span data-stu-id="03170-111">address</span></span>|<span data-ttu-id="03170-112">String</span><span class="sxs-lookup"><span data-stu-id="03170-112">String</span></span>|<span data-ttu-id="03170-113">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="03170-113">The email address of a contact.</span></span>|
|<span data-ttu-id="03170-114">name</span><span class="sxs-lookup"><span data-stu-id="03170-114">name</span></span>|<span data-ttu-id="03170-115">Строка</span><span class="sxs-lookup"><span data-stu-id="03170-115">String</span></span>|<span data-ttu-id="03170-116">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="03170-116">The display name of a contact.</span></span>|
|<span data-ttu-id="03170-117">type</span><span class="sxs-lookup"><span data-stu-id="03170-117">type</span></span> |<span data-ttu-id="03170-118">Строка</span><span class="sxs-lookup"><span data-stu-id="03170-118">String</span></span> |<span data-ttu-id="03170-119">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="03170-119">The type of email address.</span></span> <span data-ttu-id="03170-120">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="03170-120">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="03170-121">Значение по умолчанию — `unknown`, который означает, что **адрес** не был установлен как определенного типа.</span><span class="sxs-lookup"><span data-stu-id="03170-121">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="03170-122">otherLabel</span><span class="sxs-lookup"><span data-stu-id="03170-122">otherLabel</span></span> |<span data-ttu-id="03170-123">Строка</span><span class="sxs-lookup"><span data-stu-id="03170-123">String</span></span>  |<span data-ttu-id="03170-124">Чтобы сделать настраиваемого типа адреса электронной почты, задать **Тип** `other`и назначьте **otherLabel** настраиваемой строки.</span><span class="sxs-lookup"><span data-stu-id="03170-124">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="03170-125">Например может использовать действительный адрес электронной почты конкретного авторам действий.</span><span class="sxs-lookup"><span data-stu-id="03170-125">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="03170-126">Значение **типа** `other`и установите **otherLabel** в настраиваемой строке таких как `Volunteer work`.</span><span class="sxs-lookup"><span data-stu-id="03170-126">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03170-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03170-127">JSON representation</span></span>

<span data-ttu-id="03170-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03170-128">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
