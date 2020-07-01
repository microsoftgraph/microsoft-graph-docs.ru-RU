---
title: Тип ресурса Чанженотификатионколлектион
description: Представляет коллекцию уведомлений о подписке, отправляемых подписчику.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 242ab35d95cfc35c19e6d1f37cefa33ee8bd1632
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45004801"
---
# <a name="changenotificationcollection-resource-type"></a><span data-ttu-id="5dfff-103">Тип ресурса Чанженотификатионколлектион</span><span class="sxs-lookup"><span data-stu-id="5dfff-103">changeNotificationCollection resource type</span></span>

<span data-ttu-id="5dfff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dfff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5dfff-105">Представляет коллекцию уведомлений об изменении ресурсов, отправляемых подписчику.</span><span class="sxs-lookup"><span data-stu-id="5dfff-105">Represents a collection of resource change notifications sent to the subscriber.</span></span>

<span data-ttu-id="5dfff-106">Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="5dfff-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5dfff-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5dfff-107">Methods</span></span>

<span data-ttu-id="5dfff-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="5dfff-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="5dfff-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dfff-109">Properties</span></span>

| <span data-ttu-id="5dfff-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dfff-110">Property</span></span> | <span data-ttu-id="5dfff-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5dfff-111">Type</span></span> | <span data-ttu-id="5dfff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5dfff-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5dfff-113">значение</span><span class="sxs-lookup"><span data-stu-id="5dfff-113">value</span></span> | <span data-ttu-id="5dfff-114">Коллекция ([чанженотификатион](changenotification.md))</span><span class="sxs-lookup"><span data-stu-id="5dfff-114">collection([changeNotification](changenotification.md))</span></span> | <span data-ttu-id="5dfff-115">Набор уведомлений, отправляемых на URL-адрес уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5dfff-115">The set of notifications being sent to the notification URL.</span></span> <span data-ttu-id="5dfff-116">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5dfff-116">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5dfff-117">Связи</span><span class="sxs-lookup"><span data-stu-id="5dfff-117">Relationships</span></span>

<span data-ttu-id="5dfff-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5dfff-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dfff-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5dfff-119">JSON representation</span></span>

<span data-ttu-id="5dfff-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dfff-120">The following is a JSON representation of the resource.</span></span>

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
