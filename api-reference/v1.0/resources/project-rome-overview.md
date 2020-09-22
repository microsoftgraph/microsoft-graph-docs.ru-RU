---
title: Использование API Microsoft Graph для работы с проектом Рим
description: Проект Рим — это инициатива Майкрософт по созданию платформы взаимодействия между устройствами. Проект Рим позволяет приложению на локальном клиенте или в службе взаимодействовать с приложениями и службами на удаленном узле, когда пользователь входит с помощью учетной записи Майкрософт, которая используется для входа на клиентское устройство. Это позволяет программировать взаимодействие между устройствами и несколькими платформами, которые центрируются вокруг задач пользователя, а не для устройств.
localization_priority: Normal
author: ailae
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 945d3925362c6d013fa411d9b586bca18c8a24a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037208"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="8f60e-105">Использование API Microsoft Graph для работы с проектом Рим</span><span class="sxs-lookup"><span data-stu-id="8f60e-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="8f60e-106">[Проект Рим](https://developer.microsoft.com/en-us/windows/project-rome) — это инициатива Майкрософт по созданию платформы взаимодействия между устройствами.</span><span class="sxs-lookup"><span data-stu-id="8f60e-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="8f60e-107">Проект Рим позволяет приложению на локальном клиенте или в службе взаимодействовать с приложениями и службами на удаленном узле, когда пользователь входит с помощью учетной записи Майкрософт, которая используется для входа на клиентское устройство.</span><span class="sxs-lookup"><span data-stu-id="8f60e-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="8f60e-108">Это позволяет программировать взаимодействие между устройствами и несколькими платформами, которые центрируются вокруг задач пользователя, а не для устройств.</span><span class="sxs-lookup"><span data-stu-id="8f60e-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="8f60e-109">С помощью Microsoft Graph предоставляется ключевой компонент для поддержки таких возможностей: действия.</span><span class="sxs-lookup"><span data-stu-id="8f60e-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="8f60e-110">Действия</span><span class="sxs-lookup"><span data-stu-id="8f60e-110">Activities</span></span>

<span data-ttu-id="8f60e-111">Действия в Microsoft Graph позволяют обеспечить участие пользователей в приложениях на различных устройствах и платформах.</span><span class="sxs-lookup"><span data-stu-id="8f60e-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="8f60e-112">Действие является единицей задействования пользователя и состоит из трех компонентов:</span><span class="sxs-lookup"><span data-stu-id="8f60e-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="8f60e-113">Глубокая ссылка</span><span class="sxs-lookup"><span data-stu-id="8f60e-113">A deep link</span></span>
- <span data-ttu-id="8f60e-114">Визуальное представление</span><span class="sxs-lookup"><span data-stu-id="8f60e-114">A visual representation</span></span>
- <span data-ttu-id="8f60e-115">Метаданные контента, описывающие действие, с использованием [https://schema.org/](https://schema.org/) общего словаря</span><span class="sxs-lookup"><span data-stu-id="8f60e-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="8f60e-116">При создании сеанса приложением в действие добавляется элемент History, отражающий период участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f60e-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="8f60e-117">Каждый раз, когда пользователь переносит действие, для начисления задействования пользователей добавляется новый элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="8f60e-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="8f60e-118">Когда приложение публикует объекты действий пользователя, объект будет отображаться в некоторых новых поверхностях пользовательского интерфейса в Windows; Например, уведомления и шкала времени Кортаны.</span><span class="sxs-lookup"><span data-stu-id="8f60e-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="8f60e-119">Вы можете указать как расширенные метаданные (чтобы отображать действия только в правильном контексте), так и визуальные элементы (с использованием разметки [адаптивной карточки](https://adaptivecards.io/) ) в объектах действий.</span><span class="sxs-lookup"><span data-stu-id="8f60e-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="8f60e-120">Для создания и извлечения действий пользователей можно использовать следующие API Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8f60e-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="8f60e-121">Создание или замена действия</span><span class="sxs-lookup"><span data-stu-id="8f60e-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="8f60e-122">Получение действий</span><span class="sxs-lookup"><span data-stu-id="8f60e-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="8f60e-123">Получение последних действий</span><span class="sxs-lookup"><span data-stu-id="8f60e-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="8f60e-124">Удаление действия</span><span class="sxs-lookup"><span data-stu-id="8f60e-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="8f60e-125">Создание или замена элемента журнала</span><span class="sxs-lookup"><span data-stu-id="8f60e-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="8f60e-126">Удаление элемента журнала</span><span class="sxs-lookup"><span data-stu-id="8f60e-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a><span data-ttu-id="8f60e-127">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="8f60e-127">What's new</span></span>
<span data-ttu-id="8f60e-128">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="8f60e-128">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>
