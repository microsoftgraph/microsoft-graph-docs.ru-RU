---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: f1a7e2c84083675037bbf146f5660afe6fee0a31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871403"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="5825d-103">Сценарии IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="5825d-103">IVR scenarios in calls</span></span>

<span data-ttu-id="5825d-104">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5825d-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="5825d-105">Воспроизведение звукового приглашения, например, при поступлении вызова в очередь агента обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="5825d-105">Playing an audio prompt - e.g., when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="5825d-106">Запись ответа, например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.</span><span class="sxs-lookup"><span data-stu-id="5825d-106">Recording a response - e.g., to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="5825d-107">Подписываться на звуки, например, если вы хотите узнать, какие звуки DTMF выбрал абонент, обычно после проявления звукового приглашения.</span><span class="sxs-lookup"><span data-stu-id="5825d-107">Subscribing to tones - e.g., when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
