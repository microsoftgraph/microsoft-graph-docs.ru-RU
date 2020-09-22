---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 4ccfdc6fd703673cdd71284cf3ad367f94efdc5e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021282"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="26da8-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="26da8-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="26da8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26da8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="26da8-105">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="26da8-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="26da8-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="26da8-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="26da8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="26da8-107">Methods</span></span>

| <span data-ttu-id="26da8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="26da8-108">Method</span></span>           | <span data-ttu-id="26da8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="26da8-109">Return Type</span></span>    |<span data-ttu-id="26da8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26da8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26da8-111">Post</span><span class="sxs-lookup"><span data-stu-id="26da8-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="26da8-112">Поддерживаемый экземпляр ресурса: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)или [Outlook Task](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="26da8-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="26da8-113">Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="26da8-113">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="26da8-114">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="26da8-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="26da8-115">Получение</span><span class="sxs-lookup"><span data-stu-id="26da8-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="26da8-116">Поддерживаемый экземпляр ресурса ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md), [Outlook Task Folder](../resources/outlooktaskfolder.md)или POST Group [POST](../resources/post.md)), дополненный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="26da8-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="26da8-117">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="26da8-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="26da8-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="26da8-118">Properties</span></span>
| <span data-ttu-id="26da8-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="26da8-119">Property</span></span>     | <span data-ttu-id="26da8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="26da8-120">Type</span></span>   |<span data-ttu-id="26da8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="26da8-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26da8-122">id</span><span class="sxs-lookup"><span data-stu-id="26da8-122">id</span></span>|<span data-ttu-id="26da8-123">string</span><span class="sxs-lookup"><span data-stu-id="26da8-123">string</span></span>|<span data-ttu-id="26da8-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26da8-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="26da8-126">значение</span><span class="sxs-lookup"><span data-stu-id="26da8-126">value</span></span>|<span data-ttu-id="26da8-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="26da8-127">string collection</span></span>|<span data-ttu-id="26da8-128">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="26da8-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26da8-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="26da8-129">Relationships</span></span>
<span data-ttu-id="26da8-130">Нет</span><span class="sxs-lookup"><span data-stu-id="26da8-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="26da8-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26da8-131">JSON representation</span></span>

<span data-ttu-id="26da8-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26da8-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


