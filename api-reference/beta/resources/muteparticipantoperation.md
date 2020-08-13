---
title: Тип ресурса МутепартиЦипантоператион
description: Описывает формат ответа для операции отключения участника вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b7eb9821f21af7a037723815a9b670ac3c41041
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522605"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="b27b0-103">Тип ресурса МутепартиЦипантоператион</span><span class="sxs-lookup"><span data-stu-id="b27b0-103">MuteParticipantOperation resource type</span></span>

<span data-ttu-id="b27b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b27b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b27b0-105">Описывает формат ответа для операции отключения участника вызова.</span><span class="sxs-lookup"><span data-stu-id="b27b0-105">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="b27b0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b27b0-106">Properties</span></span>

| <span data-ttu-id="b27b0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b27b0-107">Property</span></span>                       | <span data-ttu-id="b27b0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b27b0-108">Type</span></span>                        | <span data-ttu-id="b27b0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b27b0-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b27b0-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="b27b0-110">clientContext</span></span>                  | <span data-ttu-id="b27b0-111">Строка</span><span class="sxs-lookup"><span data-stu-id="b27b0-111">String</span></span>                      | <span data-ttu-id="b27b0-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="b27b0-112">Unique client context string.</span></span> <span data-ttu-id="b27b0-113">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="b27b0-113">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="b27b0-114">id</span><span class="sxs-lookup"><span data-stu-id="b27b0-114">id</span></span>                             | <span data-ttu-id="b27b0-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b27b0-115">String</span></span>                      | <span data-ttu-id="b27b0-116">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="b27b0-116">The server operation ID.</span></span> <span data-ttu-id="b27b0-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b27b0-117">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="b27b0-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b27b0-118">resultInfo</span></span>                     | [<span data-ttu-id="b27b0-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b27b0-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b27b0-120">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="b27b0-120">The result information.</span></span>  <span data-ttu-id="b27b0-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b27b0-121">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="b27b0-122">status</span><span class="sxs-lookup"><span data-stu-id="b27b0-122">status</span></span>                         | <span data-ttu-id="b27b0-123">String</span><span class="sxs-lookup"><span data-stu-id="b27b0-123">String</span></span>                      | <span data-ttu-id="b27b0-124">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b27b0-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b27b0-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b27b0-125">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="b27b0-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="b27b0-126">Relationships</span></span>
<span data-ttu-id="b27b0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b27b0-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b27b0-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b27b0-128">JSON representation</span></span>

<span data-ttu-id="b27b0-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b27b0-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.muteParticipantOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "muteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
