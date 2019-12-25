---
title: Работа с API коммуникаций в Microsoft Graph
description: API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования функций голоса и видео.
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 1f20413fe905cbbfb4e007386ff852476e00a79f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871399"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="a7219-103">Работа с API коммуникаций в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a7219-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="a7219-104">API коммуникаций в Microsoft Graph добавляет новое измерение для взаимодействия приложений и служб с пользователями путем использования основных возможностей общения в приложениях и службах.</span><span class="sxs-lookup"><span data-stu-id="a7219-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="a7219-105">Этот API можно использовать для создания и приема звонков, а также для создания и получения координат собраний.</span><span class="sxs-lookup"><span data-stu-id="a7219-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="a7219-106">API коммуникаций можно использовать для создания служебных приложений (ботов), выполняющих роль участников в звонке, а также создающих собрания и получающих приглашения на них от имени пользователей.</span><span class="sxs-lookup"><span data-stu-id="a7219-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="a7219-107">Этот API предоставляет функции звонков, а также возможность создавать собрания по сети и получать приглашения на них.</span><span class="sxs-lookup"><span data-stu-id="a7219-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="a7219-108">С помощью этого API можно использовать служебные приложения (боты), при этом боты могут участвовать в звонках VoIP или собраниях Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a7219-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="a7219-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7219-109">Authorization</span></span>

<span data-ttu-id="a7219-110">Для доступа к API коммуникаций требуется одно из указанных ниже [разрешений](https://docs.microsoft.com/graph/permissions-reference#calls-permissions).</span><span class="sxs-lookup"><span data-stu-id="a7219-110">One of the following [permissions](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="a7219-111">Эти разрешения должны предоставляться администратором</span><span class="sxs-lookup"><span data-stu-id="a7219-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="a7219-112">Сценарий</span><span class="sxs-lookup"><span data-stu-id="a7219-112">Scenario</span></span>                 | <span data-ttu-id="a7219-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7219-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="a7219-114">Звонки</span><span class="sxs-lookup"><span data-stu-id="a7219-114">Calling</span></span>                 | <span data-ttu-id="a7219-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a7219-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="a7219-116">Собрания</span><span class="sxs-lookup"><span data-stu-id="a7219-116">Meetings</span></span>                 | <span data-ttu-id="a7219-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7219-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="a7219-118">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="a7219-118">Common use cases</span></span>

<span data-ttu-id="a7219-119">В таблице ниже перечислены некоторые распространенные варианты использования API коммуникаций.</span><span class="sxs-lookup"><span data-stu-id="a7219-119">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="a7219-120">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="a7219-120">Use cases</span></span>                         | <span data-ttu-id="a7219-121">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="a7219-121">REST resources</span></span>                                 | <span data-ttu-id="a7219-122">См. также</span><span class="sxs-lookup"><span data-stu-id="a7219-122">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="a7219-123">Создание приватных и групповых звонков, а также присоединение к ним</span><span class="sxs-lookup"><span data-stu-id="a7219-123">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="a7219-124">Звонок</span><span class="sxs-lookup"><span data-stu-id="a7219-124">Call</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="a7219-125">Методы звонков</span><span class="sxs-lookup"><span data-stu-id="a7219-125">Methods for calls</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="a7219-126">Звонки с интерактивным речевым взаимодействием</span><span class="sxs-lookup"><span data-stu-id="a7219-126">IVR calls</span></span>   |     | [<span data-ttu-id="a7219-127">Методы для интерактивного речевого взаимодействия</span><span class="sxs-lookup"><span data-stu-id="a7219-127">Methods for IVR</span></span>](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="a7219-128">Элементы управления звонком (участник)</span><span class="sxs-lookup"><span data-stu-id="a7219-128">Call controls (participant)</span></span> | [<span data-ttu-id="a7219-129">Участник</span><span class="sxs-lookup"><span data-stu-id="a7219-129">Participant</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="a7219-130">Собрания</span><span class="sxs-lookup"><span data-stu-id="a7219-130">Meetings</span></span>|[<span data-ttu-id="a7219-131">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a7219-131">onlineMeeting</span></span>](https://docs.microsoft.comgraph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="a7219-132">Методы для собраний</span><span class="sxs-lookup"><span data-stu-id="a7219-132">Methods for meetings</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|

## <a name="common-properties"></a><span data-ttu-id="a7219-133">Общие свойства</span><span class="sxs-lookup"><span data-stu-id="a7219-133">Common properties</span></span>

| <span data-ttu-id="a7219-134">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a7219-134">Resource</span></span>                | <span data-ttu-id="a7219-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7219-135">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="a7219-136">call</span><span class="sxs-lookup"><span data-stu-id="a7219-136">call</span></span>                               | [<span data-ttu-id="a7219-137">свойства объекта call</span><span class="sxs-lookup"><span data-stu-id="a7219-137">call properties</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="a7219-138">participant</span><span class="sxs-lookup"><span data-stu-id="a7219-138">participant</span></span>                         | [<span data-ttu-id="a7219-139">свойства объекта participant</span><span class="sxs-lookup"><span data-stu-id="a7219-139">participant properties</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="a7219-140">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a7219-140">onlineMeeting</span></span>                            | [<span data-ttu-id="a7219-141">свойства объекта onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a7219-141">onlineMeeting properties</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |

## <a name="see-also"></a><span data-ttu-id="a7219-142">См. также</span><span class="sxs-lookup"><span data-stu-id="a7219-142">See also</span></span>

- [<span data-ttu-id="a7219-143">Примеры API коммуникаций</span><span class="sxs-lookup"><span data-stu-id="a7219-143">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="a7219-144">Пакет SDK для передачи сигналов коммуникаций</span><span class="sxs-lookup"><span data-stu-id="a7219-144">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="a7219-145">Пакет SDK мультимедиа коммуникаций</span><span class="sxs-lookup"><span data-stu-id="a7219-145">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)
