---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a80283bd3f32c28b71d02acd2ae93e76cac1299
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531306"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="0f299-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="0f299-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="0f299-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f299-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f299-105">Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="0f299-105">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="0f299-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0f299-106">Methods</span></span>

| <span data-ttu-id="0f299-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0f299-107">Method</span></span>           | <span data-ttu-id="0f299-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f299-108">Return Type</span></span>    |<span data-ttu-id="0f299-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f299-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f299-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="0f299-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="0f299-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="0f299-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="0f299-112">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="0f299-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="0f299-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="0f299-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="0f299-114">Нет</span><span class="sxs-lookup"><span data-stu-id="0f299-114">None</span></span> |<span data-ttu-id="0f299-115">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="0f299-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f299-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f299-116">Properties</span></span>
| <span data-ttu-id="0f299-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f299-117">Property</span></span>     | <span data-ttu-id="0f299-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0f299-118">Type</span></span>   |<span data-ttu-id="0f299-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0f299-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f299-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="0f299-120">classifyAs</span></span>|<span data-ttu-id="0f299-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="0f299-121">inferenceClassificationType</span></span>| <span data-ttu-id="0f299-122">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="0f299-122">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="0f299-123">Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="0f299-123">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="0f299-124">id</span><span class="sxs-lookup"><span data-stu-id="0f299-124">id</span></span>|<span data-ttu-id="0f299-125">string</span><span class="sxs-lookup"><span data-stu-id="0f299-125">string</span></span>| <span data-ttu-id="0f299-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f299-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="0f299-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0f299-128">senderEmailAddress</span></span>|[<span data-ttu-id="0f299-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0f299-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0f299-130">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="0f299-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f299-131">Связи</span><span class="sxs-lookup"><span data-stu-id="0f299-131">Relationships</span></span>
<span data-ttu-id="0f299-132">Нет</span><span class="sxs-lookup"><span data-stu-id="0f299-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0f299-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f299-133">JSON representation</span></span>

<span data-ttu-id="0f299-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f299-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
