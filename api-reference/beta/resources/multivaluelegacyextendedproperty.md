---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
ms.openlocfilehash: 86ba1969e06dc549d1fca00148cbea96f94cf4b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506259"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="20198-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="20198-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20198-104">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="20198-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="20198-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="20198-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="20198-106">Методы</span><span class="sxs-lookup"><span data-stu-id="20198-106">Methods</span></span>

| <span data-ttu-id="20198-107">Метод</span><span class="sxs-lookup"><span data-stu-id="20198-107">Method</span></span>           | <span data-ttu-id="20198-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20198-108">Return Type</span></span>    |<span data-ttu-id="20198-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20198-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20198-110">Post</span><span class="sxs-lookup"><span data-stu-id="20198-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="20198-111">Поддерживаемый экземпляр ресурса: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)или [Outlook Task](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="20198-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="20198-112">Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="20198-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="20198-113">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="20198-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="20198-114">Получение</span><span class="sxs-lookup"><span data-stu-id="20198-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="20198-115">Поддерживаемый экземпляр ресурса ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task Task](../resources/outlooktask.md), [Outlook Task Folder](../resources/outlooktaskfolder.md)или POST Group [POST](../resources/post.md)), дополненный [ Объект multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="20198-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="20198-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="20198-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="20198-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="20198-117">Properties</span></span>
| <span data-ttu-id="20198-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="20198-118">Property</span></span>     | <span data-ttu-id="20198-119">Тип</span><span class="sxs-lookup"><span data-stu-id="20198-119">Type</span></span>   |<span data-ttu-id="20198-120">Описание</span><span class="sxs-lookup"><span data-stu-id="20198-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20198-121">id</span><span class="sxs-lookup"><span data-stu-id="20198-121">id</span></span>|<span data-ttu-id="20198-122">строка</span><span class="sxs-lookup"><span data-stu-id="20198-122">string</span></span>|<span data-ttu-id="20198-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20198-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="20198-125">значение</span><span class="sxs-lookup"><span data-stu-id="20198-125">value</span></span>|<span data-ttu-id="20198-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20198-126">string collection</span></span>|<span data-ttu-id="20198-127">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="20198-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20198-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="20198-128">Relationships</span></span>
<span data-ttu-id="20198-129">Нет</span><span class="sxs-lookup"><span data-stu-id="20198-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="20198-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20198-130">JSON representation</span></span>

<span data-ttu-id="20198-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20198-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/multivaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
