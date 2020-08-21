---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 41857d57010265d7942e0d1694191ee5acf3c4d1
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849746"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="0629c-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="0629c-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="0629c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0629c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="0629c-105">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="0629c-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="0629c-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="0629c-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="0629c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0629c-107">Methods</span></span>

| <span data-ttu-id="0629c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0629c-108">Method</span></span>           | <span data-ttu-id="0629c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0629c-109">Return Type</span></span>    |<span data-ttu-id="0629c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0629c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0629c-111">Post</span><span class="sxs-lookup"><span data-stu-id="0629c-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="0629c-112">Поддерживаемый экземпляр ресурса: [message,](../resources/message.md) [mailFolder,](../resources/mailfolder.md) [event,](../resources/event.md) [calendar,](../resources/calendar.md) [contact,](../resources/contact.md) [contactFolder,](../resources/contactfolder.md) [Outlook task](../resources/outlooktask.md)или [Outlook folder,](../resources/outlooktaskfolder.md)но не [записи в группе.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="0629c-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="0629c-113">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="0629c-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="0629c-114">Получение</span><span class="sxs-lookup"><span data-stu-id="0629c-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="0629c-115">Один или коллекция поддерживаемых экземпляров ресурса[(message,](../resources/message.md) [mailFolder,](../resources/mailfolder.md) [event,](../resources/event.md) [calendar,](../resources/calendar.md) [contactFolder,](../resources/contactfolder.md) [Outlook task,](../resources/outlooktask.md) [папка задач Outlook,](../resources/outlooktaskfolder.md) [запись](../resources/post.md)группы), либо один такой экземпляр, дополненный [объектом singleValueLegacyExtendedProperty.](singlevaluelegacyextendedproperty.md) [contact](../resources/contact.md)</span><span class="sxs-lookup"><span data-stu-id="0629c-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="0629c-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0629c-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="0629c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="0629c-117">Properties</span></span>
| <span data-ttu-id="0629c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="0629c-118">Property</span></span>     | <span data-ttu-id="0629c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0629c-119">Type</span></span>   |<span data-ttu-id="0629c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0629c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0629c-121">id</span><span class="sxs-lookup"><span data-stu-id="0629c-121">id</span></span>|<span data-ttu-id="0629c-122">строка</span><span class="sxs-lookup"><span data-stu-id="0629c-122">string</span></span>|<span data-ttu-id="0629c-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0629c-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="0629c-125">значение</span><span class="sxs-lookup"><span data-stu-id="0629c-125">value</span></span>|<span data-ttu-id="0629c-126">string</span><span class="sxs-lookup"><span data-stu-id="0629c-126">string</span></span>|<span data-ttu-id="0629c-127">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="0629c-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0629c-128">Связи</span><span class="sxs-lookup"><span data-stu-id="0629c-128">Relationships</span></span>
<span data-ttu-id="0629c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0629c-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0629c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0629c-130">JSON representation</span></span>

<span data-ttu-id="0629c-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0629c-131">Here is a JSON representation of the resource.</span></span>

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
