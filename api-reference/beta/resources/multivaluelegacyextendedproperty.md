---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
ms.openlocfilehash: 86ba1969e06dc549d1fca00148cbea96f94cf4b6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512950"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="c038d-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="c038d-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c038d-104">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="c038d-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="c038d-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="c038d-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="c038d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c038d-106">Methods</span></span>

| <span data-ttu-id="c038d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c038d-107">Method</span></span>           | <span data-ttu-id="c038d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c038d-108">Return Type</span></span>    |<span data-ttu-id="c038d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c038d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c038d-110">Post</span><span class="sxs-lookup"><span data-stu-id="c038d-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="c038d-111">Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c038d-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="c038d-112">Обратите внимание, что, группа [записи](../resources/post.md) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c038d-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="c038d-113">Создание объекта multiValueLegacyExtendedProperty в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="c038d-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="c038d-114">Get</span><span class="sxs-lookup"><span data-stu-id="c038d-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="c038d-115">Экземпляр поддерживаемые ресурсов ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), включающим [ multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="c038d-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="c038d-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="c038d-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="c038d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c038d-117">Properties</span></span>
| <span data-ttu-id="c038d-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c038d-118">Property</span></span>     | <span data-ttu-id="c038d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c038d-119">Type</span></span>   |<span data-ttu-id="c038d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c038d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c038d-121">id</span><span class="sxs-lookup"><span data-stu-id="c038d-121">id</span></span>|<span data-ttu-id="c038d-122">string</span><span class="sxs-lookup"><span data-stu-id="c038d-122">string</span></span>|<span data-ttu-id="c038d-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c038d-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="c038d-125">value</span><span class="sxs-lookup"><span data-stu-id="c038d-125">value</span></span>|<span data-ttu-id="c038d-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c038d-126">string collection</span></span>|<span data-ttu-id="c038d-127">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="c038d-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c038d-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c038d-128">Relationships</span></span>
<span data-ttu-id="c038d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c038d-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c038d-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c038d-130">JSON representation</span></span>

<span data-ttu-id="c038d-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c038d-131">Here is a JSON representation of the resource.</span></span>

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
