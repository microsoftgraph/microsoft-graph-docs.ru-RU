---
title: Тип ресурса МитингпартиЦипантинфо
description: Сведения о участниках собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 68b89428b4bde76f957c77d6f1ee79105802a541
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522731"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="957af-103">Тип ресурса МитингпартиЦипантинфо</span><span class="sxs-lookup"><span data-stu-id="957af-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="957af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="957af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="957af-105">Сведения о участниках собрания.</span><span class="sxs-lookup"><span data-stu-id="957af-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="957af-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="957af-106">Properties</span></span>

| <span data-ttu-id="957af-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="957af-107">Property</span></span>       | <span data-ttu-id="957af-108">Тип</span><span class="sxs-lookup"><span data-stu-id="957af-108">Type</span></span>                          | <span data-ttu-id="957af-109">Описание</span><span class="sxs-lookup"><span data-stu-id="957af-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="957af-110">хищения</span><span class="sxs-lookup"><span data-stu-id="957af-110">identity</span></span>       | [<span data-ttu-id="957af-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="957af-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="957af-112">Сведения об удостоверении участника.</span><span class="sxs-lookup"><span data-stu-id="957af-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="957af-113">Основное</span><span class="sxs-lookup"><span data-stu-id="957af-113">upn</span></span>            | <span data-ttu-id="957af-114">String</span><span class="sxs-lookup"><span data-stu-id="957af-114">String</span></span>                        | <span data-ttu-id="957af-115">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="957af-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="957af-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="957af-116">JSON representation</span></span>

<span data-ttu-id="957af-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="957af-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
