---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5aea834ff2943046aff8a390ae110d775fd2f20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989642"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="28e8e-104">Тип ресурса Едукатионсинчронизатионлиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="28e8e-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="28e8e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e8e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e8e-106">Представляет сведения о лицензии, назначаемые учетным записям пользователей.</span><span class="sxs-lookup"><span data-stu-id="28e8e-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="28e8e-107">Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="28e8e-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="28e8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="28e8e-108">Properties</span></span>

| <span data-ttu-id="28e8e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="28e8e-109">Property</span></span>  | <span data-ttu-id="28e8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="28e8e-110">Type</span></span>              | <span data-ttu-id="28e8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28e8e-111">Description</span></span>                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="28e8e-112">Тег</span><span class="sxs-lookup"><span data-stu-id="28e8e-112">appliesTo</span></span> | <span data-ttu-id="28e8e-113">String</span><span class="sxs-lookup"><span data-stu-id="28e8e-113">String</span></span>            | <span data-ttu-id="28e8e-114">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="28e8e-114">The user role type to assign to license.</span></span> <span data-ttu-id="28e8e-115">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="28e8e-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="28e8e-116">скуидс</span><span class="sxs-lookup"><span data-stu-id="28e8e-116">skuIds</span></span>    | <span data-ttu-id="28e8e-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28e8e-117">String collection</span></span> | <span data-ttu-id="28e8e-118">Представляет идентификаторы SKU назначаемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="28e8e-118">Represents the SKU identifiers of the licenses to assign.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="28e8e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28e8e-119">JSON representation</span></span>

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


