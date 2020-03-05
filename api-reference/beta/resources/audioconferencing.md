---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонной линии для собрания по сети.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab74b8819cc8dec7d63d5072cee1f1a147accd16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508124"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="ca515-103">Тип ресурса АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="ca515-103">audioConferencing resource type</span></span>

<span data-ttu-id="ca515-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ca515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca515-105">Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="ca515-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ca515-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca515-106">Properties</span></span>

| <span data-ttu-id="ca515-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca515-107">Property</span></span>            | <span data-ttu-id="ca515-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ca515-108">Type</span></span>    | <span data-ttu-id="ca515-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ca515-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="ca515-110">диалинурл</span><span class="sxs-lookup"><span data-stu-id="ca515-110">dialinUrl</span></span>           | <span data-ttu-id="ca515-111">String</span><span class="sxs-lookup"><span data-stu-id="ca515-111">String</span></span>  | <span data-ttu-id="ca515-112">URL-адрес веб-страницы, которая содержит сведения о телефонном доступе.</span><span class="sxs-lookup"><span data-stu-id="ca515-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="ca515-113">конференцеид</span><span class="sxs-lookup"><span data-stu-id="ca515-113">ConferenceId</span></span>        | <span data-ttu-id="ca515-114">String</span><span class="sxs-lookup"><span data-stu-id="ca515-114">String</span></span>  | <span data-ttu-id="ca515-115">Идентификатор конференции онлайн-собрания.</span><span class="sxs-lookup"><span data-stu-id="ca515-115">The conference id of the online meeting.</span></span>      |
| <span data-ttu-id="ca515-116">толлфринумбер</span><span class="sxs-lookup"><span data-stu-id="ca515-116">tollFreeNumber</span></span>      | <span data-ttu-id="ca515-117">String</span><span class="sxs-lookup"><span data-stu-id="ca515-117">String</span></span>  | <span data-ttu-id="ca515-118">Бесплатный номер, который подключается к поставщику конференции с аудио.</span><span class="sxs-lookup"><span data-stu-id="ca515-118">The toll-free number that connects to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="ca515-119">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="ca515-119">tollNumber</span></span>          | <span data-ttu-id="ca515-120">String</span><span class="sxs-lookup"><span data-stu-id="ca515-120">String</span></span>  | <span data-ttu-id="ca515-121">Платный номер, который подключается к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="ca515-121">The toll number that connects to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="ca515-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca515-122">JSON representation</span></span>

<span data-ttu-id="ca515-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca515-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "ConferenceId": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
