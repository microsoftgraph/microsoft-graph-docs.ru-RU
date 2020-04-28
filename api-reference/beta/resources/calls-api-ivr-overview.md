---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 62872c07dcf8072a9a5e471c53950a0b77b96814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507791"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="f6abb-103">Сценарии IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="f6abb-103">IVR scenarios in calls</span></span>

<span data-ttu-id="f6abb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6abb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6abb-105">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6abb-105">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="f6abb-106">Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="f6abb-106">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="f6abb-107">Запись ответа, например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.</span><span class="sxs-lookup"><span data-stu-id="f6abb-107">Recording a response -for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="f6abb-108">Подписываться на звуки, например, если вы хотите узнать, какие звуки DTMF выбрал абонент, обычно после проявления звукового приглашения.</span><span class="sxs-lookup"><span data-stu-id="f6abb-108">Subscribing to tones - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="f6abb-109">Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Рекордреспонсе, которые могут быть в процессе выполнения.</span><span class="sxs-lookup"><span data-stu-id="f6abb-109">Cancel media processing - for example, when you want to cancel any playPrompt or recordResponse operations that might be in process.</span></span>
