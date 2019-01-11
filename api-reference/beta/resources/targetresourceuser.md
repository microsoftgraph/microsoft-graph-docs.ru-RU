---
title: Тип ресурса targetResourceUser
description: Указывает объект пользователя, который был добавлен, обновлении или удалении администраторами с как часть аудита активности. На основе targetResource ресурсов.
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831930"
---
# <a name="targetresourceuser-resource-type"></a><span data-ttu-id="1168d-104">Тип ресурса targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="1168d-104">targetResourceUser resource type</span></span>
<span data-ttu-id="1168d-105">Указывает объект пользователя, который был добавлен, обновлении или удалении администраторами с как часть аудита активности.</span><span class="sxs-lookup"><span data-stu-id="1168d-105">Indicates the user object that was added, updated or deleted by admins as part of audit activity.</span></span> <span data-ttu-id="1168d-106">На основе [targetResource](targetresource.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1168d-106">Derived from the [targetResource](targetresource.md) resource.</span></span>


## <a name="properties"></a><span data-ttu-id="1168d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1168d-107">Properties</span></span>
| <span data-ttu-id="1168d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1168d-108">Property</span></span>     | <span data-ttu-id="1168d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1168d-109">Type</span></span>   |<span data-ttu-id="1168d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1168d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1168d-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1168d-111">userPrincipalName</span></span>|<span data-ttu-id="1168d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="1168d-112">String</span></span>|<span data-ttu-id="1168d-113">Указывает уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1168d-113">Indicates the Unique Id of the User.</span></span> <span data-ttu-id="1168d-114">Ссылается на идентификатор пользователя для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1168d-114">Refers to User Id for a specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1168d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1168d-115">JSON representation</span></span>

<span data-ttu-id="1168d-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1168d-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
