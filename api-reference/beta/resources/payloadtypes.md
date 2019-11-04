---
title: Тип ресурса Пайлоадтипес
description: Представляет данные уведомления о необработанном или визуальном пользователе, которое будет доставлено клиенту приложения, получающим это уведомление, и использоваться им.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 2d740c5b19b363fa2534984bf059cd186b065e89
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939609"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="bf539-103">Тип ресурса Пайлоадтипес</span><span class="sxs-lookup"><span data-stu-id="bf539-103">payloadTypes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf539-104">Этот ресурс представляет данные о необработанном или визуальном уведомлении пользователя, которые будут доставлены и использованы клиентом приложения, получающим это уведомление.</span><span class="sxs-lookup"><span data-stu-id="bf539-104">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="bf539-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf539-105">Properties</span></span>

| <span data-ttu-id="bf539-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf539-106">Property</span></span>     | <span data-ttu-id="bf539-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bf539-107">Type</span></span>        | <span data-ttu-id="bf539-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bf539-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bf539-109">равконтент</span><span class="sxs-lookup"><span data-stu-id="bf539-109">rawContent</span></span>|<span data-ttu-id="bf539-110">Строка</span><span class="sxs-lookup"><span data-stu-id="bf539-110">String</span></span>|<span data-ttu-id="bf539-111">Контент уведомления необработанного пользователя, который будет доставляться и потребляться клиентом приложения на всех поддерживаемых платформах (Windows, iOS, Android или The-Push), получающих это уведомление.</span><span class="sxs-lookup"><span data-stu-id="bf539-111">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="bf539-112">По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="bf539-112">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="bf539-113">висуалконтент</span><span class="sxs-lookup"><span data-stu-id="bf539-113">visualContent</span></span>|[<span data-ttu-id="bf539-114">висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="bf539-114">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="bf539-115">Визуальное содержимое уведомления визуального пользователя, которое будет использоваться платформой уведомлений на каждой поддерживаемой платформе (только для Windows, iOS и Android) и визуализирована для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf539-115">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="bf539-116">По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="bf539-116">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="bf539-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf539-117">JSON representation</span></span>

<span data-ttu-id="bf539-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf539-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.payloadTypes",
  "baseType": null
}-->

```json
{
  "rawContent": "String",
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "payloadTypes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->