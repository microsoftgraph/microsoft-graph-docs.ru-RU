---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
ms.openlocfilehash: 9aa94465ca1a0fb30c4461b99336040c72e2c5c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025661"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="a2dc0-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a2dc0-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="a2dc0-104">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="a2dc0-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="a2dc0-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a2dc0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a2dc0-106">Methods</span></span>

| <span data-ttu-id="a2dc0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a2dc0-107">Method</span></span>           | <span data-ttu-id="a2dc0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a2dc0-108">Return Type</span></span>    |<span data-ttu-id="a2dc0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2dc0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2dc0-110">Post</span><span class="sxs-lookup"><span data-stu-id="a2dc0-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="a2dc0-p101">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="a2dc0-113">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="a2dc0-114">Get</span><span class="sxs-lookup"><span data-stu-id="a2dc0-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="a2dc0-115">Экземпляр поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы), расширенный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="a2dc0-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="a2dc0-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2dc0-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2dc0-117">Properties</span></span>
| <span data-ttu-id="a2dc0-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2dc0-118">Property</span></span>     | <span data-ttu-id="a2dc0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a2dc0-119">Type</span></span>   |<span data-ttu-id="a2dc0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a2dc0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2dc0-121">id</span><span class="sxs-lookup"><span data-stu-id="a2dc0-121">id</span></span>|<span data-ttu-id="a2dc0-122">строка</span><span class="sxs-lookup"><span data-stu-id="a2dc0-122">string</span></span>|<span data-ttu-id="a2dc0-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="a2dc0-125">value</span><span class="sxs-lookup"><span data-stu-id="a2dc0-125">value</span></span>|<span data-ttu-id="a2dc0-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a2dc0-126">string collection</span></span>|<span data-ttu-id="a2dc0-127">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2dc0-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a2dc0-128">Relationships</span></span>
<span data-ttu-id="a2dc0-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a2dc0-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a2dc0-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2dc0-130">JSON representation</span></span>

<span data-ttu-id="a2dc0-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2dc0-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->