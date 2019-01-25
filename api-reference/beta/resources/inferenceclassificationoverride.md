---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511802"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="20093-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="20093-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20093-104">Представляет пользователя переопределения для способ входящих сообщений от определенного отправителя всегда следует рассматривать как и [Фокус папки «Входящие»](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="20093-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="20093-105">Методы</span><span class="sxs-lookup"><span data-stu-id="20093-105">Methods</span></span>

| <span data-ttu-id="20093-106">Метод</span><span class="sxs-lookup"><span data-stu-id="20093-106">Method</span></span>           | <span data-ttu-id="20093-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20093-107">Return Type</span></span>    |<span data-ttu-id="20093-108">Описание</span><span class="sxs-lookup"><span data-stu-id="20093-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20093-109">Update</span><span class="sxs-lookup"><span data-stu-id="20093-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="20093-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="20093-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="20093-111">Изменение поля **classifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="20093-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="20093-112">Delete</span><span class="sxs-lookup"><span data-stu-id="20093-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="20093-113">Нет</span><span class="sxs-lookup"><span data-stu-id="20093-113">None</span></span> |<span data-ttu-id="20093-114">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="20093-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="20093-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="20093-115">Properties</span></span>
| <span data-ttu-id="20093-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="20093-116">Property</span></span>     | <span data-ttu-id="20093-117">Тип</span><span class="sxs-lookup"><span data-stu-id="20093-117">Type</span></span>   |<span data-ttu-id="20093-118">Описание</span><span class="sxs-lookup"><span data-stu-id="20093-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20093-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="20093-119">classifyAs</span></span>|<span data-ttu-id="20093-120">string</span><span class="sxs-lookup"><span data-stu-id="20093-120">string</span></span>| <span data-ttu-id="20093-p101">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="20093-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="20093-123">id</span><span class="sxs-lookup"><span data-stu-id="20093-123">id</span></span>|<span data-ttu-id="20093-124">string</span><span class="sxs-lookup"><span data-stu-id="20093-124">string</span></span>| <span data-ttu-id="20093-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20093-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="20093-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="20093-127">senderEmailAddress</span></span>|[<span data-ttu-id="20093-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="20093-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="20093-129">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="20093-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20093-130">Связи</span><span class="sxs-lookup"><span data-stu-id="20093-130">Relationships</span></span>
<span data-ttu-id="20093-131">Нет</span><span class="sxs-lookup"><span data-stu-id="20093-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="20093-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20093-132">JSON representation</span></span>

<span data-ttu-id="20093-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20093-133">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassificationoverride.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
