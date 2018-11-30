---
title: Тип ресурса typedEmailAddress
description: Представляет имя, адреса электронной почты и соответствующий тип адреса электронной почты контакта.
ms.openlocfilehash: 3f40add32fbc219606b6d78041552fc108803d1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082741"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="c5dad-103">Тип ресурса typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c5dad-103">typedEmailAddress resource type</span></span>

> <span data-ttu-id="c5dad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5dad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5dad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5dad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5dad-106">Представляет имя, адреса электронной почты и их соответствующий тип адреса электронной почты [контакта](contact.md).</span><span class="sxs-lookup"><span data-stu-id="c5dad-106">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c5dad-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5dad-107">Properties</span></span>
| <span data-ttu-id="c5dad-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5dad-108">Property</span></span>     | <span data-ttu-id="c5dad-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5dad-109">Type</span></span>   |<span data-ttu-id="c5dad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5dad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5dad-111">address</span><span class="sxs-lookup"><span data-stu-id="c5dad-111">address</span></span>|<span data-ttu-id="c5dad-112">String</span><span class="sxs-lookup"><span data-stu-id="c5dad-112">String</span></span>|<span data-ttu-id="c5dad-113">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="c5dad-113">The email address of a contact.</span></span>|
|<span data-ttu-id="c5dad-114">name</span><span class="sxs-lookup"><span data-stu-id="c5dad-114">name</span></span>|<span data-ttu-id="c5dad-115">String</span><span class="sxs-lookup"><span data-stu-id="c5dad-115">String</span></span>|<span data-ttu-id="c5dad-116">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="c5dad-116">The display name of a contact.</span></span>|
|<span data-ttu-id="c5dad-117">type</span><span class="sxs-lookup"><span data-stu-id="c5dad-117">type</span></span> |<span data-ttu-id="c5dad-118">String</span><span class="sxs-lookup"><span data-stu-id="c5dad-118">String</span></span> |<span data-ttu-id="c5dad-119">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c5dad-119">The type of email address.</span></span> <span data-ttu-id="c5dad-120">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="c5dad-120">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="c5dad-121">Значение по умолчанию — `unknown`, который означает, что **адрес** не был установлен как определенного типа.</span><span class="sxs-lookup"><span data-stu-id="c5dad-121">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="c5dad-122">otherLabel</span><span class="sxs-lookup"><span data-stu-id="c5dad-122">otherLabel</span></span> |<span data-ttu-id="c5dad-123">String</span><span class="sxs-lookup"><span data-stu-id="c5dad-123">String</span></span>  |<span data-ttu-id="c5dad-124">Чтобы сделать настраиваемого типа адреса электронной почты, задать **Тип** `other`и назначьте **otherLabel** настраиваемой строки.</span><span class="sxs-lookup"><span data-stu-id="c5dad-124">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="c5dad-125">Например может использовать действительный адрес электронной почты конкретного авторам действий.</span><span class="sxs-lookup"><span data-stu-id="c5dad-125">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="c5dad-126">Значение **типа** `other`и установите **otherLabel** в настраиваемой строке таких как `Volunteer work`.</span><span class="sxs-lookup"><span data-stu-id="c5dad-126">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c5dad-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5dad-127">JSON representation</span></span>

<span data-ttu-id="c5dad-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5dad-128">Here is a JSON representation of the resource</span></span>

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
