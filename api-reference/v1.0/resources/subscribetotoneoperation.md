---
title: Тип ресурса Субскрибетотонеоператион
description: Описывает формат ответа на создание подписки для получения тонов DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a53405f58c568d17d040dd7368f39cef6838510c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094164"
---
# <a name="subscribetotoneoperation-resource-type"></a><span data-ttu-id="20f4e-103">Тип ресурса Субскрибетотонеоператион</span><span class="sxs-lookup"><span data-stu-id="20f4e-103">SubscribeToToneOperation resource type</span></span>

<span data-ttu-id="20f4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20f4e-105">Описывает формат ответа на создание подписки для получения тонов DTMF.</span><span class="sxs-lookup"><span data-stu-id="20f4e-105">Describes the response format of creation of subscription to receive DTMF tones.</span></span>

## <a name="properties"></a><span data-ttu-id="20f4e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="20f4e-106">Properties</span></span>

| <span data-ttu-id="20f4e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="20f4e-107">Property</span></span>                       | <span data-ttu-id="20f4e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="20f4e-108">Type</span></span>                        | <span data-ttu-id="20f4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20f4e-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="20f4e-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="20f4e-110">clientContext</span></span>                  | <span data-ttu-id="20f4e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="20f4e-111">String</span></span>                      | <span data-ttu-id="20f4e-112">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="20f4e-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="20f4e-113">id</span><span class="sxs-lookup"><span data-stu-id="20f4e-113">id</span></span>                             | <span data-ttu-id="20f4e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="20f4e-114">String</span></span>                      | <span data-ttu-id="20f4e-115">ИДЕНТИФИКАТОР операции сервера.</span><span class="sxs-lookup"><span data-stu-id="20f4e-115">The server operation ID.</span></span> <span data-ttu-id="20f4e-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20f4e-116">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="20f4e-117">status</span><span class="sxs-lookup"><span data-stu-id="20f4e-117">status</span></span>                         | <span data-ttu-id="20f4e-118">String</span><span class="sxs-lookup"><span data-stu-id="20f4e-118">String</span></span>                      | <span data-ttu-id="20f4e-119">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="20f4e-119">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="20f4e-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20f4e-120">Read-only.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="20f4e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="20f4e-121">Relationships</span></span>
<span data-ttu-id="20f4e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="20f4e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20f4e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20f4e-123">JSON representation</span></span>

<span data-ttu-id="20f4e-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20f4e-124">The following is a JSON representation of the resource.</span></span>

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

