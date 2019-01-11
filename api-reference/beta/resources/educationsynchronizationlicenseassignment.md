---
title: Тип ресурса educationSynchronizationLicenseAssignment
description: Представляет информацию о лицензии для назначения учетных записей пользователей. Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9100ba799c8981d5defdd74d6346a66859b2d53e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804909"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="13cca-104">Тип ресурса educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="13cca-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="13cca-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13cca-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13cca-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13cca-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13cca-107">Представляет информацию о лицензии для назначения учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="13cca-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="13cca-108">Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="13cca-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="13cca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="13cca-109">Properties</span></span>

| <span data-ttu-id="13cca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="13cca-110">Property</span></span> | <span data-ttu-id="13cca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="13cca-111">Type</span></span> | <span data-ttu-id="13cca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="13cca-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="13cca-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="13cca-113">**appliesTo**</span></span> | <span data-ttu-id="13cca-114">string</span><span class="sxs-lookup"><span data-stu-id="13cca-114">string</span></span> | <span data-ttu-id="13cca-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="13cca-115">The user role type to assign to license.</span></span> <span data-ttu-id="13cca-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="13cca-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="13cca-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="13cca-117">**skuIds**</span></span> | <span data-ttu-id="13cca-118">набор строк</span><span class="sxs-lookup"><span data-stu-id="13cca-118">collection of strings</span></span> |  <span data-ttu-id="13cca-119">Представляет идентификаторы SKU лицензий для назначения.</span><span class="sxs-lookup"><span data-stu-id="13cca-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="13cca-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13cca-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
