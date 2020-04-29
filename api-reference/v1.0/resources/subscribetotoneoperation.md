---
title: Тип ресурса Субскрибетотонеоператион
description: Описывает формат ответа на создание подписки для получения тонов DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f29d385060d93b8de54ee27f9f948f83e3ad2711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533615"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="56e59-103">Тип ресурса Субскрибетотонеоператион</span><span class="sxs-lookup"><span data-stu-id="56e59-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="56e59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56e59-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56e59-105">Описывает формат ответа на создание подписки для получения тонов DTMF.</span><span class="sxs-lookup"><span data-stu-id="56e59-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="56e59-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="56e59-106">Properties</span></span>

| <span data-ttu-id="56e59-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="56e59-107">Property</span></span>                       | <span data-ttu-id="56e59-108">Тип</span><span class="sxs-lookup"><span data-stu-id="56e59-108">Type</span></span>                        | <span data-ttu-id="56e59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="56e59-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="56e59-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="56e59-110">clientContext</span></span>                  | <span data-ttu-id="56e59-111">String</span><span class="sxs-lookup"><span data-stu-id="56e59-111">String</span></span>                      | <span data-ttu-id="56e59-112">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="56e59-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="56e59-113">id</span><span class="sxs-lookup"><span data-stu-id="56e59-113">id</span></span>                             | <span data-ttu-id="56e59-114">Строка</span><span class="sxs-lookup"><span data-stu-id="56e59-114">String</span></span>                      | <span data-ttu-id="56e59-115">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="56e59-115">The server operation ID.</span></span> <span data-ttu-id="56e59-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="56e59-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="56e59-117">status</span><span class="sxs-lookup"><span data-stu-id="56e59-117">status</span></span>                         | <span data-ttu-id="56e59-118">String</span><span class="sxs-lookup"><span data-stu-id="56e59-118">String</span></span>                      | <span data-ttu-id="56e59-119">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="56e59-119">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="56e59-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="56e59-120">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="56e59-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="56e59-121">Relationships</span></span>
<span data-ttu-id="56e59-122">Нет</span><span class="sxs-lookup"><span data-stu-id="56e59-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56e59-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56e59-123">JSON representation</span></span>

<span data-ttu-id="56e59-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56e59-124">The following is a JSON representation of the resource.</span></span>

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
