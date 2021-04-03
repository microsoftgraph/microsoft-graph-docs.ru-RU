---
title: тип ресурса chatMessageHostedContent
description: Содержимое, которое было организовано в сообщении чата
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 842ccdcad3f185eb64572c91ce5b82d673a1d43f
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582566"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="c3ca0-103">тип ресурса chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="c3ca0-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="c3ca0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3ca0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3ca0-105">Представляет содержимое Teams, которое было организовано в сообщении чата, например изображения или фрагменты кода.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="c3ca0-106">[Вложения файлов](chatmessageattachment.md) не являются хост-контентом; они хранятся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="c3ca0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c3ca0-107">Methods</span></span>

| <span data-ttu-id="c3ca0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c3ca0-108">Method</span></span>       | <span data-ttu-id="c3ca0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3ca0-109">Return Type</span></span> | <span data-ttu-id="c3ca0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3ca0-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c3ca0-111">Список chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="c3ca0-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-hostedcontents.md) | <span data-ttu-id="c3ca0-112">[коллекция chatMessageHostedContent](chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ca0-112">[chatMessageHostedContent](chatmessagehostedcontent.md) collection</span></span> | <span data-ttu-id="c3ca0-113">Извлечение списка **chatMessageHostedContent** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="c3ca0-114">Get chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="c3ca0-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="c3ca0-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="c3ca0-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="c3ca0-116">Ознакомьтесь с свойствами и отношениями объекта **chatMessageHostedContent.**</span><span class="sxs-lookup"><span data-stu-id="c3ca0-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3ca0-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3ca0-117">Properties</span></span>

<span data-ttu-id="c3ca0-118">chatMessageHostedContent происходит из [teamworkHostedContent](teamworkhostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="c3ca0-118">chatMessageHostedContent derives from [teamworkHostedContent](teamworkhostedcontent.md)</span></span>

| <span data-ttu-id="c3ca0-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3ca0-119">Property</span></span>     | <span data-ttu-id="c3ca0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c3ca0-120">Type</span></span>        | <span data-ttu-id="c3ca0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3ca0-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c3ca0-122">id</span><span class="sxs-lookup"><span data-stu-id="c3ca0-122">id</span></span>            |<span data-ttu-id="c3ca0-123">String</span><span class="sxs-lookup"><span data-stu-id="c3ca0-123">String</span></span>       | <span data-ttu-id="c3ca0-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-124">Read-only.</span></span> <span data-ttu-id="c3ca0-125">Представляет идентификатор контента в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-125">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="c3ca0-126">contentBytes</span><span class="sxs-lookup"><span data-stu-id="c3ca0-126">contentBytes</span></span>  |<span data-ttu-id="c3ca0-127">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="c3ca0-127">Edm.Binary</span></span>   | <span data-ttu-id="c3ca0-128">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-128">Write-only.</span></span> <span data-ttu-id="c3ca0-129">При размещении нового контента, размещенного в чате, представляются bytes полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-129">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="c3ca0-130">Они представлены как строка base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-130">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="c3ca0-131">contentType</span><span class="sxs-lookup"><span data-stu-id="c3ca0-131">contentType</span></span>   |<span data-ttu-id="c3ca0-132">String</span><span class="sxs-lookup"><span data-stu-id="c3ca0-132">String</span></span>       | <span data-ttu-id="c3ca0-133">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-133">Write-only.</span></span> <span data-ttu-id="c3ca0-134">При размещении нового контента, размещенного в чате, представлен тип контента, например изображения/png.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-134">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="c3ca0-135">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="c3ca0-135">Instance attributes</span></span>

<span data-ttu-id="c3ca0-136">Атрибуты экземпляра — это свойства с особым поведением.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-136">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="c3ca0-137">Эти свойства являются временными и определяют поведение, которое служба должна выполнять или предоставлять краткосрочные значения свойств, например URL-адрес загрузки элемента с истекшим сроком действия.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-137">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="c3ca0-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c3ca0-138">Property name</span></span>                     | <span data-ttu-id="c3ca0-139">Тип</span><span class="sxs-lookup"><span data-stu-id="c3ca0-139">Type</span></span>   | <span data-ttu-id="c3ca0-140">Описание</span><span class="sxs-lookup"><span data-stu-id="c3ca0-140">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="c3ca0-141">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="c3ca0-141">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="c3ca0-142">string</span><span class="sxs-lookup"><span data-stu-id="c3ca0-142">string</span></span> | <span data-ttu-id="c3ca0-143">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-143">Write-only.</span></span> <span data-ttu-id="c3ca0-144">Представляет временный ИД для размещенного контента при отправке сообщения для ссылки на размещаемую информацию в **отправленных ресурсах chatMessage.**</span><span class="sxs-lookup"><span data-stu-id="c3ca0-144">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3ca0-145">Связи</span><span class="sxs-lookup"><span data-stu-id="c3ca0-145">Relationships</span></span>

<span data-ttu-id="c3ca0-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3ca0-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3ca0-147">JSON representation</span></span>

<span data-ttu-id="c3ca0-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3ca0-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String"
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


