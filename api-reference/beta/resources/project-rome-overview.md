---
title: 'Использование API Microsoft Graph для работы с проектом Рим '
description: 'Проект Рим — это инициатива Майкрософт по созданию платформы, позволяющей разработчикам приложений создавать удобные возможности для различных устройств. Проект Рим включает различные возможности, соединяющие различные службы и клиентские конечные точки, когда пользователь входит с помощью одной учетной записи Майкрософт или рабочей или учебной учетной записи. Это позволяет реализовать межустройство и межплатформенные интерфейсы, которые центрируются вокруг задач пользователя, а не для устройств. '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbec95682b552210781ecd7390726f8d92c4aa03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965623"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="8e6c1-105">Использование API Microsoft Graph для работы с проектом Рим</span><span class="sxs-lookup"><span data-stu-id="8e6c1-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e6c1-106">[Проект Рим](https://developer.microsoft.com/en-us/windows/project-rome) — это инициатива Майкрософт по созданию платформы, позволяющей разработчикам приложений создавать удобные возможности для различных устройств.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="8e6c1-107">Проект Рим включает различные возможности, соединяющие различные службы и клиентские конечные точки, когда пользователь входит с помощью одной учетной записи Майкрософт или рабочей или учебной учетной записи.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="8e6c1-108">Это позволяет реализовать межустройство и межплатформенные интерфейсы, которые центрируются вокруг задач пользователя, а не для устройств.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="8e6c1-109">Три ключевых возможности проекта, которые можно получить с помощью Microsoft Graph, чтобы обеспечить удобство взаимодействия между устройствами: действия, устройства и уведомления.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="8e6c1-110">Действия</span><span class="sxs-lookup"><span data-stu-id="8e6c1-110">Activities</span></span>

<span data-ttu-id="8e6c1-111">Действия в Microsoft Graph позволяют обеспечить участие пользователей в приложениях на различных устройствах и платформах.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="8e6c1-112">Действие является единицей задействования пользователя и состоит из трех компонентов:</span><span class="sxs-lookup"><span data-stu-id="8e6c1-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="8e6c1-113">Глубокая ссылка</span><span class="sxs-lookup"><span data-stu-id="8e6c1-113">A deep link</span></span>
- <span data-ttu-id="8e6c1-114">Визуальное представление</span><span class="sxs-lookup"><span data-stu-id="8e6c1-114">A visual representation</span></span>
- <span data-ttu-id="8e6c1-115">Метаданные контента, описывающие действие, с использованием [https://schema.org/](https://schema.org/) общего словаря</span><span class="sxs-lookup"><span data-stu-id="8e6c1-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="8e6c1-116">При создании сеанса приложением в действие добавляется элемент History, отражающий период участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="8e6c1-117">Каждый раз, когда пользователь переносит действие, для начисления задействования пользователей добавляется новый элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="8e6c1-118">Когда приложение публикует объекты действий пользователя, объект будет отображаться в некоторых новых поверхностях пользовательского интерфейса в Windows; Например, уведомления и шкала времени Кортаны.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="8e6c1-119">Вы можете указать как расширенные метаданные (чтобы отображать действия только в правильном контексте), так и визуальные элементы (с использованием разметки [адаптивной карточки](https://adaptivecards.io/) ) в объектах действий.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="8e6c1-120">Для создания и извлечения действий пользователей можно использовать следующие API Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8e6c1-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="8e6c1-121">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="8e6c1-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="8e6c1-122">Получение действий</span><span class="sxs-lookup"><span data-stu-id="8e6c1-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="8e6c1-123">Получение последних действий</span><span class="sxs-lookup"><span data-stu-id="8e6c1-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="8e6c1-124">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="8e6c1-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="8e6c1-125">Создание или замена элемента журнала</span><span class="sxs-lookup"><span data-stu-id="8e6c1-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="8e6c1-126">Удаление элемента журнала</span><span class="sxs-lookup"><span data-stu-id="8e6c1-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="8e6c1-127">Устройства</span><span class="sxs-lookup"><span data-stu-id="8e6c1-127">Devices</span></span>

<span data-ttu-id="8e6c1-128">С помощью API Project Рим в Microsoft Graph можно выполнять следующие задачи:</span><span class="sxs-lookup"><span data-stu-id="8e6c1-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="8e6c1-129">Обнаружение устройств пользователя и подключение к ним</span><span class="sxs-lookup"><span data-stu-id="8e6c1-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="8e6c1-130">Удаленный запуск приложений на этих устройствах</span><span class="sxs-lookup"><span data-stu-id="8e6c1-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="8e6c1-131">Отправка сообщений приложениям на этих устройствах</span><span class="sxs-lookup"><span data-stu-id="8e6c1-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="8e6c1-132">С помощью этих API вы можете создавать приложения, которые создают полнофункциональные возможности для отдельного устройства.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="8e6c1-133">Например, вы можете расширить приложение для запуска на более крупном экране.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="8e6c1-134">Кроме того, вы можете создать вспомогательный интерфейс для приложения на другом устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e6c1-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="8e6c1-135">Для общения с другими устройствами Windows можно использовать следующие API Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8e6c1-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="8e6c1-136">Перечисление устройств пользователя</span><span class="sxs-lookup"><span data-stu-id="8e6c1-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="8e6c1-137">Отправка команды устройству</span><span class="sxs-lookup"><span data-stu-id="8e6c1-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="8e6c1-138">Получение состояния команды</span><span class="sxs-lookup"><span data-stu-id="8e6c1-138">Get command status</span></span>](../api/get-device-command-status.md)

