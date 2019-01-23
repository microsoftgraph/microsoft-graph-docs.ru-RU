---
title: Тип ресурса educationSynchronizationLicenseAssignment
description: Представляет информацию о лицензии для назначения учетных записей пользователей. Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c60b868ab8d973f6249d7e9ea2b30415d4b8a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409680"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="a1829-104">Тип ресурса educationSynchronizationLicenseAssignment</span><span class="sxs-lookup"><span data-stu-id="a1829-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="a1829-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a1829-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1829-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1829-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1829-107">Представляет информацию о лицензии для назначения учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="a1829-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="a1829-108">Ресурс будет использоваться для настройки назначения лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="a1829-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="a1829-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1829-109">Properties</span></span>

| <span data-ttu-id="a1829-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1829-110">Property</span></span> | <span data-ttu-id="a1829-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a1829-111">Type</span></span> | <span data-ttu-id="a1829-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a1829-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a1829-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="a1829-113">**appliesTo**</span></span> | <span data-ttu-id="a1829-114">string</span><span class="sxs-lookup"><span data-stu-id="a1829-114">string</span></span> | <span data-ttu-id="a1829-115">Тип роли пользователя для назначения лицензий.</span><span class="sxs-lookup"><span data-stu-id="a1829-115">The user role type to assign to license.</span></span> <span data-ttu-id="a1829-116">Возможные значения: `student`, `teacher`.</span><span class="sxs-lookup"><span data-stu-id="a1829-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="a1829-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="a1829-117">**skuIds**</span></span> | <span data-ttu-id="a1829-118">набор строк</span><span class="sxs-lookup"><span data-stu-id="a1829-118">collection of strings</span></span> |  <span data-ttu-id="a1829-119">Представляет идентификаторы SKU лицензий для назначения.</span><span class="sxs-lookup"><span data-stu-id="a1829-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="a1829-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1829-120">JSON representation</span></span>
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
