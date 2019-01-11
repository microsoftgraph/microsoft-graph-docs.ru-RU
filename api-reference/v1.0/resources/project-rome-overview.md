---
title: Использование Microsoft Graph API для работы с Project рим
description: Проект рим — корпорации Майкрософт для построения между устройствами среды взаимодействия с пользователем платформы. При входе пользователя с помощью ту же учетную запись Майкрософт, которой они выполняют вход на клиентском устройстве рим Project позволяет приложения на локальном клиента или службы для взаимодействия с приложениями и службы на удаленном компьютере. Это позволяет взаимодействия между устройствами и кроссплатформенный программы, центральным задач пользователя, а не устройств.
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840966"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="d3a02-105">Использование Microsoft Graph API для работы с Project рим</span><span class="sxs-lookup"><span data-stu-id="d3a02-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="d3a02-106">[Проект рим](https://developer.microsoft.com/en-us/windows/project-rome) — корпорации Майкрософт для построения между устройствами среды взаимодействия с пользователем платформы.</span><span class="sxs-lookup"><span data-stu-id="d3a02-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="d3a02-107">При входе пользователя с помощью ту же учетную запись Майкрософт, которой они выполняют вход на клиентском устройстве рим Project позволяет приложения на локальном клиента или службы для взаимодействия с приложениями и службы на удаленном компьютере.</span><span class="sxs-lookup"><span data-stu-id="d3a02-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="d3a02-108">Это позволяет взаимодействия между устройствами и кроссплатформенный программы, центральным задач пользователя, а не устройств.</span><span class="sxs-lookup"><span data-stu-id="d3a02-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="d3a02-109">Ключевой компонент доступен через Microsoft Graph для включения этих функций: действия.</span><span class="sxs-lookup"><span data-stu-id="d3a02-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="d3a02-110">Действия</span><span class="sxs-lookup"><span data-stu-id="d3a02-110">Activities</span></span>

<span data-ttu-id="d3a02-111">Действия в Microsoft Graph включается для оказания пользователя диск с приложениями между устройствами и платформами.</span><span class="sxs-lookup"><span data-stu-id="d3a02-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="d3a02-112">Действие — это единица пользовательского сотрудничества и состоит из трех компонентов:</span><span class="sxs-lookup"><span data-stu-id="d3a02-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="d3a02-113">Прямая ссылка</span><span class="sxs-lookup"><span data-stu-id="d3a02-113">A deep link</span></span>
- <span data-ttu-id="d3a02-114">Визуальное представление</span><span class="sxs-lookup"><span data-stu-id="d3a02-114">A visual representation</span></span>
- <span data-ttu-id="d3a02-115">Метаданные контента, описывающий действия, с помощью [https://schema.org/](https://schema.org/) общих словаря</span><span class="sxs-lookup"><span data-stu-id="d3a02-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="d3a02-116">При создании сеанса в приложении, элемент журнала добавляется активности в соответствии с период участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3a02-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="d3a02-117">Каждый раз, пользователь reengages с действием, новый элемент журнала добавляется активности начисления участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3a02-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="d3a02-118">При приложения публикует объекты действия пользователя, объект будет отображаться в некоторых новых поверхности пользовательского интерфейса в Windows; Например Cortana уведомления и временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="d3a02-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="d3a02-119">Можно указать расширенном метаданных (разрешено действия представления в только что правом контекст) и расширенными возможностями визуальные элементы (с помощью разметки [Адаптивный карточки](https://adaptivecards.io/) ) в объектах активности.</span><span class="sxs-lookup"><span data-stu-id="d3a02-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="d3a02-120">Следующие интерфейсы API Microsoft Graph можно использовать для создания и получения работу пользователей:</span><span class="sxs-lookup"><span data-stu-id="d3a02-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="d3a02-121">Создать или заменить активности</span><span class="sxs-lookup"><span data-stu-id="d3a02-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="d3a02-122">Получение действий</span><span class="sxs-lookup"><span data-stu-id="d3a02-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="d3a02-123">Получение последних действий</span><span class="sxs-lookup"><span data-stu-id="d3a02-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="d3a02-124">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="d3a02-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="d3a02-125">Создание или замена элемента журнала</span><span class="sxs-lookup"><span data-stu-id="d3a02-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="d3a02-126">Удаление элемента журнала</span><span class="sxs-lookup"><span data-stu-id="d3a02-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

