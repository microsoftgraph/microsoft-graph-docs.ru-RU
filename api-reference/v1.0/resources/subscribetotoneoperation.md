---
title: Тип ресурса Субскрибетотонеоператион
description: Описывает формат ответа на создание подписки для получения тонов DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6d1e42d375dd53fcb71ae049622c59d2d31b3406
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913543"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="cf1b2-103">Тип ресурса Субскрибетотонеоператион</span><span class="sxs-lookup"><span data-stu-id="cf1b2-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="cf1b2-104">Описывает формат ответа на создание подписки для получения тонов DTMF.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="cf1b2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf1b2-105">Properties</span></span>

| <span data-ttu-id="cf1b2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf1b2-106">Property</span></span>                       | <span data-ttu-id="cf1b2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cf1b2-107">Type</span></span>                        | <span data-ttu-id="cf1b2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cf1b2-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cf1b2-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="cf1b2-109">clientContext</span></span>                  | <span data-ttu-id="cf1b2-110">String</span><span class="sxs-lookup"><span data-stu-id="cf1b2-110">String</span></span>                      | <span data-ttu-id="cf1b2-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="cf1b2-112">id</span><span class="sxs-lookup"><span data-stu-id="cf1b2-112">id</span></span>                             | <span data-ttu-id="cf1b2-113">Строка</span><span class="sxs-lookup"><span data-stu-id="cf1b2-113">String</span></span>                      | <span data-ttu-id="cf1b2-114">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-114">The server operation ID.</span></span> <span data-ttu-id="cf1b2-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="cf1b2-116">status</span><span class="sxs-lookup"><span data-stu-id="cf1b2-116">status</span></span>                         | <span data-ttu-id="cf1b2-117">String</span><span class="sxs-lookup"><span data-stu-id="cf1b2-117">String</span></span>                      | <span data-ttu-id="cf1b2-118">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-118">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="cf1b2-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-119">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="cf1b2-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="cf1b2-120">Relationships</span></span>
<span data-ttu-id="cf1b2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="cf1b2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf1b2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf1b2-122">JSON representation</span></span>

<span data-ttu-id="cf1b2-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribeToToneOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
