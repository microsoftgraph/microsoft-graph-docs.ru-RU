---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2ace395b336a0950c814a4eb65103de440f59305
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966708"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="bc194-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="bc194-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc194-104">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="bc194-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="bc194-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="bc194-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="bc194-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bc194-106">Methods</span></span>

| <span data-ttu-id="bc194-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bc194-107">Method</span></span>           | <span data-ttu-id="bc194-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc194-108">Return Type</span></span>    |<span data-ttu-id="bc194-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bc194-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc194-110">Post</span><span class="sxs-lookup"><span data-stu-id="bc194-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="bc194-111">Поддерживаемый экземпляр ресурса: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)или [Outlook Task](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="bc194-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="bc194-112">Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bc194-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="bc194-113">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="bc194-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="bc194-114">Получение</span><span class="sxs-lookup"><span data-stu-id="bc194-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="bc194-115">Поддерживаемый экземпляр ресурса ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md), [Outlook Task Folder](../resources/outlooktaskfolder.md)или POST Group [POST](../resources/post.md)), дополненный [ Объект multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="bc194-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="bc194-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="bc194-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc194-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc194-117">Properties</span></span>
| <span data-ttu-id="bc194-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc194-118">Property</span></span>     | <span data-ttu-id="bc194-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bc194-119">Type</span></span>   |<span data-ttu-id="bc194-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc194-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc194-121">id</span><span class="sxs-lookup"><span data-stu-id="bc194-121">id</span></span>|<span data-ttu-id="bc194-122">string</span><span class="sxs-lookup"><span data-stu-id="bc194-122">string</span></span>|<span data-ttu-id="bc194-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc194-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="bc194-125">значение</span><span class="sxs-lookup"><span data-stu-id="bc194-125">value</span></span>|<span data-ttu-id="bc194-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bc194-126">string collection</span></span>|<span data-ttu-id="bc194-127">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="bc194-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc194-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc194-128">Relationships</span></span>
<span data-ttu-id="bc194-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bc194-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bc194-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc194-130">JSON representation</span></span>

<span data-ttu-id="bc194-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc194-131">Here is a JSON representation of the resource.</span></span>

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
