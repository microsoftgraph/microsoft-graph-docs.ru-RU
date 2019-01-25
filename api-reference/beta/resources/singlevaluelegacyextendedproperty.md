---
title: Тип ресурса singleValueLegacyExtendedProperty
description: 'Расширенное свойство, содержащее одно значение. '
localization_priority: Normal
ms.openlocfilehash: 0d889756204853a525269f28cfdd3cc1b40be8a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512369"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="95815-103">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="95815-103">singleValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95815-104">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="95815-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="95815-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="95815-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="95815-106">Методы</span><span class="sxs-lookup"><span data-stu-id="95815-106">Methods</span></span>

| <span data-ttu-id="95815-107">Метод</span><span class="sxs-lookup"><span data-stu-id="95815-107">Method</span></span>           | <span data-ttu-id="95815-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95815-108">Return Type</span></span>    |<span data-ttu-id="95815-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95815-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95815-110">Post</span><span class="sxs-lookup"><span data-stu-id="95815-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="95815-111">Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md), но не группа [учета](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="95815-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="95815-112">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="95815-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="95815-113">Получение</span><span class="sxs-lookup"><span data-stu-id="95815-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="95815-114">Один или коллекцию поддерживаемых ресурсов экземпляра ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), или один экземпляр, включающим объект [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="95815-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="95815-115">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="95815-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="95815-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="95815-116">Properties</span></span>
| <span data-ttu-id="95815-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="95815-117">Property</span></span>     | <span data-ttu-id="95815-118">Тип</span><span class="sxs-lookup"><span data-stu-id="95815-118">Type</span></span>   |<span data-ttu-id="95815-119">Описание</span><span class="sxs-lookup"><span data-stu-id="95815-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95815-120">id</span><span class="sxs-lookup"><span data-stu-id="95815-120">id</span></span>|<span data-ttu-id="95815-121">string</span><span class="sxs-lookup"><span data-stu-id="95815-121">string</span></span>|<span data-ttu-id="95815-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95815-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="95815-124">value</span><span class="sxs-lookup"><span data-stu-id="95815-124">value</span></span>|<span data-ttu-id="95815-125">строка</span><span class="sxs-lookup"><span data-stu-id="95815-125">string</span></span>|<span data-ttu-id="95815-126">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="95815-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95815-127">Связи</span><span class="sxs-lookup"><span data-stu-id="95815-127">Relationships</span></span>
<span data-ttu-id="95815-128">Нет</span><span class="sxs-lookup"><span data-stu-id="95815-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="95815-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95815-129">JSON representation</span></span>

<span data-ttu-id="95815-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95815-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/singlevaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
