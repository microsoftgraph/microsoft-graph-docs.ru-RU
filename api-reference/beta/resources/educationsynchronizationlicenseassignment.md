---
title: Тип ресурса educationSynchronizationLicenseAssignment
description: Представляет информацию о лицензии для назначения учетных записей пользователей. Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525824"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="06e3d-104">Тип ресурса educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="06e3d-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06e3d-105">Представляет информацию о лицензии для назначения учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="06e3d-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="06e3d-106">Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="06e3d-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="06e3d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="06e3d-107">Properties</span></span>

| <span data-ttu-id="06e3d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="06e3d-108">Property</span></span> | <span data-ttu-id="06e3d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="06e3d-109">Type</span></span> | <span data-ttu-id="06e3d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="06e3d-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="06e3d-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="06e3d-111">**appliesTo**</span></span> | <span data-ttu-id="06e3d-112">string</span><span class="sxs-lookup"><span data-stu-id="06e3d-112">string</span></span> | <span data-ttu-id="06e3d-113">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="06e3d-113">The user role type to assign to license.</span></span> <span data-ttu-id="06e3d-114">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="06e3d-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="06e3d-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="06e3d-115">**skuIds**</span></span> | <span data-ttu-id="06e3d-116">набор строк</span><span class="sxs-lookup"><span data-stu-id="06e3d-116">collection of strings</span></span> |  <span data-ttu-id="06e3d-117">Представляет идентификаторы SKU лицензий для назначения.</span><span class="sxs-lookup"><span data-stu-id="06e3d-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="06e3d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06e3d-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
