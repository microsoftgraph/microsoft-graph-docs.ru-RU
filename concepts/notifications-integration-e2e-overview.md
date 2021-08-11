---
title: 'Интеграция с уведомлениями Microsoft Graph '
description: 'Уведомления — один из наиболее эффективных способов взаимодействия с пользователями вашего приложения. Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий.  '
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 8dc5ef886106ca4d966e0a94ae2915040cfb5d1f1ea66d041d136db5bb7951e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149534"
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
