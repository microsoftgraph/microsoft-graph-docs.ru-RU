---
title: Сценариев IVR в вызовах
description: Ниже приведены сценарии интерактивного речевого ответа (IVR), которые поддерживают вызова API в Microsoft Graph.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a3657d60344941de931e4f77bddde922d7d01f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936363"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="e5867-103">Сценариев IVR в вызовах</span><span class="sxs-lookup"><span data-stu-id="e5867-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="e5867-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5867-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5867-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5867-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5867-106">Ниже приведены сценарии интерактивного речевого ответа (IVR), которые поддерживают вызова API в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e5867-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="e5867-107">Воспроизведение звука строки — например, при звонок в очереди сотрудник службы поддержки пользователей.</span><span class="sxs-lookup"><span data-stu-id="e5867-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="e5867-108">Запишите — например, запись звука звонящего абонента, обычно после их Херд строки с параметрами.</span><span class="sxs-lookup"><span data-stu-id="e5867-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="e5867-109">Подпишитесь на тонового сигнала — например, если необходимо знать, какие DTMF звонков вызывающего абонента, обычно после слуха Звуковое приглашение выбрать.</span><span class="sxs-lookup"><span data-stu-id="e5867-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="e5867-110">Например, Отмена обработки мультимедиа - флажок Отменить все операции PlayPrompt или записи, которые находятся в процессе.</span><span class="sxs-lookup"><span data-stu-id="e5867-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
