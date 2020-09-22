---
title: Тип ресурса Пайлоадтипес
description: Представляет данные уведомления о необработанном или визуальном пользователе, которое будет доставлено клиенту приложения, получающим это уведомление, и использоваться им.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 034770f2614bacdb9d160f4ff8d2efb4cd0a2c24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998105"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="748ba-103">Тип ресурса Пайлоадтипес</span><span class="sxs-lookup"><span data-stu-id="748ba-103">payloadTypes resource type</span></span>

<span data-ttu-id="748ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="748ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="748ba-105">Этот ресурс представляет данные о необработанном или визуальном уведомлении пользователя, которые будут доставлены и использованы клиентом приложения, получающим это уведомление.</span><span class="sxs-lookup"><span data-stu-id="748ba-105">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="748ba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="748ba-106">Properties</span></span>

| <span data-ttu-id="748ba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="748ba-107">Property</span></span>     | <span data-ttu-id="748ba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="748ba-108">Type</span></span>        | <span data-ttu-id="748ba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="748ba-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="748ba-110">равконтент</span><span class="sxs-lookup"><span data-stu-id="748ba-110">rawContent</span></span>|<span data-ttu-id="748ba-111">String</span><span class="sxs-lookup"><span data-stu-id="748ba-111">String</span></span>|<span data-ttu-id="748ba-112">Контент уведомления необработанного пользователя, который будет доставляться и потребляться клиентом приложения на всех поддерживаемых платформах (Windows, iOS, Android или The-Push), получающих это уведомление.</span><span class="sxs-lookup"><span data-stu-id="748ba-112">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="748ba-113">По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="748ba-113">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="748ba-114">висуалконтент</span><span class="sxs-lookup"><span data-stu-id="748ba-114">visualContent</span></span>|[<span data-ttu-id="748ba-115">висуалпропертиес</span><span class="sxs-lookup"><span data-stu-id="748ba-115">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="748ba-116">Визуальное содержимое уведомления визуального пользователя, которое будет использоваться платформой уведомлений на каждой поддерживаемой платформе (только для Windows, iOS и Android) и визуализирована для пользователя.</span><span class="sxs-lookup"><span data-stu-id="748ba-116">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="748ba-117">По крайней мере один из полезных данных. Равконтент или полезная нагрузка. Висуалконтент должен быть допустимым для запроса на уведомление POST.</span><span class="sxs-lookup"><span data-stu-id="748ba-117">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="748ba-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="748ba-118">JSON representation</span></span>

<span data-ttu-id="748ba-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="748ba-119">The following is a JSON representation of the resource.</span></span>

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

