---
title: Использование API облачных коммуникаций для создания собраний по сети или присоединения к ним
description: У вас будет возможность создать собрание, которое будет выполняться в будущем или мгновенно
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 22d44c32b6ece847283f2e572eeaf468eaac3dbe
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289643"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a><span data-ttu-id="09964-103">Использование API облачных коммуникаций для создания собраний по сети или присоединения к ним</span><span class="sxs-lookup"><span data-stu-id="09964-103">Use the cloud communications API to create or join online meetings</span></span>

<span data-ttu-id="09964-104">В собраниях по сети предоставляется возможность указать определенные сведения, например тему собрания, и всех участников.</span><span class="sxs-lookup"><span data-stu-id="09964-104">Online meetings provide the ability to specify certain details, such as the subject of the meeting, and who all the attendees are.</span></span> <span data-ttu-id="09964-105">Вы также можете задать дату и время начала и окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="09964-105">You can also set the date and time for when the meeting starts and ends.</span></span>

<span data-ttu-id="09964-106">Собрания по сети обеспечивают гибкость при создании собрания, выполняемого в будущем или мгновенно.</span><span class="sxs-lookup"><span data-stu-id="09964-106">Online meetings provide the flexibility to create a meeting that takes place in the future, or instantaneously.</span></span> <span data-ttu-id="09964-107">Возможность настроить собрание, запускаемые сразу же после его создания, идеально подходит для неожиданных проблем и других инцидентов, требующих немедленного внимания участников.</span><span class="sxs-lookup"><span data-stu-id="09964-107">The ability to set up a meeting that starts immediately after it is created is ideal for unexpected issues and other incidents that require the immediate attention of the attendees.</span></span>

## <a name="create-an-online-meeting"></a><span data-ttu-id="09964-108">Создание собрания по сети</span><span class="sxs-lookup"><span data-stu-id="09964-108">Create an online meeting</span></span>

<span data-ttu-id="09964-109">При создании собрания по сети вы получите [координаты](/graph/api/resources/onlinemeeting) собрания.</span><span class="sxs-lookup"><span data-stu-id="09964-109">When you create an online meeting, you'll receive [coordinates](/graph/api/resources/onlinemeeting) for the meeting.</span></span> <span data-ttu-id="09964-110">Когда участники присоединяются к собранию с помощью этих координат, создается групповой вызов.</span><span class="sxs-lookup"><span data-stu-id="09964-110">When participants join the meeting using these meeting coordinates, a group call is created.</span></span>

<span data-ttu-id="09964-111">Когда все участники покидают групповой вызов, вызов группы будет завершен.</span><span class="sxs-lookup"><span data-stu-id="09964-111">When all the participants leave the group call, the group call will end.</span></span> <span data-ttu-id="09964-112">Участники все еще могут повторно присоединиться к собранию, используя те же координаты собрания, но при этом будет создан еще один вызов группы.</span><span class="sxs-lookup"><span data-stu-id="09964-112">Participants can still rejoin the meeting afterward using the same meeting coordinates, but this will create another group call.</span></span>

><span data-ttu-id="09964-113">**Примечание:** Созданные собрания не отображаются в календарях.</span><span class="sxs-lookup"><span data-stu-id="09964-113">**Note:** The created meetings do not appear on calendars.</span></span>

## <a name="join-an-online-meeting"></a><span data-ttu-id="09964-114">Присоединение к собранию по сети</span><span class="sxs-lookup"><span data-stu-id="09964-114">Join an online meeting</span></span>
<span data-ttu-id="09964-115">После создания собрания по сети пользователи могут присоединиться двумя способами:</span><span class="sxs-lookup"><span data-stu-id="09964-115">After an online meeting is created, users can join in two ways:</span></span>

1. <span data-ttu-id="09964-116">Через браузер, используя **жоинвебурл** , возвращенный в составе [координат собрания](/graph/api/resources/onlinemeeting).</span><span class="sxs-lookup"><span data-stu-id="09964-116">Through the browser, using the **joinWebURL** that was returned as part of the [meeting coordinates](/graph/api/resources/onlinemeeting).</span></span>

2. <span data-ttu-id="09964-117">С помощью [API создания вызовов](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), для которого необходимо предоставить [координаты собрания](/graph/api/resources/onlinemeeting)([организермитингинфо](/graph/api/resources/organizermeetinginfo)и [чатинфо](/graph/api/resources/chatinfo)).</span><span class="sxs-lookup"><span data-stu-id="09964-117">Through the [create call API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), which requires that you provide the [meeting coordinates](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo), and [chatInfo](/graph/api/resources/chatinfo)).</span></span>

## <a name="see-also"></a><span data-ttu-id="09964-118">См. также</span><span class="sxs-lookup"><span data-stu-id="09964-118">See also</span></span>

- [<span data-ttu-id="09964-119">Разрешения для собраний по сети</span><span class="sxs-lookup"><span data-stu-id="09964-119">Online meeting permissions</span></span>](/graph/permissions-reference#online-meetings-permissions)
- [<span data-ttu-id="09964-120">Выбор API в Microsoft Graph для создания собраний по сети и присоединения к ним</span><span class="sxs-lookup"><span data-stu-id="09964-120">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)
