---
title: тип ресурса resourceData
description: Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: d852268ee1a007b60014a224b34d12f25100fe8c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467969"
---
# <a name="resourcedata-resource-type"></a><span data-ttu-id="6fd29-103">тип ресурса resourceData</span><span class="sxs-lookup"><span data-stu-id="6fd29-103">resourceData resource type</span></span>

<span data-ttu-id="6fd29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fd29-105">Представляет данные resouce, присоединенные к уведомлению об изменении, отправленным абоненту.</span><span class="sxs-lookup"><span data-stu-id="6fd29-105">Represents the resouce data attached to the change notification sent to the subscriber.</span></span>

<span data-ttu-id="6fd29-106">Подробности см. в статье [Получение уведомлений об изменениях с помощью API Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="6fd29-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6fd29-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6fd29-107">Methods</span></span>

<span data-ttu-id="6fd29-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="6fd29-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="6fd29-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fd29-109">Properties</span></span>

<span data-ttu-id="6fd29-110">Для ресурсов Outlook **resourceData содержит** следующие поля:</span><span class="sxs-lookup"><span data-stu-id="6fd29-110">For Outlook resources, **resourceData** contains the following fields:</span></span>

| <span data-ttu-id="6fd29-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fd29-111">Property</span></span> | <span data-ttu-id="6fd29-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6fd29-112">Type</span></span> | <span data-ttu-id="6fd29-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6fd29-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="6fd29-114">@odata.type</span><span class="sxs-lookup"><span data-stu-id="6fd29-114">@odata.type</span></span> | <span data-ttu-id="6fd29-115">строка</span><span class="sxs-lookup"><span data-stu-id="6fd29-115">string</span></span> | <span data-ttu-id="6fd29-116">@odata.type — тип сущности OData в Microsoft Graph, который описывает представленный объект.</span><span class="sxs-lookup"><span data-stu-id="6fd29-116">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="6fd29-117">@odata.id</span><span class="sxs-lookup"><span data-stu-id="6fd29-117">@odata.id</span></span> | <span data-ttu-id="6fd29-118">строка</span><span class="sxs-lookup"><span data-stu-id="6fd29-118">string</span></span> | <span data-ttu-id="6fd29-119">@odata.id — идентификатор OData для объекта.</span><span class="sxs-lookup"><span data-stu-id="6fd29-119">The OData identifier of the object.</span></span> |
| <span data-ttu-id="6fd29-120">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="6fd29-120">@odata.etag</span></span> | <span data-ttu-id="6fd29-121">строка</span><span class="sxs-lookup"><span data-stu-id="6fd29-121">string</span></span> | <span data-ttu-id="6fd29-122">@odata.etag — HTTP-тег сущности, представляющий версию объекта.</span><span class="sxs-lookup"><span data-stu-id="6fd29-122">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="6fd29-123">id</span><span class="sxs-lookup"><span data-stu-id="6fd29-123">id</span></span> | <span data-ttu-id="6fd29-124">строка</span><span class="sxs-lookup"><span data-stu-id="6fd29-124">string</span></span> | <span data-ttu-id="6fd29-125">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="6fd29-125">The identifier of the object.</span></span> |

> <span data-ttu-id="6fd29-126">**Примечание:** Значение, `id` предоставляемого **в resourceData,** допустимо на момент сгенерировании уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="6fd29-126">**Note:** The `id` value provided in **resourceData** is valid at the time the change notification was generated.</span></span> <span data-ttu-id="6fd29-127">Некоторые действия, например перенос сообщения в другую папку, могут привести к неодержительным действиям при обработке `id` уведомления об изменении.</span><span class="sxs-lookup"><span data-stu-id="6fd29-127">Some actions, such as moving a message to another folder, might result in the `id` no longer being valid when the change notification is processed.</span></span>

## <a name="relationships"></a><span data-ttu-id="6fd29-128">Связи</span><span class="sxs-lookup"><span data-stu-id="6fd29-128">Relationships</span></span>

<span data-ttu-id="6fd29-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6fd29-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fd29-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6fd29-130">JSON representation</span></span>

<span data-ttu-id="6fd29-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fd29-131">The following is a JSON representation of the resource.</span></span>

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

