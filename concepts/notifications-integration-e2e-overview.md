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
# <a name="integrate-with-microsoft-graph-notifications"></a>Интеграция с уведомлениями Microsoft Graph

Вы можете интегрировать в свои приложения уведомления Microsoft Graph с помощью нескольких простых действий, как показано на следующей схеме.

![Изображение действий по внедрению уведомлений: регистрация, внедрение использования разных устройств, серверная интеграция и интеграция с клиентскими программами](images/notifications-integration-e2e-overview.png)

1.  [Зарегистрируйте](notifications-integration-app-registration.md) свое приложение на портале Microsoft Azure.

2.  [Подключитесь](notifications-integration-cross-device-experiences-onboarding.md) к Центру партнеров или Центру разработки для Windows, чтобы получить удостоверение кроссплатформенного приложения и учетные данные push-уведомлений.

3.  [Настройте свой сервер приложений](notifications-integrating-app-server.md) для отправки уведомлений через Microsoft Graph.

4.  [Интегрируйте](notifications-integrating-with-windows.md) [пакет SDK клиента уведомлений Microsoft Graph](https://github.com/microsoft/project-rome) в клиенты приложений для Windows, Android или iOS, чтобы получать уведомления и управлять ими.
