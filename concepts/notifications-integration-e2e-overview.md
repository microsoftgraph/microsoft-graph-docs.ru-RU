---
title: 'Интеграция с уведомлениями Microsoft Graph '
description: 'Уведомления — один из наиболее эффективных способов взаимодействия с пользователями вашего приложения. Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий.  '
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: 8d3e2fe8d7c208cd2c4f0c7f55ba68a79a3d3713
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066907"
---
# <a name="integrate-with-microsoft-graph-notifications"></a>Интеграция с уведомлениями Microsoft Graph

Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий, как показано на следующей схеме.

![Изображение действий по внедрению уведомлений: регистрация, внедрение использования разных устройств, серверная интеграция и интеграция с клиентскими программами](images/notifications-integration-e2e-overview.png)

1.  [Зарегистрируйте](notifications-integration-app-registration.md) свое приложение на портале Microsoft Azure.

2. [Подключитесь](notifications-integration-cross-device-experiences-onboarding.md) к Центру партнеров или Центру разработки для Windows, чтобы получить удостоверение кроссплатформенного приложения и учетные данные push-уведомлений для Windows, iOS и Android.

3.  [Настройте свой сервер приложений](notifications-integrating-app-server.md) для отправки уведомлений через Microsoft Graph.

4.  [Интегрируйте](notifications-integrating-with-windows.md) новый [пакет SDK клиента уведомлений](https://aka.ms/GNSDK) в клиенты приложений для Windows, iOS, Android или веб-клиенты, чтобы получать уведомления и управлять ими.

> [!NOTE]
> Рекомендуем использовать новый, улучшенный и компактный [пакет SDK уведомлений](https://aka.ms/GNSDK) вместо [пакета SDK Project Rome](https://github.com/microsoft/project-rome) для различных устройств.
