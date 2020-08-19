---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c0a92607eaadc0146af8ef10185543826443d693
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811926"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="cd31e-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="cd31e-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="cd31e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd31e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd31e-105">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="cd31e-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="cd31e-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="cd31e-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="cd31e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cd31e-107">Methods</span></span>

| <span data-ttu-id="cd31e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cd31e-108">Method</span></span>           | <span data-ttu-id="cd31e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd31e-109">Return Type</span></span>    |<span data-ttu-id="cd31e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd31e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd31e-111">Post</span><span class="sxs-lookup"><span data-stu-id="cd31e-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="cd31e-p101">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cd31e-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="cd31e-114">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="cd31e-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="cd31e-115">Получение</span><span class="sxs-lookup"><span data-stu-id="cd31e-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="cd31e-116">Экземпляр поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы), расширенный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="cd31e-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="cd31e-117">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="cd31e-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd31e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd31e-118">Properties</span></span>
| <span data-ttu-id="cd31e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd31e-119">Property</span></span>     | <span data-ttu-id="cd31e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="cd31e-120">Type</span></span>   |<span data-ttu-id="cd31e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cd31e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd31e-122">id</span><span class="sxs-lookup"><span data-stu-id="cd31e-122">id</span></span>|<span data-ttu-id="cd31e-123">string</span><span class="sxs-lookup"><span data-stu-id="cd31e-123">string</span></span>|<span data-ttu-id="cd31e-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd31e-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="cd31e-126">значение</span><span class="sxs-lookup"><span data-stu-id="cd31e-126">value</span></span>|<span data-ttu-id="cd31e-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cd31e-127">string collection</span></span>|<span data-ttu-id="cd31e-128">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="cd31e-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd31e-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="cd31e-129">Relationships</span></span>
<span data-ttu-id="cd31e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="cd31e-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cd31e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd31e-131">JSON representation</span></span>

<span data-ttu-id="cd31e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd31e-132">Here is a JSON representation of the resource.</span></span>

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
