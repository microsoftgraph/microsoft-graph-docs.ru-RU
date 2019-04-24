---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc1f00ab09ac71f4f3cd9eb1aff8163a537ce257
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506729"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="45c93-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="45c93-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45c93-104">Представляет имя и SMTP-адрес экземпляра сущности, например, получателя сообщения или владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="45c93-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="45c93-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="45c93-105">Properties</span></span>
| <span data-ttu-id="45c93-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="45c93-106">Property</span></span>     | <span data-ttu-id="45c93-107">Тип</span><span class="sxs-lookup"><span data-stu-id="45c93-107">Type</span></span>   |<span data-ttu-id="45c93-108">Описание</span><span class="sxs-lookup"><span data-stu-id="45c93-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45c93-109">address</span><span class="sxs-lookup"><span data-stu-id="45c93-109">address</span></span>|<span data-ttu-id="45c93-110">String</span><span class="sxs-lookup"><span data-stu-id="45c93-110">String</span></span>|<span data-ttu-id="45c93-111">Адрес электронной почты экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="45c93-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="45c93-112">name</span><span class="sxs-lookup"><span data-stu-id="45c93-112">name</span></span>|<span data-ttu-id="45c93-113">String</span><span class="sxs-lookup"><span data-stu-id="45c93-113">String</span></span>|<span data-ttu-id="45c93-114">Отображаемое имя экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="45c93-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45c93-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45c93-115">JSON representation</span></span>

<span data-ttu-id="45c93-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45c93-116">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/emailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
