---
title: Тип ресурса Чанжетраккедентити
description: ''
localization_priority: Normal
ms.openlocfilehash: 838aeca84b6928c709a3c4775c95ab3ef8fd7692
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33347946"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="1dd91-102">Тип ресурса Чанжетраккедентити</span><span class="sxs-lookup"><span data-stu-id="1dd91-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="1dd91-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dd91-103">Properties</span></span>
|<span data-ttu-id="1dd91-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dd91-104">Property</span></span>|<span data-ttu-id="1dd91-105">Тип</span><span class="sxs-lookup"><span data-stu-id="1dd91-105">Type</span></span>|<span data-ttu-id="1dd91-106">Описание</span><span class="sxs-lookup"><span data-stu-id="1dd91-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dd91-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dd91-107">createdDateTime</span></span>| <span data-ttu-id="1dd91-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dd91-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="1dd91-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dd91-109">lastModifiedDateTime</span></span>| <span data-ttu-id="1dd91-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dd91-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="1dd91-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1dd91-111">lastModifiedBy</span></span>| [<span data-ttu-id="1dd91-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="1dd91-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="1dd91-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="1dd91-113">Relationships</span></span>
<span data-ttu-id="1dd91-114">Нет</span><span class="sxs-lookup"><span data-stu-id="1dd91-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1dd91-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1dd91-115">JSON Representation</span></span>
<span data-ttu-id="1dd91-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dd91-116">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.changeTrackedEntity",
  "baseType":"microsoft.graph.entity",
  "abstract":true
}-->

``` json
{
    "createdDateTime":"String (timestamp)",
    "lastModifiedDateTime" :"String (timestamp)",
    "lastModifiedBy":{"@odata.type":"microsoft.graph.identitySet"}
}
```



