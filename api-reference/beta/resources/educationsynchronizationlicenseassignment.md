---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d46e19c1869f7dff96a563dd54b1b9f303ce85a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434965"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="e1e02-104">Тип ресурса Едукатионсинчронизатионлиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="e1e02-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="e1e02-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1e02-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1e02-106">Представляет сведения о лицензии, назначаемые учетным записям пользователей.</span><span class="sxs-lookup"><span data-stu-id="e1e02-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="e1e02-107">Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="e1e02-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="e1e02-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1e02-108">Properties</span></span>

| <span data-ttu-id="e1e02-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1e02-109">Property</span></span>  | <span data-ttu-id="e1e02-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1e02-110">Type</span></span>              | <span data-ttu-id="e1e02-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e02-111">Description</span></span>                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e1e02-112">Тег</span><span class="sxs-lookup"><span data-stu-id="e1e02-112">appliesTo</span></span> | <span data-ttu-id="e1e02-113">String</span><span class="sxs-lookup"><span data-stu-id="e1e02-113">String</span></span>            | <span data-ttu-id="e1e02-114">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="e1e02-114">The user role type to assign to license.</span></span> <span data-ttu-id="e1e02-115">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="e1e02-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="e1e02-116">скуидс</span><span class="sxs-lookup"><span data-stu-id="e1e02-116">skuIds</span></span>    | <span data-ttu-id="e1e02-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e1e02-117">String collection</span></span> | <span data-ttu-id="e1e02-118">Представляет идентификаторы SKU назначаемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="e1e02-118">Represents the SKU identifiers of the licenses to assign.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="e1e02-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1e02-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "skuIds": ["String"]
}
```
