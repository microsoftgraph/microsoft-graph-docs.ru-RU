---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507100"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="01675-104">Тип ресурса Едукатионсинчронизатионлиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="01675-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01675-105">Представляет сведения о лицензии, назначаемые учетным записям пользователей.</span><span class="sxs-lookup"><span data-stu-id="01675-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="01675-106">Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="01675-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="01675-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="01675-107">Properties</span></span>

| <span data-ttu-id="01675-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="01675-108">Property</span></span> | <span data-ttu-id="01675-109">Тип</span><span class="sxs-lookup"><span data-stu-id="01675-109">Type</span></span> | <span data-ttu-id="01675-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01675-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="01675-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="01675-111">**appliesTo**</span></span> | <span data-ttu-id="01675-112">строка</span><span class="sxs-lookup"><span data-stu-id="01675-112">string</span></span> | <span data-ttu-id="01675-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="01675-113">The user role type to assign to license.</span></span> <span data-ttu-id="01675-114">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="01675-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="01675-115">**Скуидс**</span><span class="sxs-lookup"><span data-stu-id="01675-115">**skuIds**</span></span> | <span data-ttu-id="01675-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="01675-116">collection of strings</span></span> |  <span data-ttu-id="01675-117">Представляет идентификаторы SKU назначаемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="01675-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="01675-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01675-118">JSON representation</span></span>
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
