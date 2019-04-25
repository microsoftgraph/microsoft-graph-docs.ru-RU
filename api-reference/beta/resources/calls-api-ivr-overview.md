---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535577"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="1c099-103">Сценарии IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="1c099-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c099-104">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c099-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="1c099-105">Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="1c099-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="1c099-106">Запись — например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.</span><span class="sxs-lookup"><span data-stu-id="1c099-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="1c099-107">ПодПишитесь на тон — например, если вы хотите узнать, какие звуки DTMF выбрал абонент, как правило, после проявления звукового приглашения.</span><span class="sxs-lookup"><span data-stu-id="1c099-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="1c099-108">Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Record, которые могут быть в процессе.</span><span class="sxs-lookup"><span data-stu-id="1c099-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
