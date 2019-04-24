---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2ab19f992dd7fac48844cd46a0600a0242517709
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463283"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="6bdc2-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="6bdc2-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bdc2-104">Тип Сервицехостедмедиаконфиг.</span><span class="sxs-lookup"><span data-stu-id="6bdc2-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="6bdc2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bdc2-105">Properties</span></span>

| <span data-ttu-id="6bdc2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bdc2-106">Property</span></span>                    | <span data-ttu-id="6bdc2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6bdc2-107">Type</span></span>                                                        | <span data-ttu-id="6bdc2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6bdc2-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="6bdc2-109">Префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="6bdc2-109">preFetchMedia</span></span>               | <span data-ttu-id="6bdc2-110">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="6bdc2-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="6bdc2-111">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="6bdc2-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="6bdc2-112">Ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="6bdc2-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="6bdc2-113">Логический</span><span class="sxs-lookup"><span data-stu-id="6bdc2-113">Boolean</span></span>                                                     | <span data-ttu-id="6bdc2-114">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6bdc2-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6bdc2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bdc2-115">JSON representation</span></span>

<span data-ttu-id="6bdc2-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bdc2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "#microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="6bdc2-117">Пример</span><span class="sxs-lookup"><span data-stu-id="6bdc2-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/servicehostedmediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
