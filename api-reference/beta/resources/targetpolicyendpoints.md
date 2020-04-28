---
title: Тип ресурса Таржетполициендпоинтс
description: Представляет платформы, предназначенные для уведомлений пользователей.
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 92ff6d0748e24fd58154f596188f25c51bdc6403
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520004"
---
# <a name="targetpolicyendpoints-resource-type"></a><span data-ttu-id="66d4e-103">Тип ресурса Таржетполициендпоинтс</span><span class="sxs-lookup"><span data-stu-id="66d4e-103">targetPolicyEndpoints resource type</span></span>

<span data-ttu-id="66d4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66d4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66d4e-105">Представляет платформы, которые могут быть предназначены для получения уведомлений, отправляемых пользователю.</span><span class="sxs-lookup"><span data-stu-id="66d4e-105">Represents the platforms that can be targeted to receive notifications sent to the user.</span></span>  <span data-ttu-id="66d4e-106">К ним относятся Windows, iOS, Android и веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="66d4e-106">These include Windows, iOS, Android and Web.</span></span> 


## <a name="properties"></a><span data-ttu-id="66d4e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="66d4e-107">Properties</span></span>

| <span data-ttu-id="66d4e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="66d4e-108">Property</span></span>     | <span data-ttu-id="66d4e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="66d4e-109">Type</span></span>        | <span data-ttu-id="66d4e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66d4e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="66d4e-111">платформтипес</span><span class="sxs-lookup"><span data-stu-id="66d4e-111">platformTypes</span></span>|<span data-ttu-id="66d4e-112">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="66d4e-112">String collection</span></span>|<span data-ttu-id="66d4e-113">Используется для фильтрации распространения уведомлений на определенную платформу или платформы.</span><span class="sxs-lookup"><span data-stu-id="66d4e-113">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="66d4e-114">Допустимые значения `Windows`: `iOS`, `Android` и `WebPush`.</span><span class="sxs-lookup"><span data-stu-id="66d4e-114">Valid values are `Windows`, `iOS`, `Android` and `WebPush`.</span></span> <span data-ttu-id="66d4e-115">По умолчанию все типы конечных точек Push (Windows, iOS, Android и Push) включены.</span><span class="sxs-lookup"><span data-stu-id="66d4e-115">By default, all push endpoint types (Windows, iOS, Android and WebPush) are enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66d4e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66d4e-116">JSON representation</span></span>

<span data-ttu-id="66d4e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66d4e-117">The following is a JSON representation of the resource.</span></span>

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