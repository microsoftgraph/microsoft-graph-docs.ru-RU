---
title: Тип ресурса АудиоконференЦинг
description: Представляет сведения о доступе к телефонии для Онлинемитинг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 94dc02920e7270fbfdacb10ee9a8edee8315fc67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974285"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="5d605-103">Тип ресурса АудиоконференЦинг</span><span class="sxs-lookup"><span data-stu-id="5d605-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d605-104">Представляет сведения о доступе к телефонии для [онлинемитинг](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="5d605-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5d605-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d605-105">Properties</span></span>

| <span data-ttu-id="5d605-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d605-106">Property</span></span>            | <span data-ttu-id="5d605-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5d605-107">Type</span></span>    | <span data-ttu-id="5d605-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5d605-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="5d605-109">Диалинурл</span><span class="sxs-lookup"><span data-stu-id="5d605-109">dialinUrl</span></span>           | <span data-ttu-id="5d605-110">String</span><span class="sxs-lookup"><span data-stu-id="5d605-110">String</span></span>  | <span data-ttu-id="5d605-111">URL-адрес веб-страницы, которая содержит сведения о телефонном доступе.</span><span class="sxs-lookup"><span data-stu-id="5d605-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="5d605-112">Леадерпасскоде</span><span class="sxs-lookup"><span data-stu-id="5d605-112">leaderPasscode</span></span>      | <span data-ttu-id="5d605-113">String</span><span class="sxs-lookup"><span data-stu-id="5d605-113">String</span></span>  | <span data-ttu-id="5d605-114">Пароль заполнения, необходимый для подключения к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="5d605-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="5d605-115">ПартиЦипантпасскоде</span><span class="sxs-lookup"><span data-stu-id="5d605-115">participantPasscode</span></span> | <span data-ttu-id="5d605-116">String</span><span class="sxs-lookup"><span data-stu-id="5d605-116">String</span></span>  | <span data-ttu-id="5d605-117">Пароль участника, необходимый для подключения к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="5d605-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="5d605-118">Толлфринумбер</span><span class="sxs-lookup"><span data-stu-id="5d605-118">tollFreeNumber</span></span>      | <span data-ttu-id="5d605-119">String</span><span class="sxs-lookup"><span data-stu-id="5d605-119">String</span></span>  | <span data-ttu-id="5d605-120">Бесплатный номер для подключения к поставщику конференции с аудио.</span><span class="sxs-lookup"><span data-stu-id="5d605-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="5d605-121">Толлнумбер</span><span class="sxs-lookup"><span data-stu-id="5d605-121">tollNumber</span></span>          | <span data-ttu-id="5d605-122">String</span><span class="sxs-lookup"><span data-stu-id="5d605-122">String</span></span>  | <span data-ttu-id="5d605-123">Платный номер для подключения к поставщику конференции с аудио-и видеоконференциями.</span><span class="sxs-lookup"><span data-stu-id="5d605-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="5d605-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d605-124">JSON representation</span></span>

<span data-ttu-id="5d605-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d605-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
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
