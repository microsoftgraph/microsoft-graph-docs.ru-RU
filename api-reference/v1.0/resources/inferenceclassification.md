---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ebb32964f07345eee8c1786c68e196003ed2c804
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054884"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="fb067-103">Тип ресурса inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="fb067-103">inferenceClassification resource type</span></span>

<span data-ttu-id="fb067-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb067-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb067-105">Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.</span><span class="sxs-lookup"><span data-stu-id="fb067-105">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span>

<span data-ttu-id="fb067-106">Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="fb067-106">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fb067-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fb067-107">Methods</span></span>

| <span data-ttu-id="fb067-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fb067-108">Method</span></span>           | <span data-ttu-id="fb067-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb067-109">Return Type</span></span>    |<span data-ttu-id="fb067-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb067-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb067-111">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fb067-111">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="fb067-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fb067-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="fb067-p101">Создание переопределения для отправителя, указанному по SMTP-адресу. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="fb067-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="fb067-115">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="fb067-115">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="fb067-116">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="fb067-116">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="fb067-117">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="fb067-117">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb067-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb067-118">Properties</span></span>
| <span data-ttu-id="fb067-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb067-119">Property</span></span>     | <span data-ttu-id="fb067-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fb067-120">Type</span></span>   |<span data-ttu-id="fb067-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fb067-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb067-122">id</span><span class="sxs-lookup"><span data-stu-id="fb067-122">id</span></span>|<span data-ttu-id="fb067-123">string</span><span class="sxs-lookup"><span data-stu-id="fb067-123">string</span></span>| <span data-ttu-id="fb067-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb067-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb067-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="fb067-125">Relationships</span></span>
| <span data-ttu-id="fb067-126">Связь</span><span class="sxs-lookup"><span data-stu-id="fb067-126">Relationship</span></span> | <span data-ttu-id="fb067-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fb067-127">Type</span></span>   |<span data-ttu-id="fb067-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fb067-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb067-129">overrides</span><span class="sxs-lookup"><span data-stu-id="fb067-129">overrides</span></span>|<span data-ttu-id="fb067-130">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="fb067-130">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="fb067-p102">Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fb067-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb067-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb067-134">JSON representation</span></span>

<span data-ttu-id="fb067-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb067-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

