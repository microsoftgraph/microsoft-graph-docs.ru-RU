---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользователя переопределения для способ входящих сообщений от определенного отправителя всегда должны следует рассматривать как
ms.openlocfilehash: 63c753b7af21907717d7d9706d0606726d5670f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075857"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="232a8-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="232a8-103">inferenceClassificationOverride resource type</span></span>

> <span data-ttu-id="232a8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="232a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="232a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="232a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="232a8-106">Представляет пользователя переопределения для способ входящих сообщений от определенного отправителя всегда следует рассматривать как и [Фокус папки «Входящие»](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="232a8-106">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="232a8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="232a8-107">Methods</span></span>

| <span data-ttu-id="232a8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="232a8-108">Method</span></span>           | <span data-ttu-id="232a8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="232a8-109">Return Type</span></span>    |<span data-ttu-id="232a8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="232a8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="232a8-111">Update</span><span class="sxs-lookup"><span data-stu-id="232a8-111">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="232a8-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="232a8-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="232a8-113">Изменение поля **ClassifyAs** переопределения, указанный.</span><span class="sxs-lookup"><span data-stu-id="232a8-113">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="232a8-114">Delete</span><span class="sxs-lookup"><span data-stu-id="232a8-114">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="232a8-115">Нет</span><span class="sxs-lookup"><span data-stu-id="232a8-115">None</span></span> |<span data-ttu-id="232a8-116">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="232a8-116">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="232a8-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="232a8-117">Properties</span></span>
| <span data-ttu-id="232a8-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="232a8-118">Property</span></span>     | <span data-ttu-id="232a8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="232a8-119">Type</span></span>   |<span data-ttu-id="232a8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="232a8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="232a8-121">classifyAs</span><span class="sxs-lookup"><span data-stu-id="232a8-121">classifyAs</span></span>|<span data-ttu-id="232a8-122">string</span><span class="sxs-lookup"><span data-stu-id="232a8-122">string</span></span>| <span data-ttu-id="232a8-p102">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="232a8-p102">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="232a8-125">id</span><span class="sxs-lookup"><span data-stu-id="232a8-125">id</span></span>|<span data-ttu-id="232a8-126">строка</span><span class="sxs-lookup"><span data-stu-id="232a8-126">string</span></span>| <span data-ttu-id="232a8-p103">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232a8-p103">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="232a8-129">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="232a8-129">senderEmailAddress</span></span>|[<span data-ttu-id="232a8-130">emailAddress</span><span class="sxs-lookup"><span data-stu-id="232a8-130">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="232a8-131">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="232a8-131">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="232a8-132">Связи</span><span class="sxs-lookup"><span data-stu-id="232a8-132">Relationships</span></span>
<span data-ttu-id="232a8-133">Нет</span><span class="sxs-lookup"><span data-stu-id="232a8-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="232a8-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="232a8-134">JSON representation</span></span>

<span data-ttu-id="232a8-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="232a8-135">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->