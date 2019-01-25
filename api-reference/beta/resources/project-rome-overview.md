---
title: 'Использование Microsoft Graph API для работы с Project рим '
description: 'Проект рим является корпорации Майкрософт для построения на платформе, что позволяет разработчикам создавать между устройствами возможностей приложения. Рим Project позволяет различных возможностей, если пользователь выполнит с одной Microsoft учетной записи или работы или школе учетной записи подключиться различных служб и конечные точки клиентов. Это позволяет реализовать взаимодействия между устройствами и кроссплатформенный центральным задач пользователя, а не устройств. '
localization_priority: Normal
ms.openlocfilehash: 57c5189f3caf64ec048d000d5e9108811bd88145
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509695"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="4706e-105">Использование Microsoft Graph API для работы с Project рим</span><span class="sxs-lookup"><span data-stu-id="4706e-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4706e-106">[Проект рим](https://developer.microsoft.com/en-us/windows/project-rome) является корпорации Майкрософт для построения на платформе, что позволяет разработчикам создавать между устройствами возможностей приложения.</span><span class="sxs-lookup"><span data-stu-id="4706e-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="4706e-107">Рим Project позволяет различных возможностей, если пользователь выполнит с одной Microsoft учетной записи или работы или школе учетной записи подключиться различных служб и конечные точки клиентов.</span><span class="sxs-lookup"><span data-stu-id="4706e-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="4706e-108">Это позволяет реализовать взаимодействия между устройствами и кроссплатформенный центральным задач пользователя, а не устройств.</span><span class="sxs-lookup"><span data-stu-id="4706e-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="4706e-109">Три основные возможности рим проекта, предоставляемые посредством Microsoft Graph, чтобы обеспечить возможностей между устройствами: действия, устройств и уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4706e-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="4706e-110">Действия</span><span class="sxs-lookup"><span data-stu-id="4706e-110">Activities</span></span>

<span data-ttu-id="4706e-111">Действия в Microsoft Graph включается для оказания пользователя диск с приложениями между устройствами и платформами.</span><span class="sxs-lookup"><span data-stu-id="4706e-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="4706e-112">Действие — это единица пользовательского сотрудничества и состоит из трех компонентов:</span><span class="sxs-lookup"><span data-stu-id="4706e-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="4706e-113">Прямая ссылка</span><span class="sxs-lookup"><span data-stu-id="4706e-113">A deep link</span></span>
- <span data-ttu-id="4706e-114">Визуальное представление</span><span class="sxs-lookup"><span data-stu-id="4706e-114">A visual representation</span></span>
- <span data-ttu-id="4706e-115">Метаданные контента, описывающий действия, с помощью [https://schema.org/](https://schema.org/) общих словаря</span><span class="sxs-lookup"><span data-stu-id="4706e-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="4706e-116">При создании сеанса в приложении, элемент журнала добавляется активности в соответствии с период участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="4706e-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="4706e-117">Каждый раз, пользователь reengages с действием, новый элемент журнала добавляется активности начисления участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="4706e-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="4706e-118">При приложения публикует объекты действия пользователя, объект будет отображаться в некоторых новых поверхности пользовательского интерфейса в Windows; Например Cortana уведомления и временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="4706e-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="4706e-119">Можно указать расширенном метаданных (разрешено действия представления в только что правом контекст) и расширенными возможностями визуальные элементы (с помощью разметки [Адаптивный карточки](https://adaptivecards.io/) ) в объектах активности.</span><span class="sxs-lookup"><span data-stu-id="4706e-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="4706e-120">Следующие интерфейсы API Microsoft Graph можно использовать для создания и получения работу пользователей:</span><span class="sxs-lookup"><span data-stu-id="4706e-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="4706e-121">Создать или заменить активности</span><span class="sxs-lookup"><span data-stu-id="4706e-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="4706e-122">Получение действий</span><span class="sxs-lookup"><span data-stu-id="4706e-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="4706e-123">Получение последних действий</span><span class="sxs-lookup"><span data-stu-id="4706e-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="4706e-124">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="4706e-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="4706e-125">Создание или замена элемента журнала</span><span class="sxs-lookup"><span data-stu-id="4706e-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="4706e-126">Удаление элемента журнала</span><span class="sxs-lookup"><span data-stu-id="4706e-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="4706e-127">Устройства</span><span class="sxs-lookup"><span data-stu-id="4706e-127">Devices</span></span>

<span data-ttu-id="4706e-128">API-интерфейсы рим проекта можно использовать в Microsoft Graph для:</span><span class="sxs-lookup"><span data-stu-id="4706e-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="4706e-129">Обнаружение и подключитесь к устройствам пользователя</span><span class="sxs-lookup"><span data-stu-id="4706e-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="4706e-130">Удаленно запуска приложений на этих устройств</span><span class="sxs-lookup"><span data-stu-id="4706e-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="4706e-131">Отправлять сообщения в ваши приложения на эти устройства</span><span class="sxs-lookup"><span data-stu-id="4706e-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="4706e-132">С помощью этих интерфейсов API можно создавать приложения, которые Создание мультимедиа, которые необычный одно устройство.</span><span class="sxs-lookup"><span data-stu-id="4706e-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="4706e-133">Например можно расширить ваше приложение для запуска на экране.</span><span class="sxs-lookup"><span data-stu-id="4706e-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="4706e-134">Или можно создать взаимодействия компаньона для приложения на основе другого пользователя устройств.</span><span class="sxs-lookup"><span data-stu-id="4706e-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="4706e-135">Следующие интерфейсы API Microsoft Graph можно использовать для связи с другими устройствами Windows:</span><span class="sxs-lookup"><span data-stu-id="4706e-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="4706e-136">Список устройств пользователя</span><span class="sxs-lookup"><span data-stu-id="4706e-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="4706e-137">Отправить команду на устройство</span><span class="sxs-lookup"><span data-stu-id="4706e-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="4706e-138">Получение состояния команды</span><span class="sxs-lookup"><span data-stu-id="4706e-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="4706e-139">Уведомления</span><span class="sxs-lookup"><span data-stu-id="4706e-139">Notifications</span></span>

<span data-ttu-id="4706e-140">Уведомления о API-интерфейсы можно использовать в Microsoft Graph для доставки уведомлений через несколько конечных точек, и тот же пользователь вход на.</span><span class="sxs-lookup"><span data-stu-id="4706e-140">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="4706e-141">Пользователя можно распределять непосредственно при учете уведомлений вместо причинят адреса/каналов устройств.</span><span class="sxs-lookup"><span data-stu-id="4706e-141">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="4706e-142">Таким образом, можно сосредоточиться на проектировании сценарии правом уведомлений в human ориентированных, а не ориентированный на устройстве способом.</span><span class="sxs-lookup"><span data-stu-id="4706e-142">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="4706e-143">Можно опубликовать уведомление о необработанных данных или прямой visual уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4706e-143">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="4706e-144">При доставке необработанные данные уведомления в конечной точки устройства, затем воспользуйтесь [SDK клиента](https://github.com/Microsoft/project-rome) (Microsoft Graph уведомления пакет SDK для Windows SDK рим проекта для iOS и Android) для получения и управление уведомлениями.</span><span class="sxs-lookup"><span data-stu-id="4706e-144">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="4706e-145">При прямой Визуальное уведомление о доставке в конечной точки устройства, теперь показаны собственного уведомления платформы для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4706e-145">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="4706e-146">Дополнительные сведения см [создания и отправки уведомлений](../api/projectrome-notification-post.md).</span><span class="sxs-lookup"><span data-stu-id="4706e-146">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/project-rome-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
