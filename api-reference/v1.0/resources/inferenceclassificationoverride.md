---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c65bbecda618115e40a3c3cc36f2b952597b9c85
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808909"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="4bddb-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4bddb-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="4bddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bddb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4bddb-105">Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="4bddb-105">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="4bddb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4bddb-106">Methods</span></span>

| <span data-ttu-id="4bddb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4bddb-107">Method</span></span>           | <span data-ttu-id="4bddb-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4bddb-108">Return Type</span></span>    |<span data-ttu-id="4bddb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4bddb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bddb-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="4bddb-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="4bddb-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4bddb-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="4bddb-112">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="4bddb-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|<span data-ttu-id="4bddb-113">[удаление](../api/inferenceclassificationoverride-delete.md);</span><span class="sxs-lookup"><span data-stu-id="4bddb-113">[Delete](../api/inferenceclassificationoverride-delete.md)</span></span> | <span data-ttu-id="4bddb-114">Нет</span><span class="sxs-lookup"><span data-stu-id="4bddb-114">None</span></span> |<span data-ttu-id="4bddb-115">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="4bddb-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="4bddb-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bddb-116">Properties</span></span>
| <span data-ttu-id="4bddb-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bddb-117">Property</span></span>     | <span data-ttu-id="4bddb-118">Тип</span><span class="sxs-lookup"><span data-stu-id="4bddb-118">Type</span></span>   |<span data-ttu-id="4bddb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4bddb-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bddb-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="4bddb-120">classifyAs</span></span>|<span data-ttu-id="4bddb-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="4bddb-121">inferenceClassificationType</span></span>| <span data-ttu-id="4bddb-122">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="4bddb-122">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="4bddb-123">Возможные значения: `focused` , `other` .</span><span class="sxs-lookup"><span data-stu-id="4bddb-123">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="4bddb-124">id</span><span class="sxs-lookup"><span data-stu-id="4bddb-124">id</span></span>|<span data-ttu-id="4bddb-125">string</span><span class="sxs-lookup"><span data-stu-id="4bddb-125">string</span></span>| <span data-ttu-id="4bddb-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4bddb-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="4bddb-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4bddb-128">senderEmailAddress</span></span>|[<span data-ttu-id="4bddb-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4bddb-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="4bddb-130">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="4bddb-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bddb-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="4bddb-131">Relationships</span></span>
<span data-ttu-id="4bddb-132">Нет</span><span class="sxs-lookup"><span data-stu-id="4bddb-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4bddb-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bddb-133">JSON representation</span></span>

<span data-ttu-id="4bddb-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bddb-134">Here is a JSON representation of the resource.</span></span>

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
