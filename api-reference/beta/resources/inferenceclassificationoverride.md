---
title: Тип ресурса inferenceClassificationOverride
description: Представляет переопределение пользователя, определяющее, как должны классифицироваться входящие сообщения от определенного отправителя
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 8e133a4dcfb227016b4b8436c315aef7719ba8e2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807558"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="e6273-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e6273-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="e6273-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6273-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6273-105">Представляет переопределение пользователя, которое всегда должно классифицироваться как входящие сообщения от определенного отправителя, как в [папке "отсортированные"](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="e6273-105">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="e6273-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e6273-106">Methods</span></span>

| <span data-ttu-id="e6273-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e6273-107">Method</span></span>           | <span data-ttu-id="e6273-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6273-108">Return Type</span></span>    |<span data-ttu-id="e6273-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e6273-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6273-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="e6273-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="e6273-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e6273-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="e6273-112">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="e6273-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|<span data-ttu-id="e6273-113">[удаление](../api/inferenceclassificationoverride-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e6273-113">[Delete](../api/inferenceclassificationoverride-delete.md)</span></span> | <span data-ttu-id="e6273-114">Нет</span><span class="sxs-lookup"><span data-stu-id="e6273-114">None</span></span> |<span data-ttu-id="e6273-115">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="e6273-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6273-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6273-116">Properties</span></span>
| <span data-ttu-id="e6273-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6273-117">Property</span></span>     | <span data-ttu-id="e6273-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e6273-118">Type</span></span>   |<span data-ttu-id="e6273-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e6273-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6273-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="e6273-120">classifyAs</span></span>|<span data-ttu-id="e6273-121">string</span><span class="sxs-lookup"><span data-stu-id="e6273-121">string</span></span>| <span data-ttu-id="e6273-p101">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e6273-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="e6273-124">id</span><span class="sxs-lookup"><span data-stu-id="e6273-124">id</span></span>|<span data-ttu-id="e6273-125">string</span><span class="sxs-lookup"><span data-stu-id="e6273-125">string</span></span>| <span data-ttu-id="e6273-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6273-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="e6273-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e6273-128">senderEmailAddress</span></span>|[<span data-ttu-id="e6273-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e6273-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e6273-130">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="e6273-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6273-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="e6273-131">Relationships</span></span>
<span data-ttu-id="e6273-132">Нет</span><span class="sxs-lookup"><span data-stu-id="e6273-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6273-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6273-133">JSON representation</span></span>

<span data-ttu-id="e6273-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6273-134">Here is a JSON representation of the resource.</span></span>

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
