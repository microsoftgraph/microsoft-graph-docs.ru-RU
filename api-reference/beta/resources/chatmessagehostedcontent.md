---
title: Тип ресурса chatMessageHostedContent
description: Содержимое, которое было в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cc4f61fb0b0e6c174be50c988d1cbb22576c4f27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159621"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="7f136-103">Тип ресурса chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7f136-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="7f136-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f136-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f136-105">Представляет содержимое Teams, которое имеется в сообщении чата, например изображения или фрагменты кода.</span><span class="sxs-lookup"><span data-stu-id="7f136-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="7f136-106">[Вложенные файлы](chatmessageattachment.md) не являются контентом; они хранятся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7f136-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="7f136-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7f136-107">Methods</span></span>

| <span data-ttu-id="7f136-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7f136-108">Method</span></span>       | <span data-ttu-id="7f136-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7f136-109">Return Type</span></span> | <span data-ttu-id="7f136-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f136-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7f136-111">Список chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7f136-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="7f136-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7f136-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="7f136-113">Получить список **chatMessageHostedContent** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="7f136-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="7f136-114">Get chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7f136-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="7f136-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="7f136-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="7f136-116">Чтение свойств и связей объекта **chatMessageHostedContent.**</span><span class="sxs-lookup"><span data-stu-id="7f136-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7f136-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f136-117">Properties</span></span>

| <span data-ttu-id="7f136-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f136-118">Property</span></span>     | <span data-ttu-id="7f136-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7f136-119">Type</span></span>        | <span data-ttu-id="7f136-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7f136-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f136-121">id</span><span class="sxs-lookup"><span data-stu-id="7f136-121">id</span></span>            |<span data-ttu-id="7f136-122">String</span><span class="sxs-lookup"><span data-stu-id="7f136-122">String</span></span>       | <span data-ttu-id="7f136-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f136-123">Read-only.</span></span> <span data-ttu-id="7f136-124">Представляет идентификатор содержимого сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="7f136-124">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="7f136-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="7f136-125">contentBytes</span></span>  |<span data-ttu-id="7f136-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="7f136-126">Edm.Binary</span></span>   | <span data-ttu-id="7f136-127">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="7f136-127">Write-only.</span></span> <span data-ttu-id="7f136-128">При публикации нового размещенного содержимого сообщения чата представляет количество полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="7f136-128">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="7f136-129">Они представлены в качестве строки base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="7f136-129">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="7f136-130">contentType</span><span class="sxs-lookup"><span data-stu-id="7f136-130">contentType</span></span>   |<span data-ttu-id="7f136-131">String</span><span class="sxs-lookup"><span data-stu-id="7f136-131">String</span></span>       | <span data-ttu-id="7f136-132">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="7f136-132">Write-only.</span></span> <span data-ttu-id="7f136-133">При публикации нового размещенного содержимого сообщения чата представляет тип содержимого, например изображение/png.</span><span class="sxs-lookup"><span data-stu-id="7f136-133">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="7f136-134">Атрибуты экземпляра</span><span class="sxs-lookup"><span data-stu-id="7f136-134">Instance attributes</span></span>

<span data-ttu-id="7f136-135">Атрибуты экземпляра — это свойства с особым поведением.</span><span class="sxs-lookup"><span data-stu-id="7f136-135">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="7f136-136">Эти свойства являются временными и определяют поведение, которое должна выполнять служба, или предоставляют краткосрочные значения свойств, например URL-адрес скачивания элемента, срок действия которого истекает.</span><span class="sxs-lookup"><span data-stu-id="7f136-136">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="7f136-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7f136-137">Property name</span></span>                     | <span data-ttu-id="7f136-138">Тип</span><span class="sxs-lookup"><span data-stu-id="7f136-138">Type</span></span>   | <span data-ttu-id="7f136-139">Описание</span><span class="sxs-lookup"><span data-stu-id="7f136-139">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="7f136-140">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="7f136-140">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="7f136-141">string</span><span class="sxs-lookup"><span data-stu-id="7f136-141">string</span></span> | <span data-ttu-id="7f136-142">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="7f136-142">Write-only.</span></span> <span data-ttu-id="7f136-143">Представляет temporaryId размещенного содержимого при публикации сообщения для ссылки на размещенное содержимое в отправляемом ресурсе **chatMessage.**</span><span class="sxs-lookup"><span data-stu-id="7f136-143">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f136-144">Связи</span><span class="sxs-lookup"><span data-stu-id="7f136-144">Relationships</span></span>

<span data-ttu-id="7f136-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7f136-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f136-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7f136-146">JSON representation</span></span>

<span data-ttu-id="7f136-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f136-147">The following is a JSON representation of the resource.</span></span>

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


