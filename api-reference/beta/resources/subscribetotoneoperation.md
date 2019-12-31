---
title: Тип ресурса Субскрибетотонеоператион
description: Описывает формат ответа на создание подписки для получения тонов DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0b10062ed51aae20d6d4268da349b9b429d6c528
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913690"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="0216c-103">Тип ресурса Субскрибетотонеоператион</span><span class="sxs-lookup"><span data-stu-id="0216c-103">SubscribeToToneOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0216c-104">Описывает формат ответа на создание подписки для получения тонов DTMF.</span><span class="sxs-lookup"><span data-stu-id="0216c-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="0216c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0216c-105">Properties</span></span>

| <span data-ttu-id="0216c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0216c-106">Property</span></span>                       | <span data-ttu-id="0216c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0216c-107">Type</span></span>                        | <span data-ttu-id="0216c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0216c-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0216c-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="0216c-109">clientContext</span></span>                  | <span data-ttu-id="0216c-110">String</span><span class="sxs-lookup"><span data-stu-id="0216c-110">String</span></span>                      | <span data-ttu-id="0216c-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="0216c-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="0216c-112">id</span><span class="sxs-lookup"><span data-stu-id="0216c-112">id</span></span>                             | <span data-ttu-id="0216c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0216c-113">String</span></span>                      | <span data-ttu-id="0216c-114">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="0216c-114">The server operation ID.</span></span> <span data-ttu-id="0216c-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0216c-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="0216c-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0216c-116">resultInfo</span></span>                     | [<span data-ttu-id="0216c-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0216c-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0216c-118">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="0216c-118">The result information.</span></span>  <span data-ttu-id="0216c-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0216c-119">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="0216c-120">status</span><span class="sxs-lookup"><span data-stu-id="0216c-120">status</span></span>                         | <span data-ttu-id="0216c-121">String</span><span class="sxs-lookup"><span data-stu-id="0216c-121">String</span></span>                      | <span data-ttu-id="0216c-122">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0216c-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0216c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0216c-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="0216c-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="0216c-124">Relationships</span></span>
<span data-ttu-id="0216c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0216c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0216c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0216c-126">JSON representation</span></span>

<span data-ttu-id="0216c-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0216c-127">The following is a JSON representation of the resource.</span></span>

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
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
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
