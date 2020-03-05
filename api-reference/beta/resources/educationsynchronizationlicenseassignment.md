---
title: Тип ресурса Едукатионсинчронизатионлиценсеассигнмент
description: Представляет сведения о лицензии, назначаемые учетным записям пользователей. Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5c806b451cc7f757da09927a5732426b0971f2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500193"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="ad509-104">Тип ресурса Едукатионсинчронизатионлиценсеассигнмент</span><span class="sxs-lookup"><span data-stu-id="ad509-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="ad509-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ad509-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad509-106">Представляет сведения о лицензии, назначаемые учетным записям пользователей.</span><span class="sxs-lookup"><span data-stu-id="ad509-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="ad509-107">Ресурс будет использоваться для настройки назначенных лицензий при создании новых учетных записей пользователей.</span><span class="sxs-lookup"><span data-stu-id="ad509-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="ad509-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad509-108">Properties</span></span>

| <span data-ttu-id="ad509-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad509-109">Property</span></span> | <span data-ttu-id="ad509-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ad509-110">Type</span></span> | <span data-ttu-id="ad509-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ad509-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ad509-112">**Тег**</span><span class="sxs-lookup"><span data-stu-id="ad509-112">**appliesTo**</span></span> | <span data-ttu-id="ad509-113">строка</span><span class="sxs-lookup"><span data-stu-id="ad509-113">string</span></span> | <span data-ttu-id="ad509-114">Тип роли пользователя, назначаемый лицензии.</span><span class="sxs-lookup"><span data-stu-id="ad509-114">The user role type to assign to license.</span></span> <span data-ttu-id="ad509-115">Возможные значения: `student`, `teacher`, `faculty`.</span><span class="sxs-lookup"><span data-stu-id="ad509-115">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="ad509-116">**скуидс**</span><span class="sxs-lookup"><span data-stu-id="ad509-116">**skuIds**</span></span> | <span data-ttu-id="ad509-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad509-117">collection of strings</span></span> |  <span data-ttu-id="ad509-118">Представляет идентификаторы SKU назначаемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="ad509-118">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="ad509-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad509-119">JSON representation</span></span>
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
