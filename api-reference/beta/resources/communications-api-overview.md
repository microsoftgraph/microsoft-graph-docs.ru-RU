---
title: Работа с API коммуникаций в Microsoft Graph
description: API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: dbad2e21d5e3dbdae37ab30b02d2a96970722040
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870353"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="e7bcd-103">Работа с API коммуникаций в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e7bcd-103">Working with the communications API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7bcd-104">API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="e7bcd-105">Этот API можно использовать для создания и приема звонков, создания и получения координат собраний, а также проверки присутствия пользователей.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="e7bcd-106">API коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, создающих собрания и получающих приглашения на них от имени пользователей, а также для проверки доступности пользователей и их действий.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users and to check their presence availability and activity.</span></span>
<span data-ttu-id="e7bcd-107">Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="e7bcd-108">С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="e7bcd-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7bcd-109">Authorization</span></span>

<span data-ttu-id="e7bcd-110">Для доступа к API коммуникаций требуется одно из указанных ниже [разрешений](/graph/permissions-reference#calls-permissions).</span><span class="sxs-lookup"><span data-stu-id="e7bcd-110">One of the following [permissions](/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="e7bcd-111">Эти разрешения должны предоставляться администратором</span><span class="sxs-lookup"><span data-stu-id="e7bcd-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="e7bcd-112">Сценарий</span><span class="sxs-lookup"><span data-stu-id="e7bcd-112">Scenario</span></span>                 | <span data-ttu-id="e7bcd-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7bcd-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="e7bcd-114">Звонки</span><span class="sxs-lookup"><span data-stu-id="e7bcd-114">Calling</span></span>                 | <span data-ttu-id="e7bcd-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="e7bcd-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="e7bcd-116">Собрания</span><span class="sxs-lookup"><span data-stu-id="e7bcd-116">Meetings</span></span>                 | <span data-ttu-id="e7bcd-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7bcd-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="e7bcd-118">Присутствие</span><span class="sxs-lookup"><span data-stu-id="e7bcd-118">Presence</span></span>                 | <span data-ttu-id="e7bcd-119">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7bcd-119">Presence.Read, Presence.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="e7bcd-120">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="e7bcd-120">Common use cases</span></span>

<span data-ttu-id="e7bcd-121">В таблице ниже перечислены некоторые распространенные варианты использования API коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="e7bcd-121">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="e7bcd-122">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="e7bcd-122">Use cases</span></span>                         | <span data-ttu-id="e7bcd-123">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="e7bcd-123">REST resources</span></span>                                 | <span data-ttu-id="e7bcd-124">См. также</span><span class="sxs-lookup"><span data-stu-id="e7bcd-124">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="e7bcd-125">Создание приватных и групповых звонков, а также присоединение к ним</span><span class="sxs-lookup"><span data-stu-id="e7bcd-125">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="e7bcd-126">Звонок</span><span class="sxs-lookup"><span data-stu-id="e7bcd-126">Call</span></span>](/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="e7bcd-127">Методы звонков</span><span class="sxs-lookup"><span data-stu-id="e7bcd-127">Methods for calls</span></span>](/graph/api/resources/call?view=graph-rest-beta#methods)|
|<span data-ttu-id="e7bcd-128">Звонки с интерактивным речевым взаимодействием</span><span class="sxs-lookup"><span data-stu-id="e7bcd-128">IVR calls</span></span>   |     | [<span data-ttu-id="e7bcd-129">Методы для интерактивного речевого взаимодействия</span><span class="sxs-lookup"><span data-stu-id="e7bcd-129">Methods for IVR</span></span>](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="e7bcd-130">Элементы управления звонком (участник)</span><span class="sxs-lookup"><span data-stu-id="e7bcd-130">Call controls (participant)</span></span> | [<span data-ttu-id="e7bcd-131">Участник</span><span class="sxs-lookup"><span data-stu-id="e7bcd-131">Participant</span></span>](/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="e7bcd-132">Собрания</span><span class="sxs-lookup"><span data-stu-id="e7bcd-132">Meetings</span></span>|[<span data-ttu-id="e7bcd-133">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="e7bcd-133">onlineMeeting</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="e7bcd-134">Методы для собраний</span><span class="sxs-lookup"><span data-stu-id="e7bcd-134">Methods for meetings</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|<span data-ttu-id="e7bcd-135">Присутствие</span><span class="sxs-lookup"><span data-stu-id="e7bcd-135">Presence</span></span> | [<span data-ttu-id="e7bcd-136">presence</span><span class="sxs-lookup"><span data-stu-id="e7bcd-136">presence</span></span>](/graph/api/resources/presence) | [<span data-ttu-id="e7bcd-137">Методы для присутствия</span><span class="sxs-lookup"><span data-stu-id="e7bcd-137">Methods for presence</span></span>](/graph/api/resources/presence#methods) |

## <a name="common-properties"></a><span data-ttu-id="e7bcd-138">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="e7bcd-138">Common properties</span></span>

| <span data-ttu-id="e7bcd-139">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e7bcd-139">Resource</span></span>                | <span data-ttu-id="e7bcd-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7bcd-140">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="e7bcd-141">call</span><span class="sxs-lookup"><span data-stu-id="e7bcd-141">call</span></span>                               | [<span data-ttu-id="e7bcd-142">свойства объекта call</span><span class="sxs-lookup"><span data-stu-id="e7bcd-142">call properties</span></span>](/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="e7bcd-143">participant</span><span class="sxs-lookup"><span data-stu-id="e7bcd-143">participant</span></span>                         | [<span data-ttu-id="e7bcd-144">свойства объекта participant</span><span class="sxs-lookup"><span data-stu-id="e7bcd-144">participant properties</span></span>](/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="e7bcd-145">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="e7bcd-145">onlineMeeting</span></span>                            | [<span data-ttu-id="e7bcd-146">свойства объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="e7bcd-146">onlineMeeting properties</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| <span data-ttu-id="e7bcd-147">presence</span><span class="sxs-lookup"><span data-stu-id="e7bcd-147">presence</span></span> | [<span data-ttu-id="e7bcd-148">свойства объекта presence</span><span class="sxs-lookup"><span data-stu-id="e7bcd-148">presence properties</span></span>](/graph/api/resources/presence#properties) |

## <a name="see-also"></a><span data-ttu-id="e7bcd-149">См. также</span><span class="sxs-lookup"><span data-stu-id="e7bcd-149">See also</span></span>

- [<span data-ttu-id="e7bcd-150">Примеры API коммуникаций</span><span class="sxs-lookup"><span data-stu-id="e7bcd-150">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="e7bcd-151">Пакет SDK для передачи сигналов коммуникаций</span><span class="sxs-lookup"><span data-stu-id="e7bcd-151">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="e7bcd-152">Пакет SDK мультимедиа коммуникаций</span><span class="sxs-lookup"><span data-stu-id="e7bcd-152">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
