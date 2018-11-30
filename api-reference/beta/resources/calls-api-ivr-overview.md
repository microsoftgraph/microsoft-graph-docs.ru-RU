---
title: Сценариев IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые поддерживают вызова API в Microsoft Graph.
ms.openlocfilehash: 22318b2bc755b161a55fc42fd924017545d38e3b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074893"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="6cb8b-103">Сценариев IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="6cb8b-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="6cb8b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cb8b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cb8b-106">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые поддерживают вызова API в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="6cb8b-107">Воспроизведение звука строки — например, при звонок в очереди сотрудник службы поддержки пользователей.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="6cb8b-108">Запишите — например, запись звука звонящего абонента, обычно после их Херд строки с параметрами.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="6cb8b-109">Подпишитесь на тонового сигнала — например, если необходимо знать, какие DTMF звонков вызывающего абонента, обычно после слуха Звуковое приглашение выбрать.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="6cb8b-110">Например, Отмена обработки мультимедиа - флажок Отменить все операции PlayPrompt или записи, которые находятся в процессе.</span><span class="sxs-lookup"><span data-stu-id="6cb8b-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
