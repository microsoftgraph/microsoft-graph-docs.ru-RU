---
title: Сценарии IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 3b33a673218238f861e7122de8320d6c8a20e435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042732"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="0eb62-103">Сценарии IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="0eb62-103">IVR scenarios in calls</span></span>

<span data-ttu-id="0eb62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eb62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eb62-105">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые вызываются API-интерфейсам в службе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0eb62-105">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="0eb62-106">Воспроизведение звуковых запросов, например, при поступлении вызова в очередь агента обслуживания клиентов.</span><span class="sxs-lookup"><span data-stu-id="0eb62-106">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="0eb62-107">Запись ответа, например, для записи звука вызывающего абонента, как правило, после того, как он слышал приглашение с параметрами.</span><span class="sxs-lookup"><span data-stu-id="0eb62-107">Recording a response -for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="0eb62-108">Подписываться на звуки, например, если вы хотите узнать, какие звуки DTMF выбрал абонент, обычно после проявления звукового приглашения.</span><span class="sxs-lookup"><span data-stu-id="0eb62-108">Subscribing to tones - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="0eb62-109">Отмена обработки мультимедиа — например, если вы хотите отменить все операции Плайпромпт или Рекордреспонсе, которые могут быть в процессе выполнения.</span><span class="sxs-lookup"><span data-stu-id="0eb62-109">Cancel media processing - for example, when you want to cancel any playPrompt or recordResponse operations that might be in process.</span></span>


