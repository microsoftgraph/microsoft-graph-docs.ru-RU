---
title: Тип ресурса получателей
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 1ba4e8c88de3ba96e5e846cb5be8261562567ac3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507840"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="8e761-103">Тип ресурса получателей</span><span class="sxs-lookup"><span data-stu-id="8e761-103">recipients resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="8e761-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e761-104">JSON representation</span></span>

<span data-ttu-id="8e761-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8e761-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8e761-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e761-106">Properties</span></span>
| <span data-ttu-id="8e761-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e761-107">Property</span></span>     | <span data-ttu-id="8e761-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8e761-108">Type</span></span>   |<span data-ttu-id="8e761-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8e761-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e761-110">alias</span><span class="sxs-lookup"><span data-stu-id="8e761-110">alias</span></span>|<span data-ttu-id="8e761-111">String</span><span class="sxs-lookup"><span data-stu-id="8e761-111">String</span></span>||
|<span data-ttu-id="8e761-112">email</span><span class="sxs-lookup"><span data-stu-id="8e761-112">email</span></span>|<span data-ttu-id="8e761-113">String</span><span class="sxs-lookup"><span data-stu-id="8e761-113">String</span></span>||
|<span data-ttu-id="8e761-114">objectId</span><span class="sxs-lookup"><span data-stu-id="8e761-114">objectId</span></span>|<span data-ttu-id="8e761-115">String</span><span class="sxs-lookup"><span data-stu-id="8e761-115">String</span></span>||
|<span data-ttu-id="8e761-116">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="8e761-116">permissionIdentityType</span></span>|<span data-ttu-id="8e761-117">String</span><span class="sxs-lookup"><span data-stu-id="8e761-117">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recipients.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
