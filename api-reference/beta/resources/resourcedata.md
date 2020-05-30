---
title: Тип ресурса resourceData
description: Представляет данные ресурсов, вложенные в уведомление об изменении, отправляемое подписчику.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 0f962ddeb118f2f7e98cfa9cc5f3acc45f083071
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/30/2020
ms.locfileid: "44430603"
---
# <a name="resourcedata-resource-type"></a><span data-ttu-id="362b2-103">Тип ресурса resourceData</span><span class="sxs-lookup"><span data-stu-id="362b2-103">resourceData resource type</span></span>

<span data-ttu-id="362b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="362b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="362b2-105">Представляет данные ресурсов, вложенные в уведомление об изменении, отправляемое подписчику.</span><span class="sxs-lookup"><span data-stu-id="362b2-105">Represents the resouce data attached to the change notification sent to the subscriber.</span></span>

<span data-ttu-id="362b2-106">Дополнительные сведения см. [в статье Использование API Microsoft Graph для получения уведомлений об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="362b2-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="362b2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="362b2-107">Methods</span></span>

<span data-ttu-id="362b2-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="362b2-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="362b2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="362b2-109">Properties</span></span>

<span data-ttu-id="362b2-110">Для ресурсов Outlook **resourceData** содержит следующие поля:</span><span class="sxs-lookup"><span data-stu-id="362b2-110">For Outlook resources, **resourceData** contains the following fields:</span></span>

| <span data-ttu-id="362b2-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="362b2-111">Property</span></span> | <span data-ttu-id="362b2-112">Тип</span><span class="sxs-lookup"><span data-stu-id="362b2-112">Type</span></span> | <span data-ttu-id="362b2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="362b2-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="362b2-114">@odata.type</span><span class="sxs-lookup"><span data-stu-id="362b2-114">@odata.type</span></span> | <span data-ttu-id="362b2-115">string</span><span class="sxs-lookup"><span data-stu-id="362b2-115">string</span></span> | <span data-ttu-id="362b2-116">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="362b2-116">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="362b2-117">@odata.id</span><span class="sxs-lookup"><span data-stu-id="362b2-117">@odata.id</span></span> | <span data-ttu-id="362b2-118">string</span><span class="sxs-lookup"><span data-stu-id="362b2-118">string</span></span> | <span data-ttu-id="362b2-119">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="362b2-119">The OData identifier of the object.</span></span> |
| <span data-ttu-id="362b2-120">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="362b2-120">@odata.etag</span></span> | <span data-ttu-id="362b2-121">строка</span><span class="sxs-lookup"><span data-stu-id="362b2-121">string</span></span> | <span data-ttu-id="362b2-122">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="362b2-122">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="362b2-123">id</span><span class="sxs-lookup"><span data-stu-id="362b2-123">id</span></span> | <span data-ttu-id="362b2-124">строка</span><span class="sxs-lookup"><span data-stu-id="362b2-124">string</span></span> | <span data-ttu-id="362b2-125">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="362b2-125">The identifier of the object.</span></span> |

> <span data-ttu-id="362b2-126">**Примечание:** `id`Значение, указанное в **resourceData** , является допустимым во время создания уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="362b2-126">**Note:** The `id` value provided in **resourceData** is valid at the time the change notification was generated.</span></span> <span data-ttu-id="362b2-127">Некоторые действия, например перемещение сообщения в другую папку, могут привести к `id` недействительности при обработке уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="362b2-127">Some actions, such as moving a message to another folder, might result in the `id` no longer being valid when the change notification is processed.</span></span>

## <a name="relationships"></a><span data-ttu-id="362b2-128">Связи</span><span class="sxs-lookup"><span data-stu-id="362b2-128">Relationships</span></span>

<span data-ttu-id="362b2-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="362b2-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="362b2-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="362b2-130">JSON representation</span></span>

<span data-ttu-id="362b2-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="362b2-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "id": "1565293727947",
  "@odata.type": "#Microsoft.Graph.ChatMessage",
  "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
}
```

<!-- uuid: eb6c98ec-8257-4826-910e-5c603265257f
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource data resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
