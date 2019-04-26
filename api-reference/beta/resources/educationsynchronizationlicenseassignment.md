---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ae9b89d9fe921967b50b8e290ce29026dbc35ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334053"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="8a765-104">Тип ресурса Едукатионсинчронизатионлиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="8a765-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a765-105">Представляет сведения о лицензии, назначаемые учетным записям пользователей.</span><span class="sxs-lookup"><span data-stu-id="8a765-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="8a765-106">Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="8a765-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="8a765-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a765-107">Properties</span></span>

| <span data-ttu-id="8a765-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a765-108">Property</span></span> | <span data-ttu-id="8a765-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8a765-109">Type</span></span> | <span data-ttu-id="8a765-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a765-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8a765-111">**Тег**</span><span class="sxs-lookup"><span data-stu-id="8a765-111">**appliesTo**</span></span> | <span data-ttu-id="8a765-112">string</span><span class="sxs-lookup"><span data-stu-id="8a765-112">string</span></span> | <span data-ttu-id="8a765-113">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="8a765-113">The user role type to assign to license.</span></span> <span data-ttu-id="8a765-114">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="8a765-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="8a765-115">**Скуидс**</span><span class="sxs-lookup"><span data-stu-id="8a765-115">**skuIds**</span></span> | <span data-ttu-id="8a765-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8a765-116">collection of strings</span></span> |  <span data-ttu-id="8a765-117">Представляет идентификаторы SKU назначаемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="8a765-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="8a765-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a765-118">JSON representation</span></span>
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
