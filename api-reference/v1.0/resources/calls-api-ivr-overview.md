---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 9cbf0b9640c13c45730aa5842e150c4ad58767c4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913459"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="951b6-103">Сценарии IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="951b6-103">IVR scenarios in calls</span></span>

<span data-ttu-id="951b6-104">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="951b6-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="951b6-105">Воспроизведение звукового приглашения, например, при поступлении вызова в очередь агента обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="951b6-105">Playing an audio prompt - e.g., when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="951b6-106">Запись ответа, например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.</span><span class="sxs-lookup"><span data-stu-id="951b6-106">Recording a response - e.g., to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="951b6-107">Подписываться на звуки, например, если вы хотите узнать, какие звуки DTMF выбрал абонент, обычно после проявления звукового приглашения.</span><span class="sxs-lookup"><span data-stu-id="951b6-107">Subscribing to tones - e.g., when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
