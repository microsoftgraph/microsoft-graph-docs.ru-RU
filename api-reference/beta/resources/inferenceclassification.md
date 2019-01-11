---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
localization_priority: Normal
ms.openlocfilehash: 82d16e24e21231b8ec168eda793257ef780c2219
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877793"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="9f124-103">Тип ресурса inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="9f124-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="9f124-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f124-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f124-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f124-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f124-106">Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.</span><span class="sxs-lookup"><span data-stu-id="9f124-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="9f124-107">Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="9f124-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9f124-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9f124-108">Methods</span></span>

| <span data-ttu-id="9f124-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9f124-109">Method</span></span>           | <span data-ttu-id="9f124-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f124-110">Return Type</span></span>    |<span data-ttu-id="9f124-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f124-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f124-112">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9f124-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="9f124-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9f124-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="9f124-p102">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="9f124-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="9f124-116">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="9f124-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="9f124-117">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="9f124-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="9f124-118">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="9f124-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="9f124-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f124-119">Properties</span></span>
| <span data-ttu-id="9f124-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f124-120">Property</span></span>     | <span data-ttu-id="9f124-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9f124-121">Type</span></span>   |<span data-ttu-id="9f124-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9f124-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f124-123">id</span><span class="sxs-lookup"><span data-stu-id="9f124-123">id</span></span>|<span data-ttu-id="9f124-124">строка</span><span class="sxs-lookup"><span data-stu-id="9f124-124">string</span></span>| <span data-ttu-id="9f124-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f124-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f124-126">Связи</span><span class="sxs-lookup"><span data-stu-id="9f124-126">Relationships</span></span>
| <span data-ttu-id="9f124-127">Связь</span><span class="sxs-lookup"><span data-stu-id="9f124-127">Relationship</span></span> | <span data-ttu-id="9f124-128">Тип</span><span class="sxs-lookup"><span data-stu-id="9f124-128">Type</span></span>   |<span data-ttu-id="9f124-129">Описание</span><span class="sxs-lookup"><span data-stu-id="9f124-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f124-130">overrides</span><span class="sxs-lookup"><span data-stu-id="9f124-130">overrides</span></span>|<span data-ttu-id="9f124-131">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="9f124-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="9f124-p103">Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9f124-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f124-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f124-135">JSON representation</span></span>

<span data-ttu-id="9f124-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f124-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
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
