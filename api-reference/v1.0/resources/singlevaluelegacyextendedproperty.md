---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dd1f191488ed314d9129779c83571580ebc7c823
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086398"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="8bf2f-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8bf2f-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="8bf2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bf2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8bf2f-105">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="8bf2f-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8bf2f-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="8bf2f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8bf2f-107">Methods</span></span>

| <span data-ttu-id="8bf2f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8bf2f-108">Method</span></span>           | <span data-ttu-id="8bf2f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bf2f-109">Return Type</span></span>    |<span data-ttu-id="8bf2f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf2f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bf2f-111">Post</span><span class="sxs-lookup"><span data-stu-id="8bf2f-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="8bf2f-112">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md), но не [post](../resources/post.md) группы.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="8bf2f-113">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="8bf2f-114">Получение</span><span class="sxs-lookup"><span data-stu-id="8bf2f-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="8bf2f-115">Один или несколько экземпляров поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы) либо один такой экземпляр, расширенный объектом [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="8bf2f-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="8bf2f-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bf2f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bf2f-117">Properties</span></span>
| <span data-ttu-id="8bf2f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bf2f-118">Property</span></span>     | <span data-ttu-id="8bf2f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8bf2f-119">Type</span></span>   |<span data-ttu-id="8bf2f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8bf2f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bf2f-121">id</span><span class="sxs-lookup"><span data-stu-id="8bf2f-121">id</span></span>|<span data-ttu-id="8bf2f-122">string</span><span class="sxs-lookup"><span data-stu-id="8bf2f-122">string</span></span>|<span data-ttu-id="8bf2f-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="8bf2f-125">значение</span><span class="sxs-lookup"><span data-stu-id="8bf2f-125">value</span></span>|<span data-ttu-id="8bf2f-126">string</span><span class="sxs-lookup"><span data-stu-id="8bf2f-126">string</span></span>|<span data-ttu-id="8bf2f-127">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bf2f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="8bf2f-128">Relationships</span></span>
<span data-ttu-id="8bf2f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="8bf2f-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8bf2f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bf2f-130">JSON representation</span></span>

<span data-ttu-id="8bf2f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bf2f-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

