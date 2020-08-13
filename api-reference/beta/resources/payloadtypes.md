---
title: Тип ресурса Пайлоадтипес
description: Представляет данные уведомления о необработанном или визуальном пользователе, которое будет доставлено клиенту приложения, получающим это уведомление, и использоваться им.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: a35d48839e6932274f4257ce475710ea904878c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521985"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="88a0a-103">Тип ресурса Пайлоадтипес</span><span class="sxs-lookup"><span data-stu-id="88a0a-103">payloadTypes resource type</span></span>

<span data-ttu-id="88a0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88a0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a0a-105">Этот ресурс представляет данные о необработанном или визуальном уведомлении пользователя, которые будут доставлены и использованы клиентом приложения, получающим это уведомление.</span><span class="sxs-lookup"><span data-stu-id="88a0a-105">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="88a0a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="88a0a-106">Properties</span></span>

| <span data-ttu-id="88a0a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a0a-107">Property</span></span>     | <span data-ttu-id="88a0a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="88a0a-108">Type</span></span>        | <span data-ttu-id="88a0a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="88a0a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88a0a-110">равконтент</span><span class="sxs-lookup"><span data-stu-id="88a0a-110">rawContent</span></span>|<span data-ttu-id="88a0a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="88a0a-111">String</span></span>|<span data-ttu-id="88a0a-112">Контент уведомления необработанного пользователя, который будет доставляться и потребляться клиентом приложения на всех поддерживаемых платформах (Windows, iOS, Android или The-Push), получающих это уведомление.</span><span class="sxs-lookup"><span data-stu-id="88a0a-112">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="88a0a-113">По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="88a0a-113">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="88a0a-114">висуалконтент</span><span class="sxs-lookup"><span data-stu-id="88a0a-114">visualContent</span></span>|[<span data-ttu-id="88a0a-115">висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="88a0a-115">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="88a0a-116">Визуальное содержимое уведомления визуального пользователя, которое будет использоваться платформой уведомлений на каждой поддерживаемой платформе (только для Windows, iOS и Android) и визуализирована для пользователя.</span><span class="sxs-lookup"><span data-stu-id="88a0a-116">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="88a0a-117">По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="88a0a-117">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="88a0a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88a0a-118">JSON representation</span></span>

<span data-ttu-id="88a0a-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88a0a-119">The following is a JSON representation of the resource.</span></span>

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