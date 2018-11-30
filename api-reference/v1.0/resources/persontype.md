---
title: тип ресурса personType
description: Представляет тип пользователя.
ms.openlocfilehash: 3938be8d1dd0bf4a4934de4bbcd7862185971128
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025194"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="b8fd5-103">тип ресурса personType</span><span class="sxs-lookup"><span data-stu-id="b8fd5-103">personType resource type</span></span>

<span data-ttu-id="b8fd5-104">Представляет тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8fd5-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8fd5-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b8fd5-105">JSON representation</span></span>

<span data-ttu-id="b8fd5-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8fd5-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b8fd5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8fd5-107">Properties</span></span>
| <span data-ttu-id="b8fd5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8fd5-108">Property</span></span>     | <span data-ttu-id="b8fd5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8fd5-109">Type</span></span>   |<span data-ttu-id="b8fd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8fd5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8fd5-111">класс</span><span class="sxs-lookup"><span data-stu-id="b8fd5-111">class</span></span>|<span data-ttu-id="b8fd5-112">String</span><span class="sxs-lookup"><span data-stu-id="b8fd5-112">String</span></span>|<span data-ttu-id="b8fd5-113">Тип источника данных, например Person.</span><span class="sxs-lookup"><span data-stu-id="b8fd5-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="b8fd5-114">subclass</span><span class="sxs-lookup"><span data-stu-id="b8fd5-114">subclass</span></span>|<span data-ttu-id="b8fd5-115">String</span><span class="sxs-lookup"><span data-stu-id="b8fd5-115">String</span></span>|<span data-ttu-id="b8fd5-116">Дополнительный тип источника данных, например OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="b8fd5-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
