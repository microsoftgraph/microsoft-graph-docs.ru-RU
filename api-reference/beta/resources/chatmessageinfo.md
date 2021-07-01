---
title: тип ресурса chatMessageInfo
description: Представляет предварительный просмотр ресурса chatMessage.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc03ee6743aa8115f5a231b3766cc2d6c3d5537b
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236318"
---
# <a name="chatmessageinfo-resource-type"></a><span data-ttu-id="1eb36-103">тип ресурса chatMessageInfo</span><span class="sxs-lookup"><span data-stu-id="1eb36-103">chatMessageInfo resource type</span></span>

<span data-ttu-id="1eb36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eb36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb36-105">Представляет предварительный просмотр [ресурса chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="1eb36-105">Represents a preview of a [chatMessage](../resources/chatmessage.md) resource.</span></span> <span data-ttu-id="1eb36-106">Этот объект может быть извлечен только в составе списка [чатов.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="1eb36-106">This object can only be fetched as part of a list of [chats](../resources/chat.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1eb36-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1eb36-107">Properties</span></span>
|<span data-ttu-id="1eb36-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1eb36-108">Property</span></span>|<span data-ttu-id="1eb36-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1eb36-109">Type</span></span>|<span data-ttu-id="1eb36-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1eb36-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eb36-111">body</span><span class="sxs-lookup"><span data-stu-id="1eb36-111">body</span></span>|[<span data-ttu-id="1eb36-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="1eb36-112">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="1eb36-113">Тело [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="1eb36-113">Body of the [chatMessage](../resources/chatmessage.md).</span></span> <span data-ttu-id="1eb36-114">Это будет по-прежнему содержать маркеры для @mentions и вложений, даже если объект не возвращает @mentions и вложения.</span><span class="sxs-lookup"><span data-stu-id="1eb36-114">This will still contain markers for @mentions and attachments even though the object does not return @mentions and attachments.</span></span>|
|<span data-ttu-id="1eb36-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1eb36-115">createdDateTime</span></span>|<span data-ttu-id="1eb36-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1eb36-116">DateTimeOffset</span></span>|<span data-ttu-id="1eb36-117">Объект времени даты, представляющий время создания сообщения.</span><span class="sxs-lookup"><span data-stu-id="1eb36-117">Date time object representing the time at which message was created.</span></span>|
|<span data-ttu-id="1eb36-118">from</span><span class="sxs-lookup"><span data-stu-id="1eb36-118">from</span></span>|[<span data-ttu-id="1eb36-119">chatMessageFromIdentitySet</span><span class="sxs-lookup"><span data-stu-id="1eb36-119">chatMessageFromIdentitySet</span></span>](../resources/chatmessagefromidentityset.md)|<span data-ttu-id="1eb36-120">Сведения о отправителье сообщения.</span><span class="sxs-lookup"><span data-stu-id="1eb36-120">Information about the sender of the message.</span></span>|
|<span data-ttu-id="1eb36-121">id</span><span class="sxs-lookup"><span data-stu-id="1eb36-121">id</span></span>|<span data-ttu-id="1eb36-122">String</span><span class="sxs-lookup"><span data-stu-id="1eb36-122">String</span></span>|<span data-ttu-id="1eb36-123">ID [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="1eb36-123">ID of the [chatMessage](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="1eb36-124">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1eb36-124">isDeleted</span></span>|<span data-ttu-id="1eb36-125">Логический</span><span class="sxs-lookup"><span data-stu-id="1eb36-125">Boolean</span></span>|<span data-ttu-id="1eb36-126">Если `true` установлено, исходное сообщение удалено.</span><span class="sxs-lookup"><span data-stu-id="1eb36-126">If set to `true`, the original message has been deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eb36-127">Связи</span><span class="sxs-lookup"><span data-stu-id="1eb36-127">Relationships</span></span>
<span data-ttu-id="1eb36-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1eb36-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eb36-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1eb36-129">JSON representation</span></span>
<span data-ttu-id="1eb36-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1eb36-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageInfo",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "createdDateTime": "String (timestamp)",
  "isDeleted": "Boolean"
}
```

## <a name="see-also"></a><span data-ttu-id="1eb36-131">См. также</span><span class="sxs-lookup"><span data-stu-id="1eb36-131">See also</span></span>

- [<span data-ttu-id="1eb36-132">chat</span><span class="sxs-lookup"><span data-stu-id="1eb36-132">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="1eb36-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="1eb36-133">chatMessage</span></span>](../resources/chatmessage.md)

