---
title: Тип ресурса inferenceClassificationOverride
description: Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c3d792d7f8687da1b65e969f1b42d61612532a22
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029220"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="cf6a4-103">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="cf6a4-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="cf6a4-104">Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="cf6a4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="cf6a4-105">Methods</span></span>

| <span data-ttu-id="cf6a4-106">Метод</span><span class="sxs-lookup"><span data-stu-id="cf6a4-106">Method</span></span>           | <span data-ttu-id="cf6a4-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf6a4-107">Return Type</span></span>    |<span data-ttu-id="cf6a4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cf6a4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf6a4-109">Обновление</span><span class="sxs-lookup"><span data-stu-id="cf6a4-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="cf6a4-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="cf6a4-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="cf6a4-111">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="cf6a4-112">Удаление</span><span class="sxs-lookup"><span data-stu-id="cf6a4-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="cf6a4-113">Нет</span><span class="sxs-lookup"><span data-stu-id="cf6a4-113">None</span></span> |<span data-ttu-id="cf6a4-114">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf6a4-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf6a4-115">Properties</span></span>
| <span data-ttu-id="cf6a4-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf6a4-116">Property</span></span>     | <span data-ttu-id="cf6a4-117">Тип</span><span class="sxs-lookup"><span data-stu-id="cf6a4-117">Type</span></span>   |<span data-ttu-id="cf6a4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="cf6a4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf6a4-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="cf6a4-119">classifyAs</span></span>|<span data-ttu-id="cf6a4-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="cf6a4-120">inferenceClassificationType</span></span>| <span data-ttu-id="cf6a4-121">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="cf6a4-122">Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="cf6a4-123">id</span><span class="sxs-lookup"><span data-stu-id="cf6a4-123">id</span></span>|<span data-ttu-id="cf6a4-124">string</span><span class="sxs-lookup"><span data-stu-id="cf6a4-124">string</span></span>| <span data-ttu-id="cf6a4-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="cf6a4-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="cf6a4-127">senderEmailAddress</span></span>|[<span data-ttu-id="cf6a4-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cf6a4-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="cf6a4-129">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf6a4-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="cf6a4-130">Relationships</span></span>
<span data-ttu-id="cf6a4-131">Нет</span><span class="sxs-lookup"><span data-stu-id="cf6a4-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cf6a4-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf6a4-132">JSON representation</span></span>

<span data-ttu-id="cf6a4-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf6a4-133">Here is a JSON representation of the resource.</span></span>

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
