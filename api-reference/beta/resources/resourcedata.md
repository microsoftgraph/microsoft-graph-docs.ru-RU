---
title: тип ресурса resourceData
description: Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: b2ddfd62a797cbf5674f522d6fa3c93eca528c30
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469369"
---
# <a name="resourcedata-resource-type"></a><span data-ttu-id="329ad-103">тип ресурса resourceData</span><span class="sxs-lookup"><span data-stu-id="329ad-103">resourceData resource type</span></span>

<span data-ttu-id="329ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="329ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="329ad-105">Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.</span><span class="sxs-lookup"><span data-stu-id="329ad-105">Represents the resouce data attached to the change notification sent to the subscriber.</span></span>

<span data-ttu-id="329ad-106">Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="329ad-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="329ad-107">Методы</span><span class="sxs-lookup"><span data-stu-id="329ad-107">Methods</span></span>

<span data-ttu-id="329ad-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="329ad-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="329ad-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="329ad-109">Properties</span></span>

<span data-ttu-id="329ad-110">Для ресурсов Outlook **resourceData содержит** следующие поля:</span><span class="sxs-lookup"><span data-stu-id="329ad-110">For Outlook resources, **resourceData** contains the following fields:</span></span>

| <span data-ttu-id="329ad-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="329ad-111">Property</span></span> | <span data-ttu-id="329ad-112">Тип</span><span class="sxs-lookup"><span data-stu-id="329ad-112">Type</span></span> | <span data-ttu-id="329ad-113">Описание</span><span class="sxs-lookup"><span data-stu-id="329ad-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="329ad-114">@odata.type</span><span class="sxs-lookup"><span data-stu-id="329ad-114">@odata.type</span></span> | <span data-ttu-id="329ad-115">строка</span><span class="sxs-lookup"><span data-stu-id="329ad-115">string</span></span> | <span data-ttu-id="329ad-116">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="329ad-116">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="329ad-117">@odata.id</span><span class="sxs-lookup"><span data-stu-id="329ad-117">@odata.id</span></span> | <span data-ttu-id="329ad-118">строка</span><span class="sxs-lookup"><span data-stu-id="329ad-118">string</span></span> | <span data-ttu-id="329ad-119">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="329ad-119">The OData identifier of the object.</span></span> |
| <span data-ttu-id="329ad-120">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="329ad-120">@odata.etag</span></span> | <span data-ttu-id="329ad-121">строка</span><span class="sxs-lookup"><span data-stu-id="329ad-121">string</span></span> | <span data-ttu-id="329ad-122">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="329ad-122">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="329ad-123">id</span><span class="sxs-lookup"><span data-stu-id="329ad-123">id</span></span> | <span data-ttu-id="329ad-124">строка</span><span class="sxs-lookup"><span data-stu-id="329ad-124">string</span></span> | <span data-ttu-id="329ad-125">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="329ad-125">The identifier of the object.</span></span> |

> <span data-ttu-id="329ad-126">**Примечание:** Значение, `id` предоставляемого **в resourceData,** допустимо на момент сгенерировании уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="329ad-126">**Note:** The `id` value provided in **resourceData** is valid at the time the change notification was generated.</span></span> <span data-ttu-id="329ad-127">Некоторые действия, например перенос сообщения в другую папку, могут привести к неодержительным действиям при обработке `id` уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="329ad-127">Some actions, such as moving a message to another folder, might result in the `id` no longer being valid when the change notification is processed.</span></span>

## <a name="relationships"></a><span data-ttu-id="329ad-128">Связи</span><span class="sxs-lookup"><span data-stu-id="329ad-128">Relationships</span></span>

<span data-ttu-id="329ad-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="329ad-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="329ad-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="329ad-130">JSON representation</span></span>

<span data-ttu-id="329ad-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="329ad-131">The following is a JSON representation of the resource.</span></span>

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


