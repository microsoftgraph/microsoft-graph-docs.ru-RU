---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b13fa96cbfbb0e0eb6fefc97ef76e2278ca26640
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811240"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="b2975-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="b2975-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="b2975-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2975-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2975-105">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="b2975-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="b2975-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b2975-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="b2975-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b2975-107">Methods</span></span>

| <span data-ttu-id="b2975-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b2975-108">Method</span></span>           | <span data-ttu-id="b2975-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2975-109">Return Type</span></span>    |<span data-ttu-id="b2975-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2975-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2975-111">Post</span><span class="sxs-lookup"><span data-stu-id="b2975-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="b2975-112">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md), но не [post](../resources/post.md) группы.</span><span class="sxs-lookup"><span data-stu-id="b2975-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="b2975-113">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="b2975-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="b2975-114">Получение</span><span class="sxs-lookup"><span data-stu-id="b2975-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="b2975-115">Один или несколько экземпляров поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы) либо один такой экземпляр, расширенный объектом [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="b2975-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="b2975-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b2975-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2975-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2975-117">Properties</span></span>
| <span data-ttu-id="b2975-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2975-118">Property</span></span>     | <span data-ttu-id="b2975-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b2975-119">Type</span></span>   |<span data-ttu-id="b2975-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b2975-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2975-121">id</span><span class="sxs-lookup"><span data-stu-id="b2975-121">id</span></span>|<span data-ttu-id="b2975-122">string</span><span class="sxs-lookup"><span data-stu-id="b2975-122">string</span></span>|<span data-ttu-id="b2975-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2975-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="b2975-125">значение</span><span class="sxs-lookup"><span data-stu-id="b2975-125">value</span></span>|<span data-ttu-id="b2975-126">string</span><span class="sxs-lookup"><span data-stu-id="b2975-126">string</span></span>|<span data-ttu-id="b2975-127">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="b2975-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2975-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2975-128">Relationships</span></span>
<span data-ttu-id="b2975-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b2975-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b2975-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2975-130">JSON representation</span></span>

<span data-ttu-id="b2975-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2975-131">Here is a JSON representation of the resource.</span></span>

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
