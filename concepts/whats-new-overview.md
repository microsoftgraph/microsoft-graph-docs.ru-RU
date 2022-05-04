---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 4db9be8a564eb133b92830729902f5c36d0ed84c
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191670"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


## <a name="april-2022-new-in-preview-only"></a>Апрель 2022 г.: новые возможности только в предварительной версии

### <a name="customer-bookings"></a>Резервирование для пользователей
- [Получение сведений о доступности](/graph/api/bookingbusiness-getstaffavailability?view=graph-rest-beta&preserve-view=true) ресурсов [staff member](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true) в [организации](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true).
- Использование разрешения приложений `Bookings.Read.All` в операциях чтения для ресурсов [business](/graph/api/resources/bookingbusiness?view=graph-rest-beta&preserve-view=true), [staff member](/graph/api/resources/bookingstaffmember?view=graph-rest-beta&preserve-view=true), [service](/graph/api/resources/bookingservice?view=graph-rest-beta&preserve-view=true), [customer](/graph/api/resources/bookingcustomer?view=graph-rest-beta&preserve-view=true) и [appointment](/graph/api/resources/bookingappointment?view=graph-rest-beta&preserve-view=true).
- Использование разрешения приложений `BookingsAppointment.ReadWrite.All` для операций чтения и записи ресурсов клиентов и встреч.

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер
Указание [параметров Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) в составе [ параметров организации облачного компьютера](/graph/api/resources/cloudPcOrganizationSettings?view=graph-rest-beta&preserve-view=true) для клиента.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Настройка [параметров федерации](/graph/api/resources/internalDomainFederation?view=graph-rest-beta&preserve-view=true) федеративных доменов в Azure Active Directory.

### <a name="reports--identity-and-access-reports"></a>Отчеты | Отчеты об удостоверениях и доступе
Подтверждение того, что событие является [высокорискованным и скомпрометированным](/graph/api/signin-confirmCompromised?view=graph-rest-beta&preserve-view=true) или [безопасным](/graph/api/signin-confirmSafe?view=graph-rest-beta&preserve-view=true) путем его маркировки в соответствующих журналах входа Azure Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Отчеты | Отчеты об использовании Microsoft 365
- [Получение общего отчета о распределении](/graph/api/reportroot-getTeamsUserActivityTotalDistributionCounts?view=graph-rest-beta&preserve-view=true) для количества определенных действий Teams за указанный период. Количество действий Teams, включая сообщения чата команды, звонки, собрания, длительность звукового фрагмента, публикацию сообщений и т. д.
- Получение дополнительных типов действий в отчетах, которые [получают сведения о пользователе](/graph/api/reportroot-getTeamsUserActivityUserDetail?view=graph-rest-beta&preserve-view=true), [получают количество действий](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta&preserve-view=true) и [получают общее количество действий](/graph/api/reportroot-getteamsuseractivitytotalcounts?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Командная работа
Предоставление общего доступа к каналу одной или нескольким командам:
- [Перечисление только каналов, к которым предоставлен общий доступ в команде](/graph/api/team-list-incomingchannels?view=graph-rest-beta&preserve-view=true).
- [Перечисление всех каналов в команде](/graph/api/team-list-allchannels?view=graph-rest-beta&preserve-view=true), включая каналы, размещенные в команде, и команды, к которым предоставлен общий доступ в команде.
- [Перечисление участников команды, у которых есть доступ к указанному общему каналу](/graph/api/sharedwithchannelteaminfo-list-allowedmembers?view=graph-rest-beta&preserve-view=true).
- [Удаление канала, к которому предоставлен общий доступ в команде](/graph/api/team-delete-incomingchannel?view=graph-rest-beta&preserve-view=true).
- [Перечисление команд, которым предоставлен общий доступ к указанному каналу](/graph/api/sharedwithchannelteaminfo-list?view=graph-rest-beta&preserve-view=true).
- [Отмена общего доступа к каналу для команды](/graph/api/sharedwithchannelteaminfo-delete?view=graph-rest-beta&preserve-view=true).


## <a name="march-2022-new-and-generally-available"></a>Март 2022 г.: новые и общедоступные возможности

### <a name="files"></a>Файлы
Использование ресурса [bundle](/graph/api/resources/bundle) для обмена несколькими файлами одновременно, аналогично другим ресурсам [driveItem](/graph/api/resources/driveitem). Вы можете применять действия CRUD к пакету и [добавить](/graph/api/bundle-additem) элемент в пакет или [удалить](/graph/api/bundle-removeitem) его из пакета.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Использование [разрешения для конкретного ресурса](/graph/api/resources/resourcespecificpermission), чтобы авторизовать прямой доступ приложения Teams к данным определенного экземпляра чата или команды. Например, разрешение для конкретного ресурса ChannelMessage.Read.Group позволяет приложению Teams читать сообщения канала одной команды.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- [Получение](/graph/api/approval-get) решений об [утверждении](/graph/api/resources/approval), связанных с [запросом на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest).
- В рамках [управления правами Azure Active Directory (Azure AD)](/graph/api/resources/entitlementmanagement-overview) используйте [политику назначения пакета доступа](/graph/api/resources/accesspackageassignmentpolicy) для управления запросом, утверждением, назначением или регулярной проверкой [пакета доступа](/graph/api/resources/accesspackage). Вы можете управлять доступом внутренних и внешних пользователей к группам, приложениям и веб-сайтам SharePoint Online организации.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Указание [включения или исключения клиентских приложений](/graph/api/resources/conditionalaccessclientapplications) среди [набора условий](/graph/api/resources/conditionalAccessConditionSet) для применения [политики условного доступа](/graph/api/resources/conditionalaccesspolicy).


## <a name="march-2022-new-in-preview-only"></a>Март 2022 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
Указание одного или нескольких [участников собрания](/graph/api/resources/meetingParticipants?view=graph-rest-beta&preserve-view=true) в качестве соорганизатора.

### <a name="compliance--ediscovery"></a>Соответствие требованиям | Обнаружение электронных данных
[Очистка данных](/graph/api/ediscovery-sourcecollection-purgeData?view=graph-rest-beta&preserve-view=true) и окончательное удаление сообщений Microsoft Teams из [исходной коллекции](/graph/api/resources/ediscovery-sourcecollection?view=graph-rest-beta&preserve-view=true) обнаружения электронных данных.

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер
- Использование делегированных разрешений или разрешений приложения `RoleManagement.Read.CloudPC` для операций чтения ресурса [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Использование делегированных разрешений или разрешений приложения `RoleManagement.ReadWrite.CloudPC` для операций чтения и записи ресурса [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Указание идентификатора и отображаемого имени подписки Azure в составе сведений об [исходном образе устройства](/graph/api/resources/cloudPcSourceDeviceImage?view=graph-rest-beta&preserve-view=true).
- Указание и настройка [параметров Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) при создании облачных компьютеров для [политики подготовки](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true).

### <a name="device-and-app-management--corporate-management"></a>Управление устройствами и приложениями | Корпоративное управление
- Обновления Intune за март для бета-версии.

### <a name="device-and-app-management--multi-tenant-management"></a>Управление устройствами и приложениями | Управление несколькими клиентами
[Перечисление](/graph/api/managedtenants-managedtenant-list-auditevents?view=graph-rest-beta&preserve-view=true) и [получение](/graph/api/managedtenants-auditevent-get?view=graph-rest-beta&preserve-view=true) событий аудита для управляемых клиентов в Microsoft 365 Lighthouse.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
- [Перечисление](/graph/api/organizationsettings-list-microsoftapplicationdataaccess?view=graph-rest-beta&preserve-view=true) или [обновление](/graph/api/microsoftapplicationdataaccesssettings-update?view=graph-rest-beta&preserve-view=true) [параметров](/graph/api/resources/microsoftapplicationdataaccesssettings?view=graph-rest-beta&preserve-view=true), которые определяют доступ из приложений Майкрософт к данным Microsoft 365, принадлежащим пользователям в организации. Например (при надлежащей авторизации) указывается, могут ли только приложения Microsoft 365 (к примеру, Word и Excel) получать доступ к данным Microsoft 365 пользователей или другие приложения Майкрософт (например, Windows) также могут получать доступ к данным. По умолчанию все пользователи в организации могут получить доступ в приложении Майкрософт к любым данным Microsoft 365, к которым пользователю был разрешен доступ. 
- Следуя модели кибербезопасности "Никому не доверяй", партнеры Майкрософт могут использовать [детализированные права полномочного администратора (GDAP)](/graph/api/resources/delegatedadminrelationships-api-overview?view=graph-rest-beta&preserve-view=true) для выполнения административных задач с минимальными правами доступа к клиентам пользователей, чтобы избежать потенциальных рисков безопасности. Вместо запроса роли глобального администратора (как в прошлом) партнеры запрашивают определенные роли для администрирования клиента пользователя на определенный период времени, а их пользователи должны явно предоставить им доступ с минимальными правами.

### <a name="security--attack-simulation-and-training"></a>Безопасность | Имитация атак и обучение
- [Перечисление автоматизации имитации](/graph/api/attacksimulationroot-list-simulationautomations?view=graph-rest-beta&preserve-view=true) для клиента.
- [Перечисление запусков](/graph/api/resources/simulationautomationrun?view=graph-rest-beta&preserve-view=true) автоматизации имитации для клиента.

### <a name="search"></a>Поиск
- Указание в [поисковом запросе](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true), следует ли удалить дубликаты файлов SharePoint из результатов поиска. Значение по умолчанию: false.
- Квалификация строки [поискового запроса](/graph/api/resources/searchquery?view=graph-rest-beta&preserve-view=true) с помощью шаблона, который поддерживает KQL и переменные запроса.

### <a name="sites-and-lists"></a>Сайты и списки
- Для [столбца](/graph/api/resources/columnDefinition?view=graph-rest-beta&preserve-view=true), содержащего данные таксономии, указывается родительский [термин](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) и [набор терминов](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true), для которых дочерние термины можно выбрать в качестве значений столбцов.
- Получение параметров [сайта](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true), включая его язык и часовой пояс.

### <a name="tasks-and-plans"></a>Задачи и планы
Определение того, может ли план Планировщика, предназначенный для интерфейсов за пределами Планировщика (например, Microsoft Teams), отслеживать работу в этом контексте путем проверки связи **details** соответствующего ресурса [plannerPlan](/graph/api/resources/plannerPlan?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Teamwork
- Получение или настройка [сводных сведений](/graph/api/resources/teamSummary?view=graph-rest-beta&preserve-view=true) о [команде](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), включая количество владельцев, участников и гостей.
- Сортировка сообщений по убыванию при [перечислении сообщений в чате](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на сайте [сообщества Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Впервые в состоянии **_предварительной версии_**. Все связанные обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](https://developer.microsoft.com/graph/changelog/).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).
