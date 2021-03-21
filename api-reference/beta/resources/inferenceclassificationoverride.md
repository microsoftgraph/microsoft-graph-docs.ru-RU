---
title: Тип ресурса inferenceClassificationOverride
description: Представляет переопределения пользователя в том, как всегда следует классифицировать входящие сообщения от конкретного отправи-
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 537032c220ed98fc9052afe6a31376359836fa94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954999"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="22d12-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="22d12-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="22d12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d12-105">Представляет переопределения пользователя в том, как всегда следует классифицировать входящие сообщения от конкретного отправитель, как в [сфокусированных почтовых ящиках.](manage-focused-inbox.md)</span><span class="sxs-lookup"><span data-stu-id="22d12-105">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="22d12-106">Методы</span><span class="sxs-lookup"><span data-stu-id="22d12-106">Methods</span></span>

| <span data-ttu-id="22d12-107">Метод</span><span class="sxs-lookup"><span data-stu-id="22d12-107">Method</span></span>           | <span data-ttu-id="22d12-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22d12-108">Return Type</span></span>    |<span data-ttu-id="22d12-109">Описание</span><span class="sxs-lookup"><span data-stu-id="22d12-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22d12-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="22d12-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="22d12-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="22d12-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="22d12-112">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="22d12-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|<span data-ttu-id="22d12-113">[удаление](../api/inferenceclassificationoverride-delete.md);</span><span class="sxs-lookup"><span data-stu-id="22d12-113">[Delete](../api/inferenceclassificationoverride-delete.md)</span></span> | <span data-ttu-id="22d12-114">Нет</span><span class="sxs-lookup"><span data-stu-id="22d12-114">None</span></span> |<span data-ttu-id="22d12-115">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="22d12-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="22d12-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="22d12-116">Properties</span></span>
| <span data-ttu-id="22d12-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="22d12-117">Property</span></span>     | <span data-ttu-id="22d12-118">Тип</span><span class="sxs-lookup"><span data-stu-id="22d12-118">Type</span></span>   |<span data-ttu-id="22d12-119">Описание</span><span class="sxs-lookup"><span data-stu-id="22d12-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d12-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="22d12-120">classifyAs</span></span>|<span data-ttu-id="22d12-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="22d12-121">inferenceClassificationType</span></span>| <span data-ttu-id="22d12-p101">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="22d12-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="22d12-124">id</span><span class="sxs-lookup"><span data-stu-id="22d12-124">id</span></span>|<span data-ttu-id="22d12-125">string</span><span class="sxs-lookup"><span data-stu-id="22d12-125">string</span></span>| <span data-ttu-id="22d12-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22d12-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="22d12-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="22d12-128">senderEmailAddress</span></span>|[<span data-ttu-id="22d12-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="22d12-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="22d12-130">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="22d12-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22d12-131">Связи</span><span class="sxs-lookup"><span data-stu-id="22d12-131">Relationships</span></span>
<span data-ttu-id="22d12-132">Нет</span><span class="sxs-lookup"><span data-stu-id="22d12-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="22d12-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22d12-133">JSON representation</span></span>

<span data-ttu-id="22d12-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22d12-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


