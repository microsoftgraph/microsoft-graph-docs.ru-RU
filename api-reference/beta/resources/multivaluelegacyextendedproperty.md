---
title: Тип ресурса multiValueLegacyExtendedProperty
description: Расширенное свойство, содержащее коллекцию значений.
localization_priority: Normal
ms.openlocfilehash: de77f94076fe6bb2f0aa3ded3b1839b8d25ce752
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575893"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="efd62-103">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="efd62-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd62-104">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="efd62-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="efd62-105">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="efd62-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="efd62-106">Методы</span><span class="sxs-lookup"><span data-stu-id="efd62-106">Methods</span></span>

| <span data-ttu-id="efd62-107">Метод</span><span class="sxs-lookup"><span data-stu-id="efd62-107">Method</span></span>           | <span data-ttu-id="efd62-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efd62-108">Return Type</span></span>    |<span data-ttu-id="efd62-109">Описание</span><span class="sxs-lookup"><span data-stu-id="efd62-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efd62-110">Post</span><span class="sxs-lookup"><span data-stu-id="efd62-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="efd62-111">Поддерживаемые ресурсов экземпляра: [сообщения](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md)или [папки задач Outlook](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="efd62-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="efd62-112">Обратите внимание, что, группа [записи](../resources/post.md) не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efd62-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="efd62-113">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="efd62-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="efd62-114">Get</span><span class="sxs-lookup"><span data-stu-id="efd62-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="efd62-115">Экземпляр поддерживаемые ресурсов ([сообщение](../resources/message.md), [mailFolder](../resources/mailfolder.md), [события](../resources/event.md), [календаря](../resources/calendar.md), [контактов](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [задачи Outlook](../resources/outlooktask.md), [папки задач Outlook](../resources/outlooktaskfolder.md)или группа [учета](../resources/post.md)), включающим [ multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="efd62-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="efd62-116">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="efd62-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="efd62-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="efd62-117">Properties</span></span>
| <span data-ttu-id="efd62-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="efd62-118">Property</span></span>     | <span data-ttu-id="efd62-119">Тип</span><span class="sxs-lookup"><span data-stu-id="efd62-119">Type</span></span>   |<span data-ttu-id="efd62-120">Описание</span><span class="sxs-lookup"><span data-stu-id="efd62-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efd62-121">id</span><span class="sxs-lookup"><span data-stu-id="efd62-121">id</span></span>|<span data-ttu-id="efd62-122">string</span><span class="sxs-lookup"><span data-stu-id="efd62-122">string</span></span>|<span data-ttu-id="efd62-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efd62-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="efd62-125">value</span><span class="sxs-lookup"><span data-stu-id="efd62-125">value</span></span>|<span data-ttu-id="efd62-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="efd62-126">string collection</span></span>|<span data-ttu-id="efd62-127">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="efd62-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efd62-128">Связи</span><span class="sxs-lookup"><span data-stu-id="efd62-128">Relationships</span></span>
<span data-ttu-id="efd62-129">Нет</span><span class="sxs-lookup"><span data-stu-id="efd62-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="efd62-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efd62-130">JSON representation</span></span>

<span data-ttu-id="efd62-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efd62-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/multivaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
