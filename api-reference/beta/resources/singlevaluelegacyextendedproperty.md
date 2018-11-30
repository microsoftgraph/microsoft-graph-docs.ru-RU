---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
ms.openlocfilehash: 1b9eeaa05ee15aab30c1761cd35f70f586dffb24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081657"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="272b4-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="272b4-103">singleValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="272b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="272b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="272b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="272b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="272b4-106">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="272b4-106">An extended property that contains a single value.</span></span> 

<span data-ttu-id="272b4-107">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="272b4-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="272b4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="272b4-108">Methods</span></span>

| <span data-ttu-id="272b4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="272b4-109">Method</span></span>           | <span data-ttu-id="272b4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="272b4-110">Return Type</span></span>    |<span data-ttu-id="272b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="272b4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="272b4-112">Post</span><span class="sxs-lookup"><span data-stu-id="272b4-112">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="272b4-113">Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md), но не группа [учета](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="272b4-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="272b4-114">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="272b4-114">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="272b4-115">Получение</span><span class="sxs-lookup"><span data-stu-id="272b4-115">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="272b4-116">Один или коллекцию поддерживаемых ресурсов экземпляра ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), или один экземпляр, включающим объект [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="272b4-116">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="272b4-117">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="272b4-117">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="272b4-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="272b4-118">Properties</span></span>
| <span data-ttu-id="272b4-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="272b4-119">Property</span></span>     | <span data-ttu-id="272b4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="272b4-120">Type</span></span>   |<span data-ttu-id="272b4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="272b4-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="272b4-122">id</span><span class="sxs-lookup"><span data-stu-id="272b4-122">id</span></span>|<span data-ttu-id="272b4-123">string</span><span class="sxs-lookup"><span data-stu-id="272b4-123">string</span></span>|<span data-ttu-id="272b4-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="272b4-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="272b4-126">value</span><span class="sxs-lookup"><span data-stu-id="272b4-126">value</span></span>|<span data-ttu-id="272b4-127">строка</span><span class="sxs-lookup"><span data-stu-id="272b4-127">string</span></span>|<span data-ttu-id="272b4-128">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="272b4-128">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="272b4-129">Связи</span><span class="sxs-lookup"><span data-stu-id="272b4-129">Relationships</span></span>
<span data-ttu-id="272b4-130">Нет</span><span class="sxs-lookup"><span data-stu-id="272b4-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="272b4-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="272b4-131">JSON representation</span></span>

<span data-ttu-id="272b4-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="272b4-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->