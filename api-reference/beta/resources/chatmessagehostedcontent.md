---
title: тип ресурса chatMessageHostedContent
description: Содержимое, которое было организовано в сообщении чата
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2434253ef303123ac7d64695cdbbc6172d7989c
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626232"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="a24d7-103">тип ресурса chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="a24d7-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="a24d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a24d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a24d7-105">Представляет содержимое Teams, которое было организовано в сообщении чата, например изображения или фрагменты кода.</span><span class="sxs-lookup"><span data-stu-id="a24d7-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="a24d7-106">[Вложения файлов](chatmessageattachment.md) не являются хост-контентом; они хранятся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a24d7-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="a24d7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a24d7-107">Methods</span></span>

| <span data-ttu-id="a24d7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a24d7-108">Method</span></span>       | <span data-ttu-id="a24d7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a24d7-109">Return Type</span></span> | <span data-ttu-id="a24d7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a24d7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a24d7-111">Список chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="a24d7-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="a24d7-112">[коллекция chatMessageHostedContent](chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="a24d7-112">[chatMessageHostedContent](chatmessagehostedcontent.md) collection</span></span> | <span data-ttu-id="a24d7-113">Извлечение списка **chatMessageHostedContent** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="a24d7-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="a24d7-114">Get chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="a24d7-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="a24d7-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="a24d7-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="a24d7-116">Ознакомьтесь с свойствами и отношениями объекта **chatMessageHostedContent.**</span><span class="sxs-lookup"><span data-stu-id="a24d7-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a24d7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a24d7-117">Properties</span></span>

<span data-ttu-id="a24d7-118">chatMessageHostedContent происходит из [teamworkHostedContent](teamworkhostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="a24d7-118">chatMessageHostedContent derives from [teamworkHostedContent](teamworkhostedcontent.md)</span></span>

| <span data-ttu-id="a24d7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a24d7-119">Property</span></span>     | <span data-ttu-id="a24d7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a24d7-120">Type</span></span>        | <span data-ttu-id="a24d7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a24d7-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a24d7-122">id</span><span class="sxs-lookup"><span data-stu-id="a24d7-122">id</span></span>            |<span data-ttu-id="a24d7-123">String</span><span class="sxs-lookup"><span data-stu-id="a24d7-123">String</span></span>       | <span data-ttu-id="a24d7-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a24d7-124">Read-only.</span></span> <span data-ttu-id="a24d7-125">Представляет идентификатор контента в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="a24d7-125">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="a24d7-126">contentBytes</span><span class="sxs-lookup"><span data-stu-id="a24d7-126">contentBytes</span></span>  |<span data-ttu-id="a24d7-127">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="a24d7-127">Edm.Binary</span></span>   | <span data-ttu-id="a24d7-128">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="a24d7-128">Write-only.</span></span> <span data-ttu-id="a24d7-129">При размещении нового контента, размещенного в чате, представляются bytes полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="a24d7-129">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="a24d7-130">Они представлены как строка base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="a24d7-130">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="a24d7-131">contentType</span><span class="sxs-lookup"><span data-stu-id="a24d7-131">contentType</span></span>   |<span data-ttu-id="a24d7-132">String</span><span class="sxs-lookup"><span data-stu-id="a24d7-132">String</span></span>       | <span data-ttu-id="a24d7-133">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="a24d7-133">Write-only.</span></span> <span data-ttu-id="a24d7-134">При размещении нового контента, размещенного в чате, представлен тип контента, например изображения/png.</span><span class="sxs-lookup"><span data-stu-id="a24d7-134">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="a24d7-135">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="a24d7-135">Instance attributes</span></span>

<span data-ttu-id="a24d7-136">Атрибуты экземпляра — это свойства с особым поведением.</span><span class="sxs-lookup"><span data-stu-id="a24d7-136">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="a24d7-137">Эти свойства являются временными и определяют поведение, которое служба должна выполнять или предоставлять краткосрочные значения свойств, например URL-адрес загрузки элемента с истекшим сроком действия.</span><span class="sxs-lookup"><span data-stu-id="a24d7-137">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="a24d7-138">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a24d7-138">Property name</span></span>                     | <span data-ttu-id="a24d7-139">Тип</span><span class="sxs-lookup"><span data-stu-id="a24d7-139">Type</span></span>   | <span data-ttu-id="a24d7-140">Описание</span><span class="sxs-lookup"><span data-stu-id="a24d7-140">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="a24d7-141">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="a24d7-141">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="a24d7-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a24d7-142">string</span></span> | <span data-ttu-id="a24d7-143">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="a24d7-143">Write-only.</span></span> <span data-ttu-id="a24d7-144">Представляет временный ИД для размещенного контента при отправке сообщения для ссылки на размещаемую информацию в **отправленных ресурсах chatMessage.**</span><span class="sxs-lookup"><span data-stu-id="a24d7-144">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a24d7-145">Связи</span><span class="sxs-lookup"><span data-stu-id="a24d7-145">Relationships</span></span>

<span data-ttu-id="a24d7-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a24d7-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a24d7-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a24d7-147">JSON representation</span></span>

<span data-ttu-id="a24d7-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a24d7-148">The following is a JSON representation of the resource.</span></span>

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


