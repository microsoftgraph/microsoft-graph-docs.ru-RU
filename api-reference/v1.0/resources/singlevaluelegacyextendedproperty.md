---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
ms.openlocfilehash: 82a2ca848ba22381366016617c3fa6529ce4ee54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025435"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="c2c3d-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="c2c3d-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="c2c3d-104">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="c2c3d-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c2c3d-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="c2c3d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c2c3d-106">Methods</span></span>

| <span data-ttu-id="c2c3d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c2c3d-107">Method</span></span>           | <span data-ttu-id="c2c3d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2c3d-108">Return Type</span></span>    |<span data-ttu-id="c2c3d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c3d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2c3d-110">Создание</span><span class="sxs-lookup"><span data-stu-id="c2c3d-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="c2c3d-111">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md), но не [post](../resources/post.md) группы.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="c2c3d-112">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="c2c3d-113">Получение</span><span class="sxs-lookup"><span data-stu-id="c2c3d-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="c2c3d-114">Один или несколько экземпляров поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы) либо один такой экземпляр, расширенный объектом [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="c2c3d-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="c2c3d-115">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2c3d-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2c3d-116">Properties</span></span>
| <span data-ttu-id="c2c3d-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2c3d-117">Property</span></span>     | <span data-ttu-id="c2c3d-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c2c3d-118">Type</span></span>   |<span data-ttu-id="c2c3d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c3d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2c3d-120">id</span><span class="sxs-lookup"><span data-stu-id="c2c3d-120">id</span></span>|<span data-ttu-id="c2c3d-121">строка</span><span class="sxs-lookup"><span data-stu-id="c2c3d-121">string</span></span>|<span data-ttu-id="c2c3d-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="c2c3d-124">value</span><span class="sxs-lookup"><span data-stu-id="c2c3d-124">value</span></span>|<span data-ttu-id="c2c3d-125">строка</span><span class="sxs-lookup"><span data-stu-id="c2c3d-125">string</span></span>|<span data-ttu-id="c2c3d-126">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2c3d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="c2c3d-127">Relationships</span></span>
<span data-ttu-id="c2c3d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="c2c3d-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c2c3d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2c3d-129">JSON representation</span></span>

<span data-ttu-id="c2c3d-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2c3d-130">Here is a JSON representation of the resource.</span></span>

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