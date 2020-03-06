---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a34e09b233a60858e23155f87808e40d080867f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507707"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="2f62f-103">Тип ресурса Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2f62f-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="2f62f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f62f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f62f-105">Представляет контент, размещенный в сообщении чата, например изображения или фрагменты кода.</span><span class="sxs-lookup"><span data-stu-id="2f62f-105">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="2f62f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2f62f-106">Methods</span></span>

| <span data-ttu-id="2f62f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2f62f-107">Method</span></span>       | <span data-ttu-id="2f62f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f62f-108">Return Type</span></span> | <span data-ttu-id="2f62f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f62f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2f62f-110">Список Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2f62f-110">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="2f62f-111">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2f62f-111">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="2f62f-112">Получение списка **чатмессажехостедконтент** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2f62f-112">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="2f62f-113">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2f62f-113">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="2f62f-114">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2f62f-114">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="2f62f-115">Чтение свойств и связей объекта **чатмессажехостедконтент** .</span><span class="sxs-lookup"><span data-stu-id="2f62f-115">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f62f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f62f-116">Properties</span></span>

| <span data-ttu-id="2f62f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f62f-117">Property</span></span>     | <span data-ttu-id="2f62f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2f62f-118">Type</span></span>        | <span data-ttu-id="2f62f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2f62f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f62f-120">id</span><span class="sxs-lookup"><span data-stu-id="2f62f-120">id</span></span>|<span data-ttu-id="2f62f-121">String</span><span class="sxs-lookup"><span data-stu-id="2f62f-121">String</span></span>| <span data-ttu-id="2f62f-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f62f-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f62f-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="2f62f-123">Relationships</span></span>

<span data-ttu-id="2f62f-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2f62f-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f62f-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2f62f-125">JSON representation</span></span>

<span data-ttu-id="2f62f-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f62f-126">The following is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)"
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
