---
title: Работа с API коммуникаций в Microsoft Graph
description: API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: b70006aad978ce05c63f62354a3ac7f27105e4f9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913228"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="57b4d-103">Работа с API коммуникаций в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="57b4d-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="57b4d-104">API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах.</span><span class="sxs-lookup"><span data-stu-id="57b4d-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="57b4d-105">Этот API можно использовать для создания и приема звонков, а также для создания и получения координат собраний.</span><span class="sxs-lookup"><span data-stu-id="57b4d-105">You can use this API to create and receive calls as well as create and retrieve meeting coordinates.</span></span>

<span data-ttu-id="57b4d-106">API коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, а также создающих собрания и получающих приглашения на них от имени пользователей.</span><span class="sxs-lookup"><span data-stu-id="57b4d-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="57b4d-107">Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них.</span><span class="sxs-lookup"><span data-stu-id="57b4d-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="57b4d-108">С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="57b4d-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="57b4d-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57b4d-109">Authorization</span></span>

<span data-ttu-id="57b4d-110">Для доступа к API коммуникаций требуется одно из указанных ниже [разрешений](https://docs.microsoft.com/graph/permissions-reference#calls-permissions).</span><span class="sxs-lookup"><span data-stu-id="57b4d-110">One of the following [permissions](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="57b4d-111">Эти разрешения должны предоставляться администратором</span><span class="sxs-lookup"><span data-stu-id="57b4d-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="57b4d-112">Сценарий</span><span class="sxs-lookup"><span data-stu-id="57b4d-112">Scenario</span></span>                 | <span data-ttu-id="57b4d-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57b4d-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="57b4d-114">Звонки</span><span class="sxs-lookup"><span data-stu-id="57b4d-114">Calling</span></span>                 | <span data-ttu-id="57b4d-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="57b4d-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="57b4d-116">Собрания</span><span class="sxs-lookup"><span data-stu-id="57b4d-116">Meetings</span></span>                 | <span data-ttu-id="57b4d-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="57b4d-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="57b4d-118">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="57b4d-118">Common use cases</span></span>

<span data-ttu-id="57b4d-119">В таблице ниже перечислены некоторые распространенные варианты использования API коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="57b4d-119">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="57b4d-120">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="57b4d-120">Use cases</span></span>                         | <span data-ttu-id="57b4d-121">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="57b4d-121">REST resources</span></span>                                 | <span data-ttu-id="57b4d-122">См. также</span><span class="sxs-lookup"><span data-stu-id="57b4d-122">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="57b4d-123">Создание приватных и групповых звонков, а также присоединение к ним</span><span class="sxs-lookup"><span data-stu-id="57b4d-123">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="57b4d-124">Звонок</span><span class="sxs-lookup"><span data-stu-id="57b4d-124">Call</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="57b4d-125">Методы звонков</span><span class="sxs-lookup"><span data-stu-id="57b4d-125">Methods for calls</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="57b4d-126">Звонки с интерактивным речевым взаимодействием</span><span class="sxs-lookup"><span data-stu-id="57b4d-126">IVR calls</span></span>   |     | [<span data-ttu-id="57b4d-127">Методы для интерактивного речевого взаимодействия</span><span class="sxs-lookup"><span data-stu-id="57b4d-127">Methods for IVR</span></span>](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="57b4d-128">Элементы управления звонком (участник)</span><span class="sxs-lookup"><span data-stu-id="57b4d-128">Call controls (participant)</span></span> | [<span data-ttu-id="57b4d-129">Участник</span><span class="sxs-lookup"><span data-stu-id="57b4d-129">Participant</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="57b4d-130">Собрания</span><span class="sxs-lookup"><span data-stu-id="57b4d-130">Meetings</span></span>|[<span data-ttu-id="57b4d-131">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="57b4d-131">onlineMeeting</span></span>](https://docs.microsoft.comgraph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="57b4d-132">Методы для собраний</span><span class="sxs-lookup"><span data-stu-id="57b4d-132">Methods for meetings</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|

## <a name="common-properties"></a><span data-ttu-id="57b4d-133">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="57b4d-133">Common properties</span></span>

| <span data-ttu-id="57b4d-134">Ресурс</span><span class="sxs-lookup"><span data-stu-id="57b4d-134">Resource</span></span>                | <span data-ttu-id="57b4d-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="57b4d-135">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="57b4d-136">call</span><span class="sxs-lookup"><span data-stu-id="57b4d-136">call</span></span>                               | [<span data-ttu-id="57b4d-137">свойства объекта call</span><span class="sxs-lookup"><span data-stu-id="57b4d-137">call properties</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="57b4d-138">participant</span><span class="sxs-lookup"><span data-stu-id="57b4d-138">participant</span></span>                         | [<span data-ttu-id="57b4d-139">свойства объекта participant</span><span class="sxs-lookup"><span data-stu-id="57b4d-139">participant properties</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="57b4d-140">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="57b4d-140">onlineMeeting</span></span>                            | [<span data-ttu-id="57b4d-141">свойства объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="57b4d-141">onlineMeeting properties</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |

## <a name="see-also"></a><span data-ttu-id="57b4d-142">См. также</span><span class="sxs-lookup"><span data-stu-id="57b4d-142">See also</span></span>

- [<span data-ttu-id="57b4d-143">Примеры API коммуникаций</span><span class="sxs-lookup"><span data-stu-id="57b4d-143">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="57b4d-144">Пакет SDK для передачи сигналов коммуникаций</span><span class="sxs-lookup"><span data-stu-id="57b4d-144">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="57b4d-145">Пакет SDK мультимедиа коммуникаций</span><span class="sxs-lookup"><span data-stu-id="57b4d-145">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)
