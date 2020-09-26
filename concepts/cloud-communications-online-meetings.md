---
title: Создание онлайн-встреч и присоединение к ним с помощью API облачных коммуникаций
description: У вас есть гибкие возможности для создания будущих или сиюминутных собраний.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 08d7195f3eb91ba896e8045b4576e46f12aaf795
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289353"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a><span data-ttu-id="ffd7b-103">Создание онлайн-встреч и присоединение к ним с помощью API облачных коммуникаций</span><span class="sxs-lookup"><span data-stu-id="ffd7b-103">Use the cloud communications API to create or join online meetings</span></span>

<span data-ttu-id="ffd7b-104">В собраниях по сети предоставляется возможность указать определенные сведения, например тему собрания, и всех участников.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-104">Online meetings provide the ability to specify certain details, such as the subject of the meeting, and who all the attendees are.</span></span> <span data-ttu-id="ffd7b-105">Вы также можете задать дату и время начала и окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-105">You can also set the date and time for when the meeting starts and ends.</span></span>

<span data-ttu-id="ffd7b-106">Собрания по сети обеспечивают гибкость при создании собрания, выполняемого в будущем или мгновенно.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-106">Online meetings provide the flexibility to create a meeting that takes place in the future, or instantaneously.</span></span> <span data-ttu-id="ffd7b-107">Возможность настроить собрание, запускаемые сразу же после его создания, идеально подходит для неожиданных проблем и других инцидентов, требующих немедленного внимания участников.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-107">The ability to set up a meeting that starts immediately after it is created is ideal for unexpected issues and other incidents that require the immediate attention of the attendees.</span></span>

> <span data-ttu-id="ffd7b-108">**Note (Примечание** ) Этот набор интерфейсов API обеспечивает гибкость и расширенную интеграцию с функциями Microsoft Teams или Skype; Он не обновляет или не создает события в календаре.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-108">**Note** This set of APIs allows the flexibility and richer integration with Microsoft Teams or Skype capabilities; it does not update or create any event in a calendar.</span></span> <span data-ttu-id="ffd7b-109">Чтобы получить удобный способ добавить собрание по сети в календарь Outlook, используйте API календаря.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-109">For a convenient approach to add an online meeting to an Outlook calendar, use the calendar API.</span></span> <span data-ttu-id="ffd7b-110">Дополнительные сведения см. в статье [Выбор API в Microsoft Graph для создания собраний по сети и присоединения к ним](choose-online-meeting-api.md).</span><span class="sxs-lookup"><span data-stu-id="ffd7b-110">See [Choose an API in Microsoft Graph to create and join online meetings](choose-online-meeting-api.md) for more information.</span></span>

## <a name="create-an-online-meeting"></a><span data-ttu-id="ffd7b-111">Создание собрания по сети</span><span class="sxs-lookup"><span data-stu-id="ffd7b-111">Create an online meeting</span></span>

<span data-ttu-id="ffd7b-112">При создании собрания по сети вы получите [координаты](/graph/api/resources/onlinemeeting) собрания.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-112">When you create an online meeting, you'll receive [coordinates](/graph/api/resources/onlinemeeting) for the meeting.</span></span> <span data-ttu-id="ffd7b-113">Когда участники присоединяются к собранию с помощью этих координат, создается групповой вызов.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-113">When participants join the meeting using these meeting coordinates, a group call is created.</span></span>

<span data-ttu-id="ffd7b-114">Когда все участники покидают групповой вызов, вызов группы будет завершен.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-114">When all the participants leave the group call, the group call will end.</span></span> <span data-ttu-id="ffd7b-115">Участники все еще могут повторно присоединиться к собранию, используя те же координаты собрания, но при этом будет создан еще один вызов группы.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-115">Participants can still rejoin the meeting afterward using the same meeting coordinates, but this will create another group call.</span></span>

><span data-ttu-id="ffd7b-116">**Примечание:** Созданные собрания не отображаются в календарях.</span><span class="sxs-lookup"><span data-stu-id="ffd7b-116">**Note:** The created meetings do not appear on calendars.</span></span>

## <a name="join-an-online-meeting"></a><span data-ttu-id="ffd7b-117">Присоединение к собранию по сети</span><span class="sxs-lookup"><span data-stu-id="ffd7b-117">Join an online meeting</span></span>
<span data-ttu-id="ffd7b-118">После создания собрания по сети пользователи могут присоединиться двумя способами:</span><span class="sxs-lookup"><span data-stu-id="ffd7b-118">After an online meeting is created, users can join in two ways:</span></span>

1. <span data-ttu-id="ffd7b-119">Через браузер, используя **жоинвебурл** , возвращенный в составе [координат собрания](/graph/api/resources/onlinemeeting).</span><span class="sxs-lookup"><span data-stu-id="ffd7b-119">Through the browser, using the **joinWebURL** that was returned as part of the [meeting coordinates](/graph/api/resources/onlinemeeting).</span></span>

2. <span data-ttu-id="ffd7b-120">С помощью [API создания вызовов](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), для которого необходимо предоставить [координаты собрания](/graph/api/resources/onlinemeeting)([организермитингинфо](/graph/api/resources/organizermeetinginfo)и [чатинфо](/graph/api/resources/chatinfo)).</span><span class="sxs-lookup"><span data-stu-id="ffd7b-120">Through the [create call API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), which requires that you provide the [meeting coordinates](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo), and [chatInfo](/graph/api/resources/chatinfo)).</span></span>

## <a name="see-also"></a><span data-ttu-id="ffd7b-121">См. также</span><span class="sxs-lookup"><span data-stu-id="ffd7b-121">See also</span></span>

- [<span data-ttu-id="ffd7b-122">Разрешения для собраний по сети</span><span class="sxs-lookup"><span data-stu-id="ffd7b-122">Online meeting permissions</span></span>](./permissions-reference.md#online-meetings-permissions)
- [<span data-ttu-id="ffd7b-123">Выбор API в Microsoft Graph для создания собраний по сети и присоединения к ним</span><span class="sxs-lookup"><span data-stu-id="ffd7b-123">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)