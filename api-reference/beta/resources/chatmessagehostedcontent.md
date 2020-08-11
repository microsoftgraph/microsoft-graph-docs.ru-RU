---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8f1577ab7ded60dfd3cad88641bfb11f83d6ad5b
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630293"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="c690c-103">Тип ресурса Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="c690c-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="c690c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c690c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c690c-105">Представляет контент Teams, размещенный в сообщении чата, например в виде изображений или фрагментов кода.</span><span class="sxs-lookup"><span data-stu-id="c690c-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="c690c-106">[Вложенные файлы](chatmessageattachment.md) не являются размещающих контентом; они хранятся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c690c-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="c690c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c690c-107">Methods</span></span>

| <span data-ttu-id="c690c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c690c-108">Method</span></span>       | <span data-ttu-id="c690c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c690c-109">Return Type</span></span> | <span data-ttu-id="c690c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c690c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c690c-111">Список Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="c690c-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="c690c-112">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="c690c-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="c690c-113">Получение списка **чатмессажехостедконтент** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="c690c-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="c690c-114">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="c690c-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="c690c-115">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="c690c-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="c690c-116">Чтение свойств и связей объекта **чатмессажехостедконтент** .</span><span class="sxs-lookup"><span data-stu-id="c690c-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c690c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c690c-117">Properties</span></span>

| <span data-ttu-id="c690c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c690c-118">Property</span></span>     | <span data-ttu-id="c690c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c690c-119">Type</span></span>        | <span data-ttu-id="c690c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c690c-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c690c-121">id</span><span class="sxs-lookup"><span data-stu-id="c690c-121">id</span></span>            |<span data-ttu-id="c690c-122">String</span><span class="sxs-lookup"><span data-stu-id="c690c-122">String</span></span>       | <span data-ttu-id="c690c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c690c-123">Read-only.</span></span> <span data-ttu-id="c690c-124">Представляет размещенный идентификатор контента сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="c690c-124">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="c690c-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="c690c-125">contentBytes</span></span>  |<span data-ttu-id="c690c-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="c690c-126">Edm.Binary</span></span>   | <span data-ttu-id="c690c-127">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c690c-127">Write-only.</span></span> <span data-ttu-id="c690c-128">При учете нового контента, размещенного в чате, представляет байты полезных данных.</span><span class="sxs-lookup"><span data-stu-id="c690c-128">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="c690c-129">Они представлены в виде строки base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="c690c-129">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="c690c-130">contentType</span><span class="sxs-lookup"><span data-stu-id="c690c-130">contentType</span></span>   |<span data-ttu-id="c690c-131">String</span><span class="sxs-lookup"><span data-stu-id="c690c-131">String</span></span>       | <span data-ttu-id="c690c-132">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c690c-132">Write-only.</span></span> <span data-ttu-id="c690c-133">При учете нового контента, размещенного в чате, представляет тип контента, например Image/PNG.</span><span class="sxs-lookup"><span data-stu-id="c690c-133">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="c690c-134">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="c690c-134">Instance attributes</span></span>

<span data-ttu-id="c690c-135">Атрибуты экземпляра — это свойства с особым поведением.</span><span class="sxs-lookup"><span data-stu-id="c690c-135">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="c690c-136">Эти свойства являются временными и задают поведение службы или предоставляют краткосрочные значения свойств, например URL-адрес скачивания для элемента, срок действия которого истечет.</span><span class="sxs-lookup"><span data-stu-id="c690c-136">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="c690c-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c690c-137">Property name</span></span>                     | <span data-ttu-id="c690c-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c690c-138">Type</span></span>   | <span data-ttu-id="c690c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c690c-139">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="c690c-140">@microsoft. Graph. Темпорарид</span><span class="sxs-lookup"><span data-stu-id="c690c-140">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="c690c-141">string</span><span class="sxs-lookup"><span data-stu-id="c690c-141">string</span></span> | <span data-ttu-id="c690c-142">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c690c-142">Write-only.</span></span> <span data-ttu-id="c690c-143">Представляет Темпорарид для размещаемого контента при публикации сообщения для ссылки на размещенный контент в ресурсе **chatMessage** , который отправляется.</span><span class="sxs-lookup"><span data-stu-id="c690c-143">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c690c-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="c690c-144">Relationships</span></span>

<span data-ttu-id="c690c-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c690c-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c690c-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c690c-146">JSON representation</span></span>

<span data-ttu-id="c690c-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c690c-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
