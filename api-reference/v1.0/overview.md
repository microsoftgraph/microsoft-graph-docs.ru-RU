---
title: Справочные материалы по REST API Microsoft Graph v1.0
description: Добро пожаловать в справочник REST API Microsoft Graph для конечной точки версии 1.0.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: non-product-specific
doc_type: conceptualPageType
ms.openlocfilehash: 35056993ce029a715f97885fa5e8cd29bbe2446e
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533985"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a>Справочные материалы по REST API Microsoft Graph v1.0

Добро пожаловать в справочник REST API Microsoft Graph для конечной точки версии 1.0.

Наборы API в конечной точке версии 1.0 (`https://graph.microsoft.com/v1.0`) находятся в общедоступном состоянии и подверглись строгому процессу проверки и отзывов при участии клиентов, чтобы удовлетворить практические и производственные требования. Обновления для API в этой конечной точке являются добавочными и не прерывают существующие сценарии приложения.

## <a name="common-use-cases"></a>Основные сценарии выполнения

Главное достоинство Microsoft Graph заключается в удобной навигации объектов и связей в разных службах, предоставляемой в единой конечной точке REST Microsoft Graph.

Некоторые из этих служб предназначены для выполнения сложных сценариев для [пользователей](./resources/user.md) и [групп](./resources/group.md).

### <a name="user-centric-use-cases-in-v10"></a>Сценарии выполнения, ориентированные на пользователя, в версии 1.0

1. [Получение профиля](./api/user-get.md) и [фотографии](./resources/profilephoto.md) пользователя Мария.
2. [Получение сведений о профиле менеджера Марии](./api/user-list-manager.md) и [идентификаторов ее подчиненных](./api/user-list-directreports.md), хранимых в Azure Active Directory.
3. [Получение доступа к файлам Марии в OneDrive для бизнеса](./api/driveitem-list-children.md), поиск [удостоверения](./resources/identityset.md) последнего человека, который внес изменения в [файл](./resources/driveitem.md), и переход к профилю этого человека.
4. [Получение доступа к календарю Марии](./api/calendar-get.md) в Exchange Online и [определение наиболее подходящего времени для встречи Марии с ее группой](./api/user-findmeetingtimes.md) в следующие две недели.
5. [Подписка](./api/subscription-post-subscriptions.md) и [отслеживание изменений](./api/event-delta.md) в календаре Марии, уведомление Марии, если она проводит более 80% своего времени на собраниях.
6. [Настройка автоматических ответов,](./api/user-update-mailboxsettings.md#example-1) когда Мария находится вне офиса.
7. [Определение людей, которые наиболее важны для Марии,](./api/user-list-people.md) в зависимости от общения, совместной работы и корпоративных связей.
8. Получение последней проекции продаж из [диаграммы](./resources/chart.md) в файле Excel в инструменте Марии OneDrive для бизнеса.
9. [Поиск задач, назначенных Марии, в планировщике](./api/planneruser-list-tasks.md).

### <a name="microsoft-365-group-use-cases-in-v10"></a>Варианты использования групп Microsoft 365 в версии 1.0

1. Запуск отчета о группах Microsoft 365 в организации и определение группы с самыми часто [общающимися участниками группы](./api/reportroot-getoffice365groupsactivitycounts.md).
2. [Поиск планов группы Microsoft 365](./api/plannergroup-list-plans.md) и [назначение задач](./resources/plannerassignments.md) в плане.
3. [Начало новой беседы](./api/group-post-conversations.md) в группе Microsoft 365, чтобы определить, хотят ли участники [создать другую группу](./api/group-post-groups.md) для предоставления общего доступа к рабочей нагрузке.
4. [Получение стандартной записной книжки](./api/notebook-get.md) для группы и [создание страницы](./api/section-post-pages.md) для записи результата исследования.

## <a name="other-api-versions"></a>Другие версии API

В настоящее время существует две версии REST API Microsoft Graph – версия 1.0 и бета-версия.
Если вас интересует новые и улучшенные API, которые по-прежнему находятся в предварительной версии, см. статью [Справочник по конечной точке бета-версии Microsoft Graph](/graph/api/overview?view=graph-rest-beta&preserve-view=true). Следует помнить, что API в предварительной версии могут изменяться и могут нарушить работу существующих сценариев без уведомлений. Не создавайте зависимость рабочей среды от API в конечной точке бета-версии.

Дополнительные сведения см. в статье [Управление версиями и поддержка](/graph/versioning-and-support).

## <a name="call-the-v10-endpoint"></a>Вызов конечной точки версии 1.0

В запросах API Microsoft Graph к конечной точке версии 1.0 используется следующий шаблон:

```http
https://graph.microsoft.com/v1.0/{resource}?[query_parameters]
```

Дополнительные сведения см. в статье [Использование API Microsoft Graph](/graph/use-the-api).

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) конечной точки версии 1.0.

## <a name="connect-with-us"></a>Обратная связь

Есть ли дополнительные API или функции, которые вы бы хотели увидеть в Microsoft Graph? Опубликуйте новый запрос функции на [форуме идей платформы для разработчиков Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).

Хотите оставить отзыв по существующим API Microsoft Graph? Свяжитесь с нами в [GitHub](https://github.com/microsoftgraph/microsoft-graph-docs/issues).
