---
title: тип ресурса audioConferencing
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5f0c9338aefa592ed030585a6b0342d03e7717d0
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896699"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="0d876-103">тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="0d876-103">audioConferencing resource type</span></span>

<span data-ttu-id="0d876-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d876-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d876-105">Представляет сведения о доступе к телефону для [onlineMeeting.](onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="0d876-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0d876-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d876-106">Properties</span></span>

| <span data-ttu-id="0d876-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d876-107">Property</span></span>                    | <span data-ttu-id="0d876-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0d876-108">Type</span></span>              | <span data-ttu-id="0d876-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d876-109">Description</span></span>                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="0d876-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="0d876-110">dialinUrl</span></span>                   | <span data-ttu-id="0d876-111">String</span><span class="sxs-lookup"><span data-stu-id="0d876-111">String</span></span>            | <span data-ttu-id="0d876-112">URL-адрес веб-страницы, доступной извне, который содержит сведения о диалоговом номере.</span><span class="sxs-lookup"><span data-stu-id="0d876-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="0d876-113">conferenceId</span><span class="sxs-lookup"><span data-stu-id="0d876-113">conferenceId</span></span>                | <span data-ttu-id="0d876-114">String</span><span class="sxs-lookup"><span data-stu-id="0d876-114">String</span></span>            | <span data-ttu-id="0d876-115">ID конференции собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="0d876-115">The conference id of the online meeting.</span></span>                                       |
| <span data-ttu-id="0d876-116">tollFreeNumber (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="0d876-116">tollFreeNumber (deprecated)</span></span> | <span data-ttu-id="0d876-117">String</span><span class="sxs-lookup"><span data-stu-id="0d876-117">String</span></span>            | <span data-ttu-id="0d876-118">Бесплатный номер, подключенный к поставщику аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="0d876-118">The toll-free number that connects to the Audio Conference Provider.</span></span>           |
| <span data-ttu-id="0d876-119">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="0d876-119">tollFreeNumbers</span></span>             | <span data-ttu-id="0d876-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d876-120">String collection</span></span> | <span data-ttu-id="0d876-121">Список бесплатных номеров, отображаемого в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="0d876-121">List of toll-free numbers that are displayed in the meeting invite.</span></span>            |
| <span data-ttu-id="0d876-122">tollNumber (износ)</span><span class="sxs-lookup"><span data-stu-id="0d876-122">tollNumber (deprecated)</span></span>     | <span data-ttu-id="0d876-123">String</span><span class="sxs-lookup"><span data-stu-id="0d876-123">String</span></span>            | <span data-ttu-id="0d876-124">Платный номер, который подключается к поставщику аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="0d876-124">The toll number that connects to the Audio Conference Provider.</span></span>                |
| <span data-ttu-id="0d876-125">tollNumbers</span><span class="sxs-lookup"><span data-stu-id="0d876-125">tollNumbers</span></span>                 | <span data-ttu-id="0d876-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d876-126">String collection</span></span> | <span data-ttu-id="0d876-127">Список номеров платных номеров, отображаемого в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="0d876-127">List of toll numbers that are displayed in the meeting invite.</span></span>                 |

> [!CAUTION]
>
>- <span data-ttu-id="0d876-128">Свойства **tollFreeNumber** и **tollNumber** обесценяются.</span><span class="sxs-lookup"><span data-stu-id="0d876-128">The **tollFreeNumber** and **tollNumber** properties are deprecated.</span></span> <span data-ttu-id="0d876-129">Вместо этого **используйте свойства tollFreeNumbers** **и tollNumbers.**</span><span class="sxs-lookup"><span data-stu-id="0d876-129">Use the **tollFreeNumbers** and **tollNumbers** properties instead.</span></span>
>- <span data-ttu-id="0d876-130">Для обратной совместимости исходный **tollFreeNumber** добавляется в новую коллекцию **tollFreeNumbers,** а исходный **tollNumber** добавляется в новую коллекцию **tollNumbers.**</span><span class="sxs-lookup"><span data-stu-id="0d876-130">For backward compatibility, the original **tollFreeNumber** is added to the new **tollFreeNumbers** collection and the original **tollNumber** is added to the new **tollNumbers** collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d876-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d876-131">JSON representation</span></span>

<span data-ttu-id="0d876-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d876-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
  "tollFreeNumbers": ["String"],
  "tollNumbers": ["String"]
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


