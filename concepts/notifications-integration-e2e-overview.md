---
title: 'Интеграция с уведомлениями Microsoft Graph '
description: 'Уведомления — один из наиболее эффективных способов взаимодействия с пользователями вашего приложения. Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий.  '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 3cbeedfae4e47ac388b60d150505e247534ee68a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939579"
---
# <a name="integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="8183f-104">Интеграция с уведомлениями Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8183f-104">Integrate with Microsoft Graph notifications</span></span>

<span data-ttu-id="8183f-105">Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий, как показано на следующей схеме.</span><span class="sxs-lookup"><span data-stu-id="8183f-105">You can integrate your apps with Microsoft Graph notifications with a few simple steps, as shown in the following diagram.</span></span>

![Изображение действий по внедрению уведомлений: регистрация, внедрение использования разных устройств, серверная интеграция и интеграция с клиентскими программами](images/notifications-integration-e2e-overview.png)

1.  <span data-ttu-id="8183f-107">[Зарегистрируйте](notifications-integration-app-registration.md) свое приложение на портале Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="8183f-107">[Register](notifications-integration-app-registration.md) your application in the Microsoft Azure portal.</span></span>

2. <span data-ttu-id="8183f-108">[Подключитесь](notifications-integration-cross-device-experiences-onboarding.md) к Центру партнеров или Центру разработки для Windows, чтобы получить удостоверение кроссплатформенного приложения и учетные данные push-уведомлений для Windows, iOS и Android.</span><span class="sxs-lookup"><span data-stu-id="8183f-108">[Onboard](notifications-integration-cross-device-experiences-onboarding.md) to Partner Center/Windows Dev Center for cross-platform application identity and push notification credentials.</span></span>

3.  <span data-ttu-id="8183f-109">[Настройте свой сервер приложений](notifications-integrating-app-server.md) для отправки уведомлений через Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8183f-109">[Set up your app server](notifications-integrating-app-server.md) to send notifications via Microsoft Graph.</span></span>

4.  <span data-ttu-id="8183f-110">[Интегрируйте](notifications-integrating-with-windows.md) новый [пакет SDK клиента уведомлений](https://aka.ms/GNSDK) в клиенты приложений для Windows, iOS, Android или веб-клиенты, чтобы получать уведомления и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="8183f-110">[Integrate](notifications-integrating-with-windows.md) the [Microsoft Graph notifications client SDK](https://aka.ms/GNSDK) into your Windows, Android, or iOS app clients to receive and manage notifications.</span></span>

> [!NOTE]
> <span data-ttu-id="8183f-111">Рекомендуем использовать новый, улучшенный и компактный [пакет SDK уведомлений](https://aka.ms/GNSDK) вместо [пакета SDK Project Rome](https://github.com/microsoft/project-rome) для различных устройств.</span><span class="sxs-lookup"><span data-stu-id="8183f-111">We recommend using the new and improved, lightweight [notification SDK](https://aka.ms/GNSDK) instead of the cross-device [Project Rome SDK](https://github.com/microsoft/project-rome).</span></span>
