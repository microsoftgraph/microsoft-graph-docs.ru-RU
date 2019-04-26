---
title: Тип ресурса Нетворклокатиондетаил
description: Показывает сведения, связанные с сетевым расположением. .
localization_priority: Normal
ms.openlocfilehash: bfa84591f543253ed794016bbc2d25d325cd0bcc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581445"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="25183-104">Тип ресурса Нетворклокатиондетаил</span><span class="sxs-lookup"><span data-stu-id="25183-104">networkLocationDetail resource type</span></span>
<span data-ttu-id="25183-105">Показывает сведения, связанные с сетевым расположением.</span><span class="sxs-lookup"><span data-stu-id="25183-105">Indicates details associated with the network location.</span></span> <span data-ttu-id="25183-106">.</span><span class="sxs-lookup"><span data-stu-id="25183-106"></span></span>



## <a name="properties"></a><span data-ttu-id="25183-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="25183-107">Properties</span></span>
| <span data-ttu-id="25183-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="25183-108">Property</span></span>     | <span data-ttu-id="25183-109">Тип</span><span class="sxs-lookup"><span data-stu-id="25183-109">Type</span></span>   |<span data-ttu-id="25183-110">Описание</span><span class="sxs-lookup"><span data-stu-id="25183-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25183-111">Нетворктипе</span><span class="sxs-lookup"><span data-stu-id="25183-111">networkType</span></span>|<span data-ttu-id="25183-112">String</span><span class="sxs-lookup"><span data-stu-id="25183-112">String</span></span>|<span data-ttu-id="25183-113">Предоставляет тип сети.</span><span class="sxs-lookup"><span data-stu-id="25183-113">Provides the type of the network.</span></span> <span data-ttu-id="25183-114">Возможные значения: `intranet`, `extranet` `namedNetwork`, и `trusted`.</span><span class="sxs-lookup"><span data-stu-id="25183-114">Possible values are `intranet`, `extranet`, `namedNetwork`, and `trusted`.</span></span>|
|<span data-ttu-id="25183-115">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="25183-115">networkName</span></span>|<span data-ttu-id="25183-116">String</span><span class="sxs-lookup"><span data-stu-id="25183-116">String</span></span>|<span data-ttu-id="25183-117">Имя сети.</span><span class="sxs-lookup"><span data-stu-id="25183-117">Name of the network.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="25183-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25183-118">JSON representation</span></span>

<span data-ttu-id="25183-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25183-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "networkTypes": "namedNetork",
  "networkName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
