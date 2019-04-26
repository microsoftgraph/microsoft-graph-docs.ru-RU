---
title: Тип ресурса Типедемаиладдресс
description: Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты контакта.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576460"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="fc462-103">Тип ресурса Типедемаиладдресс</span><span class="sxs-lookup"><span data-stu-id="fc462-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc462-104">Представляет имя, адреса электронной почты и соответствующие им типы адресов электронной почты [контакта](contact.md).</span><span class="sxs-lookup"><span data-stu-id="fc462-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fc462-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc462-105">Properties</span></span>
| <span data-ttu-id="fc462-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc462-106">Property</span></span>     | <span data-ttu-id="fc462-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fc462-107">Type</span></span>   |<span data-ttu-id="fc462-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fc462-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc462-109">address</span><span class="sxs-lookup"><span data-stu-id="fc462-109">address</span></span>|<span data-ttu-id="fc462-110">String</span><span class="sxs-lookup"><span data-stu-id="fc462-110">String</span></span>|<span data-ttu-id="fc462-111">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="fc462-111">The email address of a contact.</span></span>|
|<span data-ttu-id="fc462-112">name</span><span class="sxs-lookup"><span data-stu-id="fc462-112">name</span></span>|<span data-ttu-id="fc462-113">Строка</span><span class="sxs-lookup"><span data-stu-id="fc462-113">String</span></span>|<span data-ttu-id="fc462-114">Отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="fc462-114">The display name of a contact.</span></span>|
|<span data-ttu-id="fc462-115">type</span><span class="sxs-lookup"><span data-stu-id="fc462-115">type</span></span> |<span data-ttu-id="fc462-116">String</span><span class="sxs-lookup"><span data-stu-id="fc462-116">String</span></span> |<span data-ttu-id="fc462-117">Тип адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fc462-117">The type of email address.</span></span> <span data-ttu-id="fc462-118">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="fc462-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="fc462-119">Значение по умолчанию `unknown`—, то есть **адрес** не был задан как определенный тип.</span><span class="sxs-lookup"><span data-stu-id="fc462-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="fc462-120">Осерлабел</span><span class="sxs-lookup"><span data-stu-id="fc462-120">otherLabel</span></span> |<span data-ttu-id="fc462-121">String</span><span class="sxs-lookup"><span data-stu-id="fc462-121">String</span></span>  |<span data-ttu-id="fc462-122">Чтобы указать настраиваемый тип адреса электронной почты, задайте \*\*\*\* для `other`параметра Тип значение и назначьте **осерлабел** настраиваемой строке.</span><span class="sxs-lookup"><span data-stu-id="fc462-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="fc462-123">Например, вы можете использовать конкретный адрес электронной почты для своих мероприятий.</span><span class="sxs-lookup"><span data-stu-id="fc462-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="fc462-124">Задайте \*\*\*\* для `other`параметра Type значение, а для параметра **осерлабел** — настраиваемую `Volunteer work`строку (например,).</span><span class="sxs-lookup"><span data-stu-id="fc462-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fc462-125">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc462-125">JSON representation</span></span>

<span data-ttu-id="fc462-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc462-126">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
