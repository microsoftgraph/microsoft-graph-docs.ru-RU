---
title: Тип ресурса changeNotificationCollection
description: Представляет коллекцию уведомлений о подписке, отправляемых подписчику.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1eadd0fbc14fe9e6581ab6fa3375837653fc0859
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598511"
---
# <a name="changenotificationcollection-resource-type"></a><span data-ttu-id="bf67d-103">Тип ресурса changeNotificationCollection</span><span class="sxs-lookup"><span data-stu-id="bf67d-103">changeNotificationCollection resource type</span></span>

<span data-ttu-id="bf67d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf67d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf67d-105">Представляет коллекцию уведомлений об изменении ресурсов, отправляемых подписчику.</span><span class="sxs-lookup"><span data-stu-id="bf67d-105">Represents a collection of resource change notifications sent to the subscriber.</span></span>

<span data-ttu-id="bf67d-106">Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="bf67d-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bf67d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bf67d-107">Methods</span></span>

<span data-ttu-id="bf67d-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf67d-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="bf67d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf67d-109">Properties</span></span>

| <span data-ttu-id="bf67d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf67d-110">Property</span></span> | <span data-ttu-id="bf67d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bf67d-111">Type</span></span> | <span data-ttu-id="bf67d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bf67d-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="bf67d-113">значение</span><span class="sxs-lookup"><span data-stu-id="bf67d-113">value</span></span> | <span data-ttu-id="bf67d-114">Коллекция ([чанженотификатион](changenotification.md))</span><span class="sxs-lookup"><span data-stu-id="bf67d-114">collection([changeNotification](changenotification.md))</span></span> | <span data-ttu-id="bf67d-115">Набор уведомлений, отправляемых на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="bf67d-115">The set of notifications being sent to the notification URL.</span></span> <span data-ttu-id="bf67d-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf67d-116">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bf67d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="bf67d-117">Relationships</span></span>

<span data-ttu-id="bf67d-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bf67d-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf67d-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bf67d-119">JSON representation</span></span>

<span data-ttu-id="bf67d-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf67d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}-->

```json
{
  "value": [],
  "validationTokens": [
    "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
  ]
}
```

<!-- uuid: 8cc2599e-9740-4191-93fa-bc13c6f91564
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification collection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
