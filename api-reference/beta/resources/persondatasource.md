---
title: Тип ресурса Персондатасаурце
description: Представляет источники, из которых берутся данные пользователя, например каталог и контакты Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 431cd9163873305508d5244005e6fe0a80501771
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573760"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="f2606-103">Тип ресурса Персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="f2606-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2606-104">Представляет источники, из которых берутся данные пользователя, например каталог и контакты Outlook.</span><span class="sxs-lookup"><span data-stu-id="f2606-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2606-105">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f2606-105">JSON representation</span></span>

<span data-ttu-id="f2606-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f2606-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f2606-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2606-107">Properties</span></span>
| <span data-ttu-id="f2606-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2606-108">Property</span></span>     | <span data-ttu-id="f2606-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f2606-109">Type</span></span>   |<span data-ttu-id="f2606-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f2606-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2606-111">type</span><span class="sxs-lookup"><span data-stu-id="f2606-111">type</span></span>|<span data-ttu-id="f2606-112">String</span><span class="sxs-lookup"><span data-stu-id="f2606-112">String</span></span>|<span data-ttu-id="f2606-113">Тип источника данных.</span><span class="sxs-lookup"><span data-stu-id="f2606-113">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/persondatasource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
