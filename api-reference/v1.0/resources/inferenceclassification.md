---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
localization_priority: Normal
ms.openlocfilehash: 8dfd76b31e452532181b46cdb0b5c321e92273a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840728"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="7f1b6-103">Тип ресурса inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="7f1b6-103">inferenceClassification resource type</span></span>

<span data-ttu-id="7f1b6-104">Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.</span><span class="sxs-lookup"><span data-stu-id="7f1b6-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="7f1b6-105">Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="7f1b6-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="7f1b6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7f1b6-106">Methods</span></span>

| <span data-ttu-id="7f1b6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7f1b6-107">Method</span></span>           | <span data-ttu-id="7f1b6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7f1b6-108">Return Type</span></span>    |<span data-ttu-id="7f1b6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1b6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f1b6-110">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="7f1b6-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="7f1b6-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="7f1b6-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="7f1b6-p101">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="7f1b6-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="7f1b6-114">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="7f1b6-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="7f1b6-115">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="7f1b6-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="7f1b6-116">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="7f1b6-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f1b6-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f1b6-117">Properties</span></span>
| <span data-ttu-id="7f1b6-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f1b6-118">Property</span></span>     | <span data-ttu-id="7f1b6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7f1b6-119">Type</span></span>   |<span data-ttu-id="7f1b6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1b6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f1b6-121">id</span><span class="sxs-lookup"><span data-stu-id="7f1b6-121">id</span></span>|<span data-ttu-id="7f1b6-122">строка</span><span class="sxs-lookup"><span data-stu-id="7f1b6-122">string</span></span>| <span data-ttu-id="7f1b6-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f1b6-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f1b6-124">Связи</span><span class="sxs-lookup"><span data-stu-id="7f1b6-124">Relationships</span></span>
| <span data-ttu-id="7f1b6-125">Связь</span><span class="sxs-lookup"><span data-stu-id="7f1b6-125">Relationship</span></span> | <span data-ttu-id="7f1b6-126">Тип</span><span class="sxs-lookup"><span data-stu-id="7f1b6-126">Type</span></span>   |<span data-ttu-id="7f1b6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1b6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f1b6-128">overrides</span><span class="sxs-lookup"><span data-stu-id="7f1b6-128">overrides</span></span>|<span data-ttu-id="7f1b6-129">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="7f1b6-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="7f1b6-p102">Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7f1b6-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f1b6-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f1b6-133">JSON representation</span></span>

<span data-ttu-id="7f1b6-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f1b6-134">Here is a JSON representation of the resource.</span></span>

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
