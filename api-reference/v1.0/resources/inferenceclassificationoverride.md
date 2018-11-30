---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
ms.openlocfilehash: 3f3f07e870a4ba549062197a380633ab591c54fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026215"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="2023d-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2023d-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="2023d-104">Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="2023d-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="2023d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2023d-105">Methods</span></span>

| <span data-ttu-id="2023d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2023d-106">Method</span></span>           | <span data-ttu-id="2023d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2023d-107">Return Type</span></span>    |<span data-ttu-id="2023d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2023d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2023d-109">Update</span><span class="sxs-lookup"><span data-stu-id="2023d-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="2023d-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2023d-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="2023d-111">Изменение поля **ClassifyAs** переопределения, указанный.</span><span class="sxs-lookup"><span data-stu-id="2023d-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="2023d-112">Delete</span><span class="sxs-lookup"><span data-stu-id="2023d-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="2023d-113">Нет</span><span class="sxs-lookup"><span data-stu-id="2023d-113">None</span></span> |<span data-ttu-id="2023d-114">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="2023d-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="2023d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="2023d-115">Properties</span></span>
| <span data-ttu-id="2023d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="2023d-116">Property</span></span>     | <span data-ttu-id="2023d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="2023d-117">Type</span></span>   |<span data-ttu-id="2023d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2023d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2023d-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="2023d-119">classifyAs</span></span>|<span data-ttu-id="2023d-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="2023d-120">inferenceClassificationType</span></span>| <span data-ttu-id="2023d-121">Указывает, как входящие сообщения из определенной отправитель всегда должен следует рассматривать как.</span><span class="sxs-lookup"><span data-stu-id="2023d-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="2023d-122">Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="2023d-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="2023d-123">id</span><span class="sxs-lookup"><span data-stu-id="2023d-123">id</span></span>|<span data-ttu-id="2023d-124">строка</span><span class="sxs-lookup"><span data-stu-id="2023d-124">string</span></span>| <span data-ttu-id="2023d-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2023d-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="2023d-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2023d-127">senderEmailAddress</span></span>|[<span data-ttu-id="2023d-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2023d-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="2023d-129">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="2023d-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2023d-130">Связи</span><span class="sxs-lookup"><span data-stu-id="2023d-130">Relationships</span></span>
<span data-ttu-id="2023d-131">Нет</span><span class="sxs-lookup"><span data-stu-id="2023d-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2023d-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2023d-132">JSON representation</span></span>

<span data-ttu-id="2023d-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2023d-133">Here is a JSON representation of the resource.</span></span>

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