---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b00550c1a4d2d02efc983ab345fbc429b443a5bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972399"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="18d3f-104">Тип ресурса Едукатионсинчронизатионлиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="18d3f-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d3f-105">Представляет сведения о лицензии, назначаемые учетным записям пользователей.</span><span class="sxs-lookup"><span data-stu-id="18d3f-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="18d3f-106">Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="18d3f-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="18d3f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="18d3f-107">Properties</span></span>

| <span data-ttu-id="18d3f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="18d3f-108">Property</span></span> | <span data-ttu-id="18d3f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="18d3f-109">Type</span></span> | <span data-ttu-id="18d3f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18d3f-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="18d3f-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="18d3f-111">**appliesTo**</span></span> | <span data-ttu-id="18d3f-112">string</span><span class="sxs-lookup"><span data-stu-id="18d3f-112">string</span></span> | <span data-ttu-id="18d3f-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="18d3f-113">The user role type to assign to license.</span></span> <span data-ttu-id="18d3f-114">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="18d3f-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="18d3f-115">**Скуидс**</span><span class="sxs-lookup"><span data-stu-id="18d3f-115">**skuIds**</span></span> | <span data-ttu-id="18d3f-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="18d3f-116">collection of strings</span></span> |  <span data-ttu-id="18d3f-117">Представляет идентификаторы SKU назначаемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="18d3f-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="18d3f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18d3f-118">JSON representation</span></span>
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
