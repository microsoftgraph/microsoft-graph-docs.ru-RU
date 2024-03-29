---
title: Создание и отправка уведомления из службы приложений (устарело)
description: Вы можете создать и отправить уведомление пользователю с помощью API Microsoft Graph (устарело).
ms.localizationpriority: high
ms.prod: notifications
author: merzink
ms.openlocfilehash: 302375137bb2408bcd6be5ad737cf34cc7d6ee70
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447137"
---
# <a name="create-and-send-a-notification-from-your-app-service-deprecated"></a>Создание и отправка уведомления из службы приложений (устарело)

> [!IMPORTANT]
> API уведомлений Microsoft Graph не рекомендуется использовать, Он прекратил возвращать данные в январе 2022 г. Дополнительные сведения об уведомлениях см. в [Центрах уведомлений Microsoft Azure](/azure/notification-hubs). Дополнительные сведения см. в записи блога [Прекращение поддержки API уведомлений Microsoft Graph (бета-версия)](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/).

Вы можете создавать и отправлять уведомления пользователю с помощью API Microsoft Graph. Уведомление хранится в хранилище службы уведомлений Microsoft Graph и отправляется всем клиентам приложений на всех устройствах, с которых целевой пользователь выполнил вход в систему. 

Чтобы отправить уведомление пользователю, служба приложений выполнит указанные ниже действия.
1. [Проверка подлинности](/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) на платформе удостоверений Майкрософт.
2. Отправка уведомления в API Microsoft Graph при помощи маркера проверки подлинности с указанием [идентификатора подписки на уведомления пользователя](/graph/api/notifications-post), полученного из клиента приложения при создании подписки.

> [!NOTE]
> Чтобы упростить проверку подлинности, рекомендуем использовать новый, улучшенный и компактный [пакет SDK уведомлений](https://aka.ms/GNSDK) на стороне клиента с идентификатором подписки на уведомления пользователя, чтобы получать уведомления и управлять их состоянием. Вы также можете отправлять уведомления от имени пользователя с помощью делегированных разрешений, а службе приложений потребуется хранить маркеры доступа и обновления. Однако это не рекомендуется. Дополнительные сведения о потоке OBO OAuth 2.0 см. в статье [Вызовы между службами с использованием делегированного удостоверения пользователя в потоке On-Behalf-Of](/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow). 


## <a name="guaranteed-delivery-on-ios"></a>Гарантированная доставка в iOS

На таких платформах, как iOS, при определенных уровнях производительности уведомления о необработанных данных могут доставляться с задержкой в связи с пакетной обработкой или вообще не достигать конечной точки. В случае высокоприоритетных уведомлений, доставляемых пользователям в iOS, платформа уведомлений Microsoft Graph позволяет выбрать функцию "резервирования" всплывающих уведомлений из необработанных данных в визуальные на целевом устройстве iOS, обеспечивая уведомление пользователей практически в реальном времени. Сведения о том, как использовать параметры резервирования, см. в описании [ресурса notification](/graph/api/resources/projectrome-notification.md).  

## <a name="getting-started"></a>Начало работы
Сведения о том, как служба приложений может начать отправлять уведомления пользователям, см. в описании объекта [notification](/graph/api/resources/projectrome-notification) и нашем [образце службы приложений](https://aka.ms/gnsample-appservice).
