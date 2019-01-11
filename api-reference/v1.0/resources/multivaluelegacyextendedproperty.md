---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
ms.openlocfilehash: 87823559bad3e149ef3c4d4d6f21f43cf66c41fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827036"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="59d34-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="59d34-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="59d34-104">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="59d34-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="59d34-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="59d34-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="59d34-106">Методы</span><span class="sxs-lookup"><span data-stu-id="59d34-106">Methods</span></span>

| <span data-ttu-id="59d34-107">Метод</span><span class="sxs-lookup"><span data-stu-id="59d34-107">Method</span></span>           | <span data-ttu-id="59d34-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="59d34-108">Return Type</span></span>    |<span data-ttu-id="59d34-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59d34-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="59d34-110">Post</span><span class="sxs-lookup"><span data-stu-id="59d34-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="59d34-p101">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="59d34-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="59d34-113">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="59d34-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|<span data-ttu-id="59d34-114">[получение](../api/multivaluelegacyextendedproperty-get.md);</span><span class="sxs-lookup"><span data-stu-id="59d34-114">[Get](../api/multivaluelegacyextendedproperty-get.md)</span></span> |<span data-ttu-id="59d34-115">Экземпляр поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы), расширенный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="59d34-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="59d34-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="59d34-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="59d34-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="59d34-117">Properties</span></span>
| <span data-ttu-id="59d34-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="59d34-118">Property</span></span>     | <span data-ttu-id="59d34-119">Тип</span><span class="sxs-lookup"><span data-stu-id="59d34-119">Type</span></span>   |<span data-ttu-id="59d34-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59d34-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d34-121">id</span><span class="sxs-lookup"><span data-stu-id="59d34-121">id</span></span>|<span data-ttu-id="59d34-122">строка</span><span class="sxs-lookup"><span data-stu-id="59d34-122">string</span></span>|<span data-ttu-id="59d34-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59d34-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="59d34-125">value</span><span class="sxs-lookup"><span data-stu-id="59d34-125">value</span></span>|<span data-ttu-id="59d34-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="59d34-126">string collection</span></span>|<span data-ttu-id="59d34-127">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="59d34-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59d34-128">Связи</span><span class="sxs-lookup"><span data-stu-id="59d34-128">Relationships</span></span>
<span data-ttu-id="59d34-129">Нет</span><span class="sxs-lookup"><span data-stu-id="59d34-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="59d34-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59d34-130">JSON representation</span></span>

<span data-ttu-id="59d34-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59d34-131">Here is a JSON representation of the resource.</span></span>

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
