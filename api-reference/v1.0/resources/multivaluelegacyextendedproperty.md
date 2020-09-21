---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67fdf6660ddacdd96106637961e580947cd4c55f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967368"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="52f7a-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="52f7a-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="52f7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52f7a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52f7a-105">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="52f7a-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="52f7a-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="52f7a-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="52f7a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="52f7a-107">Methods</span></span>

| <span data-ttu-id="52f7a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="52f7a-108">Method</span></span>           | <span data-ttu-id="52f7a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52f7a-109">Return Type</span></span>    |<span data-ttu-id="52f7a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="52f7a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52f7a-111">Post</span><span class="sxs-lookup"><span data-stu-id="52f7a-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="52f7a-p101">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="52f7a-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="52f7a-114">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="52f7a-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="52f7a-115">Получение</span><span class="sxs-lookup"><span data-stu-id="52f7a-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="52f7a-116">Экземпляр поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы), расширенный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="52f7a-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="52f7a-117">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="52f7a-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="52f7a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="52f7a-118">Properties</span></span>
| <span data-ttu-id="52f7a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="52f7a-119">Property</span></span>     | <span data-ttu-id="52f7a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="52f7a-120">Type</span></span>   |<span data-ttu-id="52f7a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="52f7a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52f7a-122">id</span><span class="sxs-lookup"><span data-stu-id="52f7a-122">id</span></span>|<span data-ttu-id="52f7a-123">string</span><span class="sxs-lookup"><span data-stu-id="52f7a-123">string</span></span>|<span data-ttu-id="52f7a-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52f7a-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="52f7a-126">значение</span><span class="sxs-lookup"><span data-stu-id="52f7a-126">value</span></span>|<span data-ttu-id="52f7a-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="52f7a-127">string collection</span></span>|<span data-ttu-id="52f7a-128">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="52f7a-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52f7a-129">Связи</span><span class="sxs-lookup"><span data-stu-id="52f7a-129">Relationships</span></span>
<span data-ttu-id="52f7a-130">Нет</span><span class="sxs-lookup"><span data-stu-id="52f7a-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="52f7a-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52f7a-131">JSON representation</span></span>

<span data-ttu-id="52f7a-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52f7a-132">Here is a JSON representation of the resource.</span></span>

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

