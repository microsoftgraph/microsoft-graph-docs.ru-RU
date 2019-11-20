---
title: Тип ресурса МутепартиЦипантоператион
description: Описывает формат ответа для операции отключения участника вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a3e48179f2b08d5bb1097507fc4751f1d7d2b4e
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748387"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="4e6aa-103">Тип ресурса МутепартиЦипантоператион</span><span class="sxs-lookup"><span data-stu-id="4e6aa-103">MuteParticipantOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6aa-104">Описывает формат ответа для операции отключения участника вызова.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-104">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="4e6aa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e6aa-105">Properties</span></span>

| <span data-ttu-id="4e6aa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e6aa-106">Property</span></span>                       | <span data-ttu-id="4e6aa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4e6aa-107">Type</span></span>                        | <span data-ttu-id="4e6aa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4e6aa-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4e6aa-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="4e6aa-109">clientContext</span></span>                  | <span data-ttu-id="4e6aa-110">Строка</span><span class="sxs-lookup"><span data-stu-id="4e6aa-110">String</span></span>                      | <span data-ttu-id="4e6aa-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-111">Unique client context string.</span></span> <span data-ttu-id="4e6aa-112">Может содержать до 256 символов.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-112">Can have a maximum of 256 characters.</span></span>                                                                               |
| <span data-ttu-id="4e6aa-113">id</span><span class="sxs-lookup"><span data-stu-id="4e6aa-113">id</span></span>                             | <span data-ttu-id="4e6aa-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4e6aa-114">String</span></span>                      | <span data-ttu-id="4e6aa-115">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-115">The server operation ID.</span></span> <span data-ttu-id="4e6aa-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-116">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="4e6aa-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4e6aa-117">resultInfo</span></span>                     | [<span data-ttu-id="4e6aa-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4e6aa-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4e6aa-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-119">The result information.</span></span>  <span data-ttu-id="4e6aa-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-120">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="4e6aa-121">status</span><span class="sxs-lookup"><span data-stu-id="4e6aa-121">status</span></span>                         | <span data-ttu-id="4e6aa-122">String</span><span class="sxs-lookup"><span data-stu-id="4e6aa-122">String</span></span>                      | <span data-ttu-id="4e6aa-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4e6aa-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-124">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="4e6aa-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e6aa-125">Relationships</span></span>
<span data-ttu-id="4e6aa-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4e6aa-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e6aa-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e6aa-127">JSON representation</span></span>

<span data-ttu-id="4e6aa-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e6aa-128">The following is a JSON representation of the resource.</span></span>

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
