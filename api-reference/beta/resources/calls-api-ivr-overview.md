---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 25f9339f33a6a679a8c8829214526fc29bc88b04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013042"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="2b918-103">Сценарии IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="2b918-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b918-104">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2b918-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="2b918-105">Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="2b918-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="2b918-106">Запись — например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.</span><span class="sxs-lookup"><span data-stu-id="2b918-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="2b918-107">Подпишитесь на тон — например, если вы хотите узнать, какие звуки DTMF выбрал абонент, как правило, после проявления звукового приглашения.</span><span class="sxs-lookup"><span data-stu-id="2b918-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="2b918-108">Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Record, которые могут быть в процессе.</span><span class="sxs-lookup"><span data-stu-id="2b918-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
