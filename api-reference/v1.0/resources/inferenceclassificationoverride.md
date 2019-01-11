---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
ms.openlocfilehash: 8df0f1e5fa34c630c51de7c73234e6092448f867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885066"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="1d818-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="1d818-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="1d818-104">Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="1d818-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="1d818-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1d818-105">Methods</span></span>

| <span data-ttu-id="1d818-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1d818-106">Method</span></span>           | <span data-ttu-id="1d818-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d818-107">Return Type</span></span>    |<span data-ttu-id="1d818-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1d818-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d818-109">[обновление](../api/inferenceclassificationoverride-update.md).</span><span class="sxs-lookup"><span data-stu-id="1d818-109">[Update](../api/inferenceclassificationoverride-update.md)</span></span> | [<span data-ttu-id="1d818-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="1d818-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="1d818-111">Изменение поля **ClassifyAs** переопределения, указанный.</span><span class="sxs-lookup"><span data-stu-id="1d818-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="1d818-112">Delete</span><span class="sxs-lookup"><span data-stu-id="1d818-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="1d818-113">Нет</span><span class="sxs-lookup"><span data-stu-id="1d818-113">None</span></span> |<span data-ttu-id="1d818-114">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="1d818-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d818-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d818-115">Properties</span></span>
| <span data-ttu-id="1d818-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d818-116">Property</span></span>     | <span data-ttu-id="1d818-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1d818-117">Type</span></span>   |<span data-ttu-id="1d818-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1d818-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d818-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="1d818-119">classifyAs</span></span>|<span data-ttu-id="1d818-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="1d818-120">inferenceClassificationType</span></span>| <span data-ttu-id="1d818-121">Указывает, как входящие сообщения из определенной отправитель всегда должен следует рассматривать как.</span><span class="sxs-lookup"><span data-stu-id="1d818-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="1d818-122">Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="1d818-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="1d818-123">id</span><span class="sxs-lookup"><span data-stu-id="1d818-123">id</span></span>|<span data-ttu-id="1d818-124">строка</span><span class="sxs-lookup"><span data-stu-id="1d818-124">string</span></span>| <span data-ttu-id="1d818-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d818-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="1d818-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1d818-127">senderEmailAddress</span></span>|[<span data-ttu-id="1d818-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1d818-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="1d818-129">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="1d818-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d818-130">Связи</span><span class="sxs-lookup"><span data-stu-id="1d818-130">Relationships</span></span>
<span data-ttu-id="1d818-131">Нет</span><span class="sxs-lookup"><span data-stu-id="1d818-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1d818-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d818-132">JSON representation</span></span>

<span data-ttu-id="1d818-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d818-133">Here is a JSON representation of the resource.</span></span>

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
