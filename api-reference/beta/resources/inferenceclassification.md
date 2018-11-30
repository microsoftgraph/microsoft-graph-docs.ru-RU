---
title: Тип ресурса inferenceClassification
description: 'Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях. '
ms.openlocfilehash: c1536ff2b88b1830c2f2a2bc5a7bed519782df4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074699"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="9472f-103">Тип ресурса inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="9472f-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="9472f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9472f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9472f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9472f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9472f-106">Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.</span><span class="sxs-lookup"><span data-stu-id="9472f-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="9472f-107">Дополнительные сведения см. в статье [Управление сортировкой почты](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="9472f-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9472f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9472f-108">Methods</span></span>

| <span data-ttu-id="9472f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9472f-109">Method</span></span>           | <span data-ttu-id="9472f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9472f-110">Return Type</span></span>    |<span data-ttu-id="9472f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9472f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9472f-112">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9472f-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="9472f-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9472f-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="9472f-p102">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="9472f-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="9472f-116">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="9472f-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="9472f-117">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="9472f-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="9472f-118">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="9472f-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="9472f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="9472f-119">Properties</span></span>
| <span data-ttu-id="9472f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="9472f-120">Property</span></span>     | <span data-ttu-id="9472f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9472f-121">Type</span></span>   |<span data-ttu-id="9472f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9472f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9472f-123">id</span><span class="sxs-lookup"><span data-stu-id="9472f-123">id</span></span>|<span data-ttu-id="9472f-124">строка</span><span class="sxs-lookup"><span data-stu-id="9472f-124">string</span></span>| <span data-ttu-id="9472f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9472f-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9472f-126">Связи</span><span class="sxs-lookup"><span data-stu-id="9472f-126">Relationships</span></span>
| <span data-ttu-id="9472f-127">Связь</span><span class="sxs-lookup"><span data-stu-id="9472f-127">Relationship</span></span> | <span data-ttu-id="9472f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="9472f-128">Type</span></span>   |<span data-ttu-id="9472f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="9472f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9472f-130">overrides</span><span class="sxs-lookup"><span data-stu-id="9472f-130">overrides</span></span>|<span data-ttu-id="9472f-131">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="9472f-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="9472f-p103">Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9472f-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9472f-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9472f-135">JSON representation</span></span>

<span data-ttu-id="9472f-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9472f-136">Here is a JSON representation of the resource.</span></span>

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