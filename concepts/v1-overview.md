# <a name="microsoft-graph-rest-api-v10-reference"></a>Справочные материалы по REST API Microsoft Graph v1.0

Добро пожаловать в справочник REST API Microsoft Graph для конечной точки версии 1.0.

Наборы API в конечной точке версии 1.0 (`https://graph.microsoft.com/v1.0`) находятся в общедоступном состоянии и подверглись строгому процессу проверки и отзывов при участии клиентов, чтобы удовлетворить практические и производственные требования. Обновления для API в этой конечной точке являются добавочными и не прерывают существующие сценарии приложения.

## <a name="common-use-cases"></a>Основные сценарии выполнения

Главное достоинство Microsoft Graph заключается в удобной навигации объектов и связей в разных службах, предоставляемой в единой конечной точке REST Microsoft Graph.

Некоторые из этих служб предназначены для выполнения сложных сценариев для [пользователей](../api-reference/v1.0/resources/user.md) и [групп](../api-reference/v1.0/resources/group.md).

### <a name="user-centric-use-cases-in-v10"></a>Сценарии выполнения, ориентированные на пользователя, в версии 1.0

1. [Получение профиля](../api-reference/v1.0/api/user_get.md) и [фотографии](../api-reference/v1.0/resources/profilephoto.md) пользователя Мария.
2. [Получение сведений о профиле менеджера Марии](../api-reference/v1.0/api/user_list_manager.md) и [идентификаторов ее подчиненных](../api-reference/v1.0/api/user_list_directreports.md), хранимых в Azure Active Directory.
3. [Получение доступа к файлам Марии в OneDrive для бизнеса](../api-reference/v1.0/api/driveitem_list_children.md), поиск [удостоверения](../api-reference/v1.0/resources/identityset.md) последнего человека, который внес изменения в [файл](../api-reference/v1.0/resources/driveitem.md), и переход к профилю этого человека.
4. [Получение доступа к календарю Марии](../api-reference/v1.0/api/calendar_get.md) в Exchange Online и [определение наиболее подходящего времени для встречи Марии с ее группой](../api-reference/v1.0/api/user_findmeetingtimes.md) в следующие две недели.
5. [Подписка](../api-reference/v1.0/api/subscription_post_subscriptions.md) и [отслеживание изменений](../api-reference/v1.0/api/event_delta.md) в календаре Марии, уведомление Марии, если она проводит более 80% своего времени на собраниях.
6. [Настройка автоматических ответов,](../api-reference/v1.0/api/user_update_mailboxsettings.md#example) когда Мария находится вне офиса.
7. [Определение людей, которые наиболее важны для Марии,](../api-reference/v1.0/api/user_list_people.md) в зависимости от общения, совместной работы и корпоративных связей.
8. Получение последней проекции продаж из [диаграммы](../api-reference/v1.0/resources/chart.md) в файле Excel в инструменте Марии OneDrive для бизнеса.
9. [Поиск задач, назначенных Марии, в планировщике](../api-reference/v1.0/api/planneruser_list_tasks.md).

### <a name="office-365-group-use-cases-in-v10"></a>Групповые сценарии выполнения Office 365 в версии 1.0

1. Запуск отчета о группах Office 365 в организации и определение группы с самыми часто [общающимися участниками группы](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitycounts.md).
2. [Поиск планов этой группы Office 365](../api-reference/v1.0/api/plannergroup_list_plans.md) и [назначение задач](../api-reference/v1.0/resources/plannerassignments.md) в этом плане.
3. [Начало новой беседы](../api-reference/v1.0/api/group_post_conversations.md) в группе Office 365, чтобы определить, хотят ли участники [создать другую группу](../api-reference/v1.0/api/group_post_groups.md) для предоставление общего доступа к рабочей нагрузке.
4. [Получение стандартной записной книжки](../api-reference/v1.0/api/notebook_get.md) для группы и [создание страницы](../api-reference/v1.0/api/section_post_pages.md) для записи результата исследования.

## <a name="other-api-versions"></a>Другие версии API

В настоящее время существует две версии REST API Microsoft Graph – версия 1.0 и бета-версия.
Если вас интересует новые и улучшенные API, которые по-прежнему находятся в предварительной версии, см. статью [Справочник по конечной точке бета-версии Microsoft Graph](../api-reference/beta/beta-overview.md). Следует помнить, что API в предварительной версии могут изменяться и могут нарушить работу существующих сценариев без уведомлений. Не создавайте зависимость рабочей среды от API в конечной точке бета-версии.

Дополнительные сведения см. в статье [Управление версиями и поддержка](versioning_and_support.md).

## <a name="connect-with-us"></a>Обратная связь

Есть ли дополнительные API или функции, которые вы бы хотели увидеть в Microsoft Graph? Опубликуйте запросы новых функций на [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).

Хотите оставить отзыв по существующим API Microsoft Graph? Свяжитесь с нами в [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).

По вопросам или справкам по коду с использованием Microsoft Graph присоединяйтесь к нам в [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoftgraph).
