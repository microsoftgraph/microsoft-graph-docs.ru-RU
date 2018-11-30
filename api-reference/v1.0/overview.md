---
title: Справочные материалы по REST API Microsoft Graph v1.0
description: Добро пожаловать в справочник REST API Microsoft Graph для конечной точки версии 1.0.
ms.openlocfilehash: 628b631a877a29dc416671c4a0c5f9a5c0b849ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027918"
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
6. [Настройка автоматических ответов,](./api/user-update-mailboxsettings.md#example) когда Мария находится вне офиса.
7. [Определение людей, которые наиболее важны для Марии,](./api/user-list-people.md) в зависимости от общения, совместной работы и корпоративных связей.
8. Получение последней проекции продаж из [диаграммы](./resources/chart.md) в файле Excel в инструменте Марии OneDrive для бизнеса.
9. [Поиск задач, назначенных Марии, в планировщике](./api/planneruser-list-tasks.md).

### <a name="office-365-group-use-cases-in-v10"></a>Групповые сценарии выполнения Office 365 в версии 1.0

1. Запуск отчета о группах Office 365 в организации и определение группы с самыми часто [общающимися участниками группы](./api/reportroot-getoffice365groupsactivitycounts.md).
2. [Поиск планов этой группы Office 365](./api/plannergroup-list-plans.md) и [назначение задач](./resources/plannerassignments.md) в этом плане.
3. [Начало новой беседы](./api/group-post-conversations.md) в группе Office 365, чтобы определить, хотят ли участники [создать другую группу](./api/group-post-groups.md) для предоставление общего доступа к рабочей нагрузке.
4. [Получение стандартной записной книжки](./api/notebook-get.md) для группы и [создание страницы](./api/section-post-pages.md) для записи результата исследования.

## <a name="other-api-versions"></a>Другие версии API

В настоящее время существует две версии REST API Microsoft Graph – версия 1.0 и бета-версия.
Если вас интересует новые и улучшенные API, которые по-прежнему находятся в предварительной версии, см. статью [Справочник по конечной точке бета-версии Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta). Следует помнить, что API в предварительной версии могут изменяться и могут нарушить работу существующих сценариев без уведомлений. Не создавайте зависимость рабочей среды от API в конечной точке бета-версии.

Дополнительные сведения см. в статье [Управление версиями и поддержка](/graph/versioning-and-support).

## <a name="connect-with-us"></a>Обратная связь

Есть ли дополнительные API или функции, которые вы бы хотели увидеть в Microsoft Graph? Опубликуйте запросы новых функций на [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).

Хотите оставить отзыв по существующим API Microsoft Graph? Свяжитесь с нами в [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).

Вопросы или справки в коде с помощью корпорацию Майкрософт