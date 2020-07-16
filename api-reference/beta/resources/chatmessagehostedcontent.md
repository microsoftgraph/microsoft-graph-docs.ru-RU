---
title: Тип ресурса Чатмессажехостедконтент
description: Контент, размещенный в сообщении чата
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 421ed3b1c439a7ae550100a113c651ab3e0a34b9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791071"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="2dc8f-103">Тип ресурса Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2dc8f-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="2dc8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dc8f-105">Представляет контент Teams, размещенный в сообщении чата, например в виде изображений или фрагментов кода.</span><span class="sxs-lookup"><span data-stu-id="2dc8f-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="2dc8f-106">[Вложенные файлы](chatmessageattachment.md) не являются размещающих контентом, они хранятся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2dc8f-106">[File attachments](chatmessageattachment.md) are not hosted content, they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="2dc8f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2dc8f-107">Methods</span></span>

| <span data-ttu-id="2dc8f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2dc8f-108">Method</span></span>       | <span data-ttu-id="2dc8f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2dc8f-109">Return Type</span></span> | <span data-ttu-id="2dc8f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc8f-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2dc8f-111">Список Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2dc8f-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="2dc8f-112">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2dc8f-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="2dc8f-113">Получение списка **чатмессажехостедконтент** для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2dc8f-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="2dc8f-114">Получение Чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2dc8f-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="2dc8f-115">чатмессажехостедконтент</span><span class="sxs-lookup"><span data-stu-id="2dc8f-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="2dc8f-116">Чтение свойств и связей объекта **чатмессажехостедконтент** .</span><span class="sxs-lookup"><span data-stu-id="2dc8f-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2dc8f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dc8f-117">Properties</span></span>

| <span data-ttu-id="2dc8f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dc8f-118">Property</span></span>     | <span data-ttu-id="2dc8f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2dc8f-119">Type</span></span>        | <span data-ttu-id="2dc8f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc8f-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2dc8f-121">id</span><span class="sxs-lookup"><span data-stu-id="2dc8f-121">id</span></span>|<span data-ttu-id="2dc8f-122">String</span><span class="sxs-lookup"><span data-stu-id="2dc8f-122">String</span></span>| <span data-ttu-id="2dc8f-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2dc8f-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dc8f-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="2dc8f-124">Relationships</span></span>

<span data-ttu-id="2dc8f-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2dc8f-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dc8f-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2dc8f-126">JSON representation</span></span>

<span data-ttu-id="2dc8f-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dc8f-127">The following is a JSON representation of the resource.</span></span>

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
