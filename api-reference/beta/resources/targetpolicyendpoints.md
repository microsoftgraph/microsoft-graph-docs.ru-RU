---
title: Тип ресурса Таржетполициендпоинтс
description: Представляет платформы, предназначенные для уведомлений пользователей.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 9c1911900f4945d6f4b75d62c62457791fbb5c6a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939469"
---
# <a name="targetpolicyendpoints-resource-type"></a><span data-ttu-id="b8288-103">Тип ресурса Таржетполициендпоинтс</span><span class="sxs-lookup"><span data-stu-id="b8288-103">targetPolicyEndpoints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8288-104">Представляет платформы, которые могут быть предназначены для получения уведомлений, отправляемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="b8288-104">Represents the platforms that can be targeted to receive notifications sent to the user.</span></span>  <span data-ttu-id="b8288-105">К ним относятся Windows, iOS, Android и веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="b8288-105">These include Windows, iOS, Android and Web.</span></span> 


## <a name="properties"></a><span data-ttu-id="b8288-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8288-106">Properties</span></span>

| <span data-ttu-id="b8288-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8288-107">Property</span></span>     | <span data-ttu-id="b8288-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b8288-108">Type</span></span>        | <span data-ttu-id="b8288-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b8288-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8288-110">платформтипес</span><span class="sxs-lookup"><span data-stu-id="b8288-110">platformTypes</span></span>|<span data-ttu-id="b8288-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b8288-111">String collection</span></span>|<span data-ttu-id="b8288-112">Используется для фильтрации распространения уведомлений на определенную платформу или платформы.</span><span class="sxs-lookup"><span data-stu-id="b8288-112">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="b8288-113">Допустимые значения `Windows`: `iOS`, `Android` и `WebPush`.</span><span class="sxs-lookup"><span data-stu-id="b8288-113">Valid values are `Windows`, `iOS`, `Android` and `WebPush`.</span></span> <span data-ttu-id="b8288-114">По умолчанию все типы конечных точек Push (Windows, iOS, Android и Push) включены.</span><span class="sxs-lookup"><span data-stu-id="b8288-114">By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8288-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8288-115">JSON representation</span></span>

<span data-ttu-id="b8288-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8288-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetPolicyEndpoints",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetPolicyEndpoints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->