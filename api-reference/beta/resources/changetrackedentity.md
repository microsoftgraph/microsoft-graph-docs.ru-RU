---
title: Тип ресурса Чанжетраккедентити
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3815b22c7bd76a894df0e98415e0c30bb77decd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974059"
---
# <a name="changetrackedentity-resource-type"></a><span data-ttu-id="57faa-102">Тип ресурса Чанжетраккедентити</span><span class="sxs-lookup"><span data-stu-id="57faa-102">changeTrackedEntity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="57faa-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="57faa-103">Properties</span></span>
|<span data-ttu-id="57faa-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="57faa-104">Property</span></span>|<span data-ttu-id="57faa-105">Тип</span><span class="sxs-lookup"><span data-stu-id="57faa-105">Type</span></span>|<span data-ttu-id="57faa-106">Описание</span><span class="sxs-lookup"><span data-stu-id="57faa-106">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57faa-107">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57faa-107">createdDateTime</span></span>| <span data-ttu-id="57faa-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57faa-108">DateTimeOffset</span></span>| |
|<span data-ttu-id="57faa-109">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57faa-109">lastModifiedDateTime</span></span>| <span data-ttu-id="57faa-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57faa-110">DateTimeOffset</span></span>| |
|<span data-ttu-id="57faa-111">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="57faa-111">lastModifiedBy</span></span>| [<span data-ttu-id="57faa-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="57faa-112">identitySet</span></span>](identityset.md) | |

## <a name="relationships"></a><span data-ttu-id="57faa-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="57faa-113">Relationships</span></span>
<span data-ttu-id="57faa-114">Нет</span><span class="sxs-lookup"><span data-stu-id="57faa-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57faa-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57faa-115">JSON Representation</span></span>
<span data-ttu-id="57faa-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57faa-116">Here is a JSON representation of the resource.</span></span>
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



