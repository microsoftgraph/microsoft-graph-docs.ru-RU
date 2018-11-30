---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
ms.openlocfilehash: 0fb1e01ad9710a0ff5f2de7f63808a6f3e988c13
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025262"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="788b3-103">Тип ресурса inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="788b3-103">inferenceClassification resource type</span></span>

<span data-ttu-id="788b3-104">Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.</span><span class="sxs-lookup"><span data-stu-id="788b3-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="788b3-105">Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="788b3-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="788b3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="788b3-106">Methods</span></span>

| <span data-ttu-id="788b3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="788b3-107">Method</span></span>           | <span data-ttu-id="788b3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="788b3-108">Return Type</span></span>    |<span data-ttu-id="788b3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="788b3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="788b3-110">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="788b3-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="788b3-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="788b3-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="788b3-p101">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="788b3-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="788b3-114">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="788b3-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="788b3-115">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="788b3-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="788b3-116">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="788b3-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="788b3-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="788b3-117">Properties</span></span>
| <span data-ttu-id="788b3-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="788b3-118">Property</span></span>     | <span data-ttu-id="788b3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="788b3-119">Type</span></span>   |<span data-ttu-id="788b3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="788b3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="788b3-121">id</span><span class="sxs-lookup"><span data-stu-id="788b3-121">id</span></span>|<span data-ttu-id="788b3-122">строка</span><span class="sxs-lookup"><span data-stu-id="788b3-122">string</span></span>| <span data-ttu-id="788b3-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="788b3-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="788b3-124">Связи</span><span class="sxs-lookup"><span data-stu-id="788b3-124">Relationships</span></span>
| <span data-ttu-id="788b3-125">Связь</span><span class="sxs-lookup"><span data-stu-id="788b3-125">Relationship</span></span> | <span data-ttu-id="788b3-126">Тип</span><span class="sxs-lookup"><span data-stu-id="788b3-126">Type</span></span>   |<span data-ttu-id="788b3-127">Описание</span><span class="sxs-lookup"><span data-stu-id="788b3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="788b3-128">overrides</span><span class="sxs-lookup"><span data-stu-id="788b3-128">overrides</span></span>|<span data-ttu-id="788b3-129">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="788b3-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="788b3-p102">Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="788b3-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="788b3-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="788b3-133">JSON representation</span></span>

<span data-ttu-id="788b3-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="788b3-134">Here is a JSON representation of the resource.</span></span>

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