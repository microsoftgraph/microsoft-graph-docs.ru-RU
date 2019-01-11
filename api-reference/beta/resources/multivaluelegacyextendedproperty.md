---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
ms.openlocfilehash: e98963eea5e1e996170f6330b9b4b333a72ad159
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839454"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="8fb3f-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8fb3f-103">multiValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="8fb3f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fb3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fb3f-106">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-106">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="8fb3f-107">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="8fb3f-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="8fb3f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8fb3f-108">Methods</span></span>

| <span data-ttu-id="8fb3f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8fb3f-109">Method</span></span>           | <span data-ttu-id="8fb3f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8fb3f-110">Return Type</span></span>    |<span data-ttu-id="8fb3f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8fb3f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fb3f-112">Post</span><span class="sxs-lookup"><span data-stu-id="8fb3f-112">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="8fb3f-113">Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8fb3f-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="8fb3f-114">Обратите внимание, что, группа [записи](../resources/post.md) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-114">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="8fb3f-115">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-115">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|<span data-ttu-id="8fb3f-116">[получение](../api/multivaluelegacyextendedproperty-get.md);</span><span class="sxs-lookup"><span data-stu-id="8fb3f-116">[Get](../api/multivaluelegacyextendedproperty-get.md)</span></span> |<span data-ttu-id="8fb3f-117">Экземпляр поддерживаемые ресурсов ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), включающим [ multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-117">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="8fb3f-118">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-118">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fb3f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fb3f-119">Properties</span></span>
| <span data-ttu-id="8fb3f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fb3f-120">Property</span></span>     | <span data-ttu-id="8fb3f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8fb3f-121">Type</span></span>   |<span data-ttu-id="8fb3f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8fb3f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fb3f-123">id</span><span class="sxs-lookup"><span data-stu-id="8fb3f-123">id</span></span>|<span data-ttu-id="8fb3f-124">строка</span><span class="sxs-lookup"><span data-stu-id="8fb3f-124">string</span></span>|<span data-ttu-id="8fb3f-p103">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-p103">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="8fb3f-127">value</span><span class="sxs-lookup"><span data-stu-id="8fb3f-127">value</span></span>|<span data-ttu-id="8fb3f-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8fb3f-128">string collection</span></span>|<span data-ttu-id="8fb3f-129">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-129">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fb3f-130">Связи</span><span class="sxs-lookup"><span data-stu-id="8fb3f-130">Relationships</span></span>
<span data-ttu-id="8fb3f-131">Нет</span><span class="sxs-lookup"><span data-stu-id="8fb3f-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8fb3f-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fb3f-132">JSON representation</span></span>

<span data-ttu-id="8fb3f-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fb3f-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
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
