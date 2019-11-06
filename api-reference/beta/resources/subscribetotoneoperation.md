---
title: Тип ресурса Субскрибетотонеоператион
description: Описывает формат ответа на создание подписки для получения тонов DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9f3a2f9cc3e32fd6455e2d692d4d4df2e9d502ac
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006538"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="f6bcb-103">Тип ресурса Субскрибетотонеоператион</span><span class="sxs-lookup"><span data-stu-id="f6bcb-103">SubscribeToToneOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6bcb-104">Описывает формат ответа на создание подписки для получения тонов DTMF.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-104">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="f6bcb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6bcb-105">Properties</span></span>

| <span data-ttu-id="f6bcb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6bcb-106">Property</span></span>                       | <span data-ttu-id="f6bcb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f6bcb-107">Type</span></span>                        | <span data-ttu-id="f6bcb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f6bcb-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f6bcb-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="f6bcb-109">clientContext</span></span>                  | <span data-ttu-id="f6bcb-110">String</span><span class="sxs-lookup"><span data-stu-id="f6bcb-110">String</span></span>                      | <span data-ttu-id="f6bcb-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="f6bcb-112">id</span><span class="sxs-lookup"><span data-stu-id="f6bcb-112">id</span></span>                             | <span data-ttu-id="f6bcb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f6bcb-113">String</span></span>                      | <span data-ttu-id="f6bcb-114">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-114">The server operation ID.</span></span> <span data-ttu-id="f6bcb-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-115">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="f6bcb-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f6bcb-116">resultInfo</span></span>                     | [<span data-ttu-id="f6bcb-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f6bcb-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="f6bcb-118">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-118">The result information.</span></span>  <span data-ttu-id="f6bcb-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-119">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="f6bcb-120">status</span><span class="sxs-lookup"><span data-stu-id="f6bcb-120">status</span></span>                         | <span data-ttu-id="f6bcb-121">String</span><span class="sxs-lookup"><span data-stu-id="f6bcb-121">String</span></span>                      | <span data-ttu-id="f6bcb-122">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="f6bcb-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-123">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="f6bcb-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="f6bcb-124">Relationships</span></span>
<span data-ttu-id="f6bcb-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f6bcb-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6bcb-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6bcb-126">JSON representation</span></span>

<span data-ttu-id="f6bcb-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6bcb-127">The following is a JSON representation of the resource.</span></span>

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
