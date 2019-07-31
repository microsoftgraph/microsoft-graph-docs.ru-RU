---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 256fea5b42f367fb9c6d08b2e871bebd825e3451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008329"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="1bc1c-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1bc1c-103">singleValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bc1c-104">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="1bc1c-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="1bc1c-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="1bc1c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1bc1c-106">Methods</span></span>

| <span data-ttu-id="1bc1c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1bc1c-107">Method</span></span>           | <span data-ttu-id="1bc1c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1bc1c-108">Return Type</span></span>    |<span data-ttu-id="1bc1c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc1c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1bc1c-110">Post</span><span class="sxs-lookup"><span data-stu-id="1bc1c-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="1bc1c-111">Поддерживаемый экземпляр ресурса: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md)или [Outlook Task](../resources/outlooktaskfolder.md), но не разноски группы [](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="1bc1c-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="1bc1c-112">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="1bc1c-113">Получение</span><span class="sxs-lookup"><span data-stu-id="1bc1c-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="1bc1c-114">Один или коллекция поддерживаемых экземпляров ресурсов ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md), [Outlook Task](../resources/outlooktaskfolder.md)или Group [POST](../resources/post.md)). или один такой экземпляр, дополненный объектом [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="1bc1c-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="1bc1c-115">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="1bc1c-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bc1c-116">Properties</span></span>
| <span data-ttu-id="1bc1c-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bc1c-117">Property</span></span>     | <span data-ttu-id="1bc1c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1bc1c-118">Type</span></span>   |<span data-ttu-id="1bc1c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc1c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1bc1c-120">id</span><span class="sxs-lookup"><span data-stu-id="1bc1c-120">id</span></span>|<span data-ttu-id="1bc1c-121">string</span><span class="sxs-lookup"><span data-stu-id="1bc1c-121">string</span></span>|<span data-ttu-id="1bc1c-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="1bc1c-124">значение</span><span class="sxs-lookup"><span data-stu-id="1bc1c-124">value</span></span>|<span data-ttu-id="1bc1c-125">string</span><span class="sxs-lookup"><span data-stu-id="1bc1c-125">string</span></span>|<span data-ttu-id="1bc1c-126">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bc1c-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="1bc1c-127">Relationships</span></span>
<span data-ttu-id="1bc1c-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1bc1c-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1bc1c-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bc1c-129">JSON representation</span></span>

<span data-ttu-id="1bc1c-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bc1c-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
