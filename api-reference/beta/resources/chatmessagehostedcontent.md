---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 39939d9d61d992e5fd77fd21360ab05e8f83dbd4
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333365"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="ec337-103">Тип ресурса Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="ec337-103">chatMessageHostedContent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec337-104">Представляет контент, размещенный в сообщении чата, например изображения или фрагменты кода.</span><span class="sxs-lookup"><span data-stu-id="ec337-104">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="ec337-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ec337-105">Methods</span></span>

| <span data-ttu-id="ec337-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ec337-106">Method</span></span>       | <span data-ttu-id="ec337-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec337-107">Return Type</span></span> | <span data-ttu-id="ec337-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ec337-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ec337-109">Список Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="ec337-109">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="ec337-110">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="ec337-110">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="ec337-111">Получение списка **чатмессажехостедконтент** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="ec337-111">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="ec337-112">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="ec337-112">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="ec337-113">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="ec337-113">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="ec337-114">Чтение свойств и связей объекта **чатмессажехостедконтент** .</span><span class="sxs-lookup"><span data-stu-id="ec337-114">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec337-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec337-115">Properties</span></span>

| <span data-ttu-id="ec337-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec337-116">Property</span></span>     | <span data-ttu-id="ec337-117">Тип</span><span class="sxs-lookup"><span data-stu-id="ec337-117">Type</span></span>        | <span data-ttu-id="ec337-118">Описание</span><span class="sxs-lookup"><span data-stu-id="ec337-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec337-119">id</span><span class="sxs-lookup"><span data-stu-id="ec337-119">id</span></span>|<span data-ttu-id="ec337-120">String</span><span class="sxs-lookup"><span data-stu-id="ec337-120">String</span></span>| <span data-ttu-id="ec337-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec337-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec337-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="ec337-122">Relationships</span></span>

<span data-ttu-id="ec337-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ec337-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec337-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ec337-124">JSON representation</span></span>

<span data-ttu-id="ec337-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec337-125">The following is a JSON representation of the resource.</span></span>

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
