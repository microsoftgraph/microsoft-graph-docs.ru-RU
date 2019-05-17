---
title: 'Интеграция с уведомлениями Microsoft Graph '
description: 'Уведомления — один из наиболее эффективных способов взаимодействия с пользователями вашего приложения. Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий.  '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 2f3a126ade92ff1615848f9f4db846aebb62d5f7
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063392"
---
# <a name="integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="01cbb-104">Интеграция с уведомлениями Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="01cbb-104">Integrate with Microsoft Graph notifications</span></span>

<span data-ttu-id="01cbb-105">Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий, как показано на следующей схеме.</span><span class="sxs-lookup"><span data-stu-id="01cbb-105">You can integrate your apps with Microsoft Graph notifications with a few simple steps, as shown in the following diagram.</span></span>

![Изображение действий по внедрению уведомлений: регистрация, внедрение использования разных устройств, серверная интеграция и интеграция с клиентскими программами](images/notifications-integration-e2e-overview.png)

1.  <span data-ttu-id="01cbb-107">[Зарегистрируйте](notifications-integration-app-registration.md) свое приложение на портале Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="01cbb-107"> Register a new application in the Azure portal</span></span>

2.  <span data-ttu-id="01cbb-108">[Подключитесь](notifications-integration-cross-device-experiences-onboarding.md) к Центру партнеров или Центру разработки для Windows, чтобы получить удостоверение кроссплатформенного приложения и учетные данные push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="01cbb-108">[Onboard](notifications-integration-cross-device-experiences-onboarding.md) to Partner Center/Windows Dev Center for cross-platform application identity and push notification credentials.</span></span>

3.  <span data-ttu-id="01cbb-109">[Настройте свой сервер приложений](notifications-integrating-app-server.md) для отправки уведомлений через Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="01cbb-109">[Set up your app server](notifications-integrating-app-server.md) to send notifications via Microsoft Graph.</span></span>

4.  <span data-ttu-id="01cbb-110">[Интегрируйте](notifications-integrating-with-windows.md) [пакет SDK клиента уведомлений Microsoft Graph](https://github.com/microsoft/project-rome) в клиенты приложений для Windows, Android или iOS, чтобы получать уведомления и управлять ими.</span><span class="sxs-lookup"><span data-stu-id="01cbb-110">[Integrate](notifications-integrating-with-windows.md) the [Microsoft Graph notifications client SDK](https://github.com/microsoft/project-rome) into your Windows, Android, or iOS app clients to receive and manage notifications.</span></span>
