---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: bf082da6c628c5b4f4ef969ced3f4f50ebf2f65f
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849165"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="de528-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="de528-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="de528-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="de528-105">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="de528-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="de528-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="de528-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="de528-107">Методы</span><span class="sxs-lookup"><span data-stu-id="de528-107">Methods</span></span>

| <span data-ttu-id="de528-108">Метод</span><span class="sxs-lookup"><span data-stu-id="de528-108">Method</span></span>           | <span data-ttu-id="de528-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="de528-109">Return Type</span></span>    |<span data-ttu-id="de528-110">Описание</span><span class="sxs-lookup"><span data-stu-id="de528-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de528-111">Post</span><span class="sxs-lookup"><span data-stu-id="de528-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="de528-112">Поддерживаемый экземпляр ресурса: [message,](../resources/message.md) [mailFolder,](../resources/mailfolder.md) [event,](../resources/event.md) [calendar,](../resources/calendar.md) [contact,](../resources/contact.md) [contactFolder,](../resources/contactfolder.md) [Outlook task](../resources/outlooktask.md)или [папка задач Outlook.](../resources/outlooktaskfolder.md)</span><span class="sxs-lookup"><span data-stu-id="de528-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="de528-113">Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="de528-113">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="de528-114">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="de528-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="de528-115">Получение</span><span class="sxs-lookup"><span data-stu-id="de528-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="de528-116">Поддерживаемый экземпляр ресурса[(message,](../resources/message.md) [mailFolder,](../resources/mailfolder.md) [event,](../resources/event.md) [calendar,](../resources/calendar.md) [contactFolder,](../resources/contact.md) [Outlook task,](../resources/outlooktask.md) [папка задач Outlook](../resources/outlooktaskfolder.md)или запись в [группе),](../resources/post.md)дополненный [объектом multiValueLegacyExtendedProperty.](multivaluelegacyextendedproperty.md) [contactFolder](../resources/contactfolder.md)</span><span class="sxs-lookup"><span data-stu-id="de528-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="de528-117">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="de528-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="de528-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="de528-118">Properties</span></span>
| <span data-ttu-id="de528-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="de528-119">Property</span></span>     | <span data-ttu-id="de528-120">Тип</span><span class="sxs-lookup"><span data-stu-id="de528-120">Type</span></span>   |<span data-ttu-id="de528-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de528-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de528-122">id</span><span class="sxs-lookup"><span data-stu-id="de528-122">id</span></span>|<span data-ttu-id="de528-123">строка</span><span class="sxs-lookup"><span data-stu-id="de528-123">string</span></span>|<span data-ttu-id="de528-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="de528-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="de528-126">значение</span><span class="sxs-lookup"><span data-stu-id="de528-126">value</span></span>|<span data-ttu-id="de528-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="de528-127">string collection</span></span>|<span data-ttu-id="de528-128">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="de528-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de528-129">Связи</span><span class="sxs-lookup"><span data-stu-id="de528-129">Relationships</span></span>
<span data-ttu-id="de528-130">Нет</span><span class="sxs-lookup"><span data-stu-id="de528-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="de528-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de528-131">JSON representation</span></span>

<span data-ttu-id="de528-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de528-132">Here is a JSON representation of the resource.</span></span>

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
