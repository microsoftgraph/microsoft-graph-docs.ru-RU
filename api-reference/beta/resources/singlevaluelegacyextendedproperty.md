---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 1733aa15f6989aaef1bb2c80d469f47d6ad86e2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136545"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="337c5-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="337c5-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="337c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="337c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="337c5-105">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="337c5-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="337c5-106">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="337c5-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="337c5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="337c5-107">Methods</span></span>

| <span data-ttu-id="337c5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="337c5-108">Method</span></span>           | <span data-ttu-id="337c5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="337c5-109">Return Type</span></span>    |<span data-ttu-id="337c5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="337c5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="337c5-111">Post</span><span class="sxs-lookup"><span data-stu-id="337c5-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="337c5-112">Поддерживаемый экземпляр ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or Outlook [task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="337c5-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="337c5-113">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="337c5-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="337c5-114">Получение</span><span class="sxs-lookup"><span data-stu-id="337c5-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="337c5-115">Один или коллекция поддерживаемых экземпляров ресурса[(сообщение,](../resources/message.md) [mailFolder,](../resources/mailfolder.md) [событие,](../resources/event.md)календарь, [](../resources/calendar.md) [контакт](../resources/contact.md), [contactFolder,](../resources/contactfolder.md)задача [Outlook,](../resources/outlooktask.md)папка задач [Outlook](../resources/outlooktaskfolder.md)или публикация [группы)](../resources/post.md)или один такой экземпляр, расширенный с помощью объекта [singleValueLegacyExtendedProperty.](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="337c5-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="337c5-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="337c5-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="337c5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="337c5-117">Properties</span></span>
| <span data-ttu-id="337c5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="337c5-118">Property</span></span>     | <span data-ttu-id="337c5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="337c5-119">Type</span></span>   |<span data-ttu-id="337c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="337c5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="337c5-121">id</span><span class="sxs-lookup"><span data-stu-id="337c5-121">id</span></span>|<span data-ttu-id="337c5-122">string</span><span class="sxs-lookup"><span data-stu-id="337c5-122">string</span></span>|<span data-ttu-id="337c5-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="337c5-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="337c5-125">значение</span><span class="sxs-lookup"><span data-stu-id="337c5-125">value</span></span>|<span data-ttu-id="337c5-126">string</span><span class="sxs-lookup"><span data-stu-id="337c5-126">string</span></span>|<span data-ttu-id="337c5-127">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="337c5-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="337c5-128">Связи</span><span class="sxs-lookup"><span data-stu-id="337c5-128">Relationships</span></span>
<span data-ttu-id="337c5-129">Нет</span><span class="sxs-lookup"><span data-stu-id="337c5-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="337c5-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="337c5-130">JSON representation</span></span>

<span data-ttu-id="337c5-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="337c5-131">Here is a JSON representation of the resource.</span></span>

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


