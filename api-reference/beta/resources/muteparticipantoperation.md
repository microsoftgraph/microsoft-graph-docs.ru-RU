---
title: Тип ресурса МутепартиЦипантоператион
description: Описывает формат ответа для операции отключения участника вызова.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5d5e716e4d8266d97139c1283415994f6206aea
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006622"
---
# <a name="muteparticipantoperation-resource-type"></a><span data-ttu-id="68e17-103">Тип ресурса МутепартиЦипантоператион</span><span class="sxs-lookup"><span data-stu-id="68e17-103">MuteParticipantOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e17-104">Описывает формат ответа для операции отключения участника вызова.</span><span class="sxs-lookup"><span data-stu-id="68e17-104">Describes the response format of a call participant mute operation.</span></span>

## <a name="properties"></a><span data-ttu-id="68e17-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="68e17-105">Properties</span></span>

| <span data-ttu-id="68e17-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="68e17-106">Property</span></span>                       | <span data-ttu-id="68e17-107">Тип</span><span class="sxs-lookup"><span data-stu-id="68e17-107">Type</span></span>                        | <span data-ttu-id="68e17-108">Описание</span><span class="sxs-lookup"><span data-stu-id="68e17-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68e17-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="68e17-109">clientContext</span></span>                  | <span data-ttu-id="68e17-110">String</span><span class="sxs-lookup"><span data-stu-id="68e17-110">String</span></span>                      | <span data-ttu-id="68e17-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="68e17-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="68e17-112">id</span><span class="sxs-lookup"><span data-stu-id="68e17-112">id</span></span>                             | <span data-ttu-id="68e17-113">Строка</span><span class="sxs-lookup"><span data-stu-id="68e17-113">String</span></span>                      | <span data-ttu-id="68e17-114">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="68e17-114">The server operation ID.</span></span> <span data-ttu-id="68e17-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68e17-115">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="68e17-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="68e17-116">resultInfo</span></span>                     | [<span data-ttu-id="68e17-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="68e17-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="68e17-118">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="68e17-118">The result information.</span></span>  <span data-ttu-id="68e17-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68e17-119">Read-only.</span></span>                                                                                            |
| <span data-ttu-id="68e17-120">status</span><span class="sxs-lookup"><span data-stu-id="68e17-120">status</span></span>                         | <span data-ttu-id="68e17-121">String</span><span class="sxs-lookup"><span data-stu-id="68e17-121">String</span></span>                      | <span data-ttu-id="68e17-122">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="68e17-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="68e17-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68e17-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="68e17-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="68e17-124">Relationships</span></span>
<span data-ttu-id="68e17-125">Нет</span><span class="sxs-lookup"><span data-stu-id="68e17-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68e17-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68e17-126">JSON representation</span></span>

<span data-ttu-id="68e17-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68e17-127">The following is a JSON representation of the resource.</span></span>

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
