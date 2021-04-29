---
title: тип ресурса audioConferencing
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43332de03467b4a5cf9d9cc867718ceafd8c4e82
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080150"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="ccbe3-103">тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ccbe3-103">audioConferencing resource type</span></span>

<span data-ttu-id="ccbe3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccbe3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccbe3-105">Представляет сведения о доступе к телефону для [onlineMeeting.](onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="ccbe3-105">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ccbe3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccbe3-106">Properties</span></span>

| <span data-ttu-id="ccbe3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccbe3-107">Property</span></span>                    | <span data-ttu-id="ccbe3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ccbe3-108">Type</span></span>              | <span data-ttu-id="ccbe3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ccbe3-109">Description</span></span>                                                                    |
| :-------------------------- | :---------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="ccbe3-110">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="ccbe3-110">dialinUrl</span></span>                   | <span data-ttu-id="ccbe3-111">String</span><span class="sxs-lookup"><span data-stu-id="ccbe3-111">String</span></span>            | <span data-ttu-id="ccbe3-112">URL-адрес веб-страницы, доступной извне, который содержит сведения о диалоговом номере.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-112">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="ccbe3-113">conferenceId</span><span class="sxs-lookup"><span data-stu-id="ccbe3-113">conferenceId</span></span>                | <span data-ttu-id="ccbe3-114">String</span><span class="sxs-lookup"><span data-stu-id="ccbe3-114">String</span></span>            | <span data-ttu-id="ccbe3-115">ID конференции собрания в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-115">The conference id of the online meeting.</span></span>                                       |
| <span data-ttu-id="ccbe3-116">tollFreeNumber (обесценилось)</span><span class="sxs-lookup"><span data-stu-id="ccbe3-116">tollFreeNumber (deprecated)</span></span> | <span data-ttu-id="ccbe3-117">String</span><span class="sxs-lookup"><span data-stu-id="ccbe3-117">String</span></span>            | <span data-ttu-id="ccbe3-118">Бесплатный номер, подключенный к поставщику аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-118">The toll-free number that connects to the Audio Conference Provider.</span></span>           |
| <span data-ttu-id="ccbe3-119">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="ccbe3-119">tollFreeNumbers</span></span>             | <span data-ttu-id="ccbe3-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ccbe3-120">String collection</span></span> | <span data-ttu-id="ccbe3-121">Список бесплатных номеров, отображаемого в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-121">List of toll-free numbers that are displayed in the meeting invite.</span></span>            |
| <span data-ttu-id="ccbe3-122">tollNumber (износ)</span><span class="sxs-lookup"><span data-stu-id="ccbe3-122">tollNumber (deprecated)</span></span>     | <span data-ttu-id="ccbe3-123">String</span><span class="sxs-lookup"><span data-stu-id="ccbe3-123">String</span></span>            | <span data-ttu-id="ccbe3-124">Платный номер, который подключается к поставщику аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-124">The toll number that connects to the Audio Conference Provider.</span></span>                |
| <span data-ttu-id="ccbe3-125">tollNumbers</span><span class="sxs-lookup"><span data-stu-id="ccbe3-125">tollNumbers</span></span>                 | <span data-ttu-id="ccbe3-126">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ccbe3-126">String collection</span></span> | <span data-ttu-id="ccbe3-127">Список номеров платных номеров, отображаемого в приглашении на собрание.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-127">List of toll numbers that are displayed in the meeting invite.</span></span>                 |

> [!CAUTION]
>
>- <span data-ttu-id="ccbe3-128">Свойства **tollFreeNumber** и **tollNumber** обесценяются.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-128">The **tollFreeNumber** and **tollNumber** properties are deprecated.</span></span> <span data-ttu-id="ccbe3-129">Вместо этого **используйте свойства tollFreeNumbers** **и tollNumbers.**</span><span class="sxs-lookup"><span data-stu-id="ccbe3-129">Use the **tollFreeNumbers** and **tollNumbers** properties instead.</span></span>
>- <span data-ttu-id="ccbe3-130">Для обратной совместимости исходный **tollFreeNumber** добавляется в новую коллекцию **tollFreeNumbers,** а исходный **tollNumber** добавляется в новую коллекцию **tollNumbers.**</span><span class="sxs-lookup"><span data-stu-id="ccbe3-130">For backward compatibility, the original **tollFreeNumber** is added to the new **tollFreeNumbers** collection and the original **tollNumber** is added to the new **tollNumbers** collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccbe3-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ccbe3-131">JSON representation</span></span>

<span data-ttu-id="ccbe3-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccbe3-132">The following is a JSON representation of the resource.</span></span>

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


