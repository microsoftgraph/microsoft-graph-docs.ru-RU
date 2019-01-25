---
title: Сценариев IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые поддерживают вызова API в Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519383"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="a7444-103">Сценариев IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="a7444-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7444-104">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые поддерживают вызова API в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a7444-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="a7444-105">Воспроизведение звука строки — например, при звонок в очереди сотрудник службы поддержки пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7444-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="a7444-106">Запишите — например, запись звука звонящего абонента, обычно после их Херд строки с параметрами.</span><span class="sxs-lookup"><span data-stu-id="a7444-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="a7444-107">Подпишитесь на тонового сигнала — например, если необходимо знать, какие DTMF звонков вызывающего абонента, обычно после слуха Звуковое приглашение выбрать.</span><span class="sxs-lookup"><span data-stu-id="a7444-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="a7444-108">Например, Отмена обработки мультимедиа - флажок Отменить все операции PlayPrompt или записи, которые находятся в процессе.</span><span class="sxs-lookup"><span data-stu-id="a7444-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
