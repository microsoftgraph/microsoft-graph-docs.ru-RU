---
title: Тип ресурса inferenceClassificationOverride
description: Представляет переопределение пользователя, определяющее, как должны классифицироваться входящие сообщения от определенного отправителя
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548735"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="f7562-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="f7562-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7562-104">Представляет переопределение пользователя, которое всегда должно классифицироваться как входящие сообщения от определенного отправителя, как в [папке "отсортированНые"](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="f7562-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="f7562-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f7562-105">Methods</span></span>

| <span data-ttu-id="f7562-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f7562-106">Method</span></span>           | <span data-ttu-id="f7562-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7562-107">Return Type</span></span>    |<span data-ttu-id="f7562-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f7562-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7562-109">Обновление</span><span class="sxs-lookup"><span data-stu-id="f7562-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="f7562-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="f7562-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="f7562-111">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="f7562-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="f7562-112">Удаление</span><span class="sxs-lookup"><span data-stu-id="f7562-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="f7562-113">Нет</span><span class="sxs-lookup"><span data-stu-id="f7562-113">None</span></span> |<span data-ttu-id="f7562-114">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="f7562-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7562-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7562-115">Properties</span></span>
| <span data-ttu-id="f7562-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7562-116">Property</span></span>     | <span data-ttu-id="f7562-117">Тип</span><span class="sxs-lookup"><span data-stu-id="f7562-117">Type</span></span>   |<span data-ttu-id="f7562-118">Описание</span><span class="sxs-lookup"><span data-stu-id="f7562-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7562-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="f7562-119">classifyAs</span></span>|<span data-ttu-id="f7562-120">string</span><span class="sxs-lookup"><span data-stu-id="f7562-120">string</span></span>| <span data-ttu-id="f7562-p101">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="f7562-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="f7562-123">id</span><span class="sxs-lookup"><span data-stu-id="f7562-123">id</span></span>|<span data-ttu-id="f7562-124">string</span><span class="sxs-lookup"><span data-stu-id="f7562-124">string</span></span>| <span data-ttu-id="f7562-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f7562-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="f7562-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f7562-127">senderEmailAddress</span></span>|[<span data-ttu-id="f7562-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="f7562-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="f7562-129">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="f7562-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7562-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7562-130">Relationships</span></span>
<span data-ttu-id="f7562-131">Нет</span><span class="sxs-lookup"><span data-stu-id="f7562-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f7562-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f7562-132">JSON representation</span></span>

<span data-ttu-id="f7562-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7562-133">Here is a JSON representation of the resource.</span></span>

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
