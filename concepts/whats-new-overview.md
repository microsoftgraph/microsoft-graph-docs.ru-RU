---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: 30119dbd92c3a1b8552f19857225d868d50dd03b
ms.sourcegitcommit: 0ae140eafaca2dddc4584930cc0ac27fb1731c61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017115"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей за последние два месяца в Microsoft Graph, [добавленных ранее возможностей](whats-new-earlier.md) и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробный список обновлений на уровне API см. в [журнале изменений API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут изменяться без предварительного уведомления, а некоторые из них, возможно, никогда не достигнут общедоступного состояния (GA). Не используйте функции, доступные в виде предварительных версий, в рабочих приложениях.


## <a name="march-2022-new-and-generally-available"></a>Март 2022 г.: новые и общедоступные возможности

### <a name="files"></a>Файлы
Использование ресурса [bundle](/graph/api/resources/bundle) для обмена несколькими файлами одновременно, аналогично другим ресурсам [driveItem](/graph/api/resources/driveitem). Вы можете применять действия CRUD к пакету и [добавить](/graph/api/bundle-additem) элемент в пакет или [удалить](/graph/api/bundle-removeitem) его из пакета.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Использование [разрешения для конкретного ресурса](/graph/api/resources/resourcespecificpermission), чтобы авторизовать прямой доступ приложения Teams к данным определенного экземпляра чата или команды. Например, разрешение для конкретного ресурса ChannelMessage.Read.Group позволяет приложению Teams читать сообщения канала одной команды.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
[Получение](/graph/api/approval-get) решений об [утверждении](/graph/api/resources/approval), связанных с [запросом на назначение пакета доступа](/graph/api/resources/accesspackageassignmentrequest).

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход в систему
Указание [включения или исключения клиентских приложений](/graph/api/resources/conditionalaccessclientapplications) среди [набора условий](/graph/api/resources/conditionalAccessConditionSet) для применения [политики условного доступа](/graph/api/resources/conditionalaccesspolicy).


## <a name="march-2022-new-in-preview-only"></a>Март 2022 г.: новые возможности только в предварительной версии

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
Указание одного или нескольких [участников собрания](/graph/api/resources/meetingParticipants?view=graph-rest-beta&preserve-view=true) в качестве соорганизатора.

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер
- Использование делегированных разрешений или разрешений приложения `RoleManagement.Read.CloudPC` для операций чтения ресурса [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Использование делегированных разрешений или разрешений приложения `RoleManagement.ReadWrite.CloudPC` для операций чтения и записи ресурса [unifiedRoleDefinition](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true).
- Указание идентификатора и отображаемого имени подписки Azure в составе сведений об [исходном образе устройства](/graph/api/resources/cloudPcSourceDeviceImage?view=graph-rest-beta&preserve-view=true).
- Указание [параметров Windows](/graph/api/resources/cloudpcwindowssettings?view=graph-rest-beta&preserve-view=true) для настройки при создании облачных компьютеров для [политики подготовки](/graph/api/resources/cloudPcProvisioningPolicy?view=graph-rest-beta&preserve-view=true).

### <a name="device-and-app-management--corporate-management"></a>Управление устройствами и приложениями | Корпоративное управление
- Обновления Intune за март для бета-версии.

### <a name="device-and-app-management--multi-tenant-management"></a>Управление устройствами и приложениями | Управление несколькими клиентами
[Перечисление](/graph/api/managedtenants-managedtenant-list-auditevents?view=graph-rest-beta&preserve-view=true) и [получение](/graph/api/managedtenants-auditevent-get?view=graph-rest-beta&preserve-view=true) событий аудита для управляемых клиентов в Microsoft 365 Lighthouse.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
[Перечисление](/graph/api/organizationsettings-list-microsoftapplicationdataaccess?view=graph-rest-beta&preserve-view=true) или [обновление](/graph/api/microsoftapplicationdataaccesssettings-update?view=graph-rest-beta&preserve-view=true) [параметров](/graph/api/resources/microsoftapplicationdataaccesssettings?view=graph-rest-beta&preserve-view=true), которые определяют доступ из приложений Майкрософт к данным Microsoft 365, принадлежащим пользователям в организации. Например (при надлежащей авторизации) указывается, могут ли только приложения Microsoft 365 (к примеру, Word и Excel) получать доступ к данным Microsoft 365 пользователей или другие приложения Майкрософт (например, Windows) также могут получать доступ к данным. По умолчанию все пользователи в организации могут получить доступ в приложении Майкрософт к любым данным Microsoft 365, к которым пользователю был разрешен доступ. 

### <a name="security--attack-simulation-and-training"></a>Безопасность | Имитация атак и обучение
- [Перечисление автоматизации имитации](/graph/api/attacksimulationroot-list-simulationautomations?view=graph-rest-beta&preserve-view=true) для клиента.
- [Перечисление запусков](/graph/api/resources/simulationautomationrun?view=graph-rest-beta&preserve-view=true) автоматизации имитации для клиента.

### <a name="search"></a>Поиск
- Указание в [поисковом запросе](/graph/api/resources/searchrequest?view=graph-rest-beta&preserve-view=true), следует ли удалить дубликаты файлов SharePoint из результатов поиска. Значение по умолчанию — False.
- Квалификация строки [поискового запроса](/graph/api/resources/searchquery?view=graph-rest-beta&preserve-view=true) с помощью шаблона, который поддерживает KQL и переменные запроса.

### <a name="sites-and-lists"></a>Сайты и списки
Для [столбца](/graph/api/resources/columnDefinition?view=graph-rest-beta&preserve-view=true), содержащего данные таксономии, указывается родительский [термин](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true) и [набор терминов](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true), для которых дочерние термины можно выбрать в качестве значений столбцов.

### <a name="tasks-and-plans"></a>Задачи и планы
Определение того, может ли план Планировщика, предназначенный для интерфейсов за пределами Планировщика (например, Microsoft Teams), отслеживать работу в этом контексте путем проверки связи **details** соответствующего ресурса [plannerPlan](/graph/api/resources/plannerPlan?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Teamwork
- Получение или настройка [сводных сведений](/graph/api/resources/teamSummary?view=graph-rest-beta&preserve-view=true) о [команде](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true), включая количество владельцев, участников и гостей.
- Сортировка сообщений по убыванию при [перечислении сообщений в чате](/graph/api/chat-list-messages?view=graph-rest-beta&preserve-view=true).


## <a name="february-2022-new-and-generally-available"></a>Февраль 2022 г.: новые и общедоступные возможности

### <a name="teamwork"></a>Teamwork
Получение [сведений о виртуальном собрании](/graph/api/resources/teamworkOnlineMeetingInfo), связанном с [чатом](/graph/api/resources/chat), с помощью свойства **onlineMeetingInfo**.

## <a name="february-2022-new-in-preview-only"></a>Февраль 2022 г.: новое только в предварительной версии

### <a name="applications"></a>Приложения
- Использование нового параметра политики для [методов проверки подлинности приложения](/graph/api/resources/applicationauthenticationmethodpolicy?view=graph-rest-beta&preserve-view=true), чтобы ограничить секрет пользовательского пароля для приложения или субъекта-службы.
- Указание [параметров](/graph/api/resources/windowsApplication?view=graph-rest-beta&preserve-view=true) приложений для устройств под управлением Windows, опубликованных в Microsoft Store или магазине игр Xbox.

### <a name="change-notifications"></a>Уведомления об изменениях
Подписка на изменения контактов, событий или сообщений Outlook для получения уведомлений, в полезные данные которых включены данные ресурсов. Дополнительные сведения см. в статье [Уведомления об изменениях, связанных с ресурсами Outlook, в Microsoft Graph](outlook-change-notifications-overview.md).

### <a name="device-and-app-management--cloud-pc"></a>Управление устройствами и приложениями | Облачный компьютер 
- Определение [параметров точки восстановления](/graph/api/resources/cloudpcrestorepointsetting?view=graph-rest-beta&preserve-view=true), которые включают периодичность создания точки восстановления и определяют возможность восстановления пользователями своих облачных компьютеров на основе резервной копии точки восстановления.
- [Восстановление](/graph/api/manageddevice-restorecloudpc?view=graph-rest-beta&preserve-view=true) облачного компьютера на основе предыдущего моментального снимка.
- [Восстановление несколько облачных компьютеров](/graph/api/manageddevice-bulkrestorecloudpc?view=graph-rest-beta&preserve-view=true) в одном запросе путем указания идентификаторов их управляемых устройств и диапазона даты и времени (например, до, после) точки восстановления.

### <a name="identity-and-access--directory-management"></a>Удостоверение и доступ | Управление каталогом
Использование прав доступа приложений для `CustomSecAttributeAssignment.Read.All` чтения [пользовательских определений атрибутов безопасности](/graph/api/resources/customsecurityattributedefinition?view=graph-rest-beta&preserve-view=true) для организации без пользователя, выполнившего вход.

### <a name="identity-and-access--governance"></a>Удостоверение и доступ | Управление
- Настройка [параметров](/graph/api/resources/accessreviewstagesettings?view=graph-rest-beta&preserve-view=true) каждого [этапа](/graph/api/resources/accessreviewstage?view=graph-rest-beta&preserve-view=true) в многоступенчатой проверке доступа. Помимо [получения](/graph/api/accessreviewstage-get?view=graph-rest-beta&preserve-view=true) или [обновления](/graph/api/accessreviewstage-update?view=graph-rest-beta&preserve-view=true) этапа проверки доступа, вам доступны следующие действия: 
  - [Остановка](/graph/api/accessreviewstage-stop?view=graph-rest-beta&preserve-view=true) предоставления проверяющими дополнительной информации на некотором этапе и переход к следующему этапу (если применимо). 
  - [Фильтрация](/graph/api/accessreviewstage-filterbycurrentuser?view=graph-rest-beta&preserve-view=true) и получение всех этапов [экземпляра проверки доступа](/graph/api/resources/accessreviewinstance?view=graph-rest-beta&preserve-view=true), для которого вызывающий пользователь является проверяющим
  - [Составление списка решений](/graph/api/accessreviewstage-list-decisions?view=graph-rest-beta&preserve-view=true) из многоступенчатой проверки доступа.
- Приложения могут использовать разрешение приложения `EntitlementManagement.ReadWrite.All` в целях [создания запроса пакета доступа для ресурса](/graph/api/entitlementmanagement-post-accesspackageresourcerequests?view=graph-rest-beta&preserve-view=true), чтобы добавить ресурс в [каталог пакетов доступа](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true) или удалить его из каталога.

### <a name="identity-and-access--identity-and-sign-in"></a>Удостоверение и доступ | Удостоверение и вход
- Использование ряда новых свойств для настройки [фирменного стиля организации](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). Например, варианта логотипа компании в виде баннера для страницы входа, настраиваемой пиктограммы сайта с URL-адресом на основе CDN, а также нескольких других настраиваемых свойств, которые пользователи могут применять для управления учетными записями.
- Включение или исключение Linux как одного из [условий платформы](/graph/api/resources/conditionalaccessplatforms?view=graph-rest-beta&preserve-view=true) в [политике условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Выявление [субъектов-служб, с которыми связан риск](/graph/api/resources/riskyserviceprincipal?view=graph-rest-beta&preserve-view=true), в организации с помощью службы Azure AD, которая постоянно [определяет и оценивает риски](/graph/api/resources/serviceprincipalriskdetection?view=graph-rest-beta&preserve-view=true) на основе различных сигналов и машинного обучения. Вы можете [подтвердить](/graph/api/riskyserviceprincipal-confirmcompromised?view=graph-rest-beta&preserve-view=true), что субъект-служба действительно скомпрометирован, после чего корпорация Майкрософт отключит объект этого субъекта-службы. Вы можете [отклонить](/graph/api/riskyserviceprincipal-dismiss?view=graph-rest-beta&preserve-view=true) риск, связанный с субъектом-службой. Кроме того, вы можете [создать журнал рисков](/graph/api/riskyserviceprincipal-list-history?view=graph-rest-beta&preserve-view=true), связанных с субъектом-службой.
- Использование [параметров межклиентского доступа](/graph/api/resources/crosstenantaccesspolicy-overview?view=graph-rest-beta&preserve-view=true) для контроля над взаимодействием между пользователями в вашей и других организациях и управления этим взаимодействием. Эти параметры детализированы и позволяют определять пользователей, группы и приложения как в вашей, так и во внешних организациях, которые могут участвовать во взаимодействии в рамках Azure AD B2B и прямом подключении Azure AD B2B. 
- Разрешение или запрещение пользователям и группам в организации применять [встроенную в Azure AD проверку подлинности на основе сертификатов (CBA)](/graph/api/resources/x509CertificateAuthenticationMethodConfiguration?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Поиск
Настройка ресурсов [acronym](/graph/api/resources/search-acronym?view=graph-rest-beta&preserve-view=true), [bookmark](/graph/api/resources/search-bookmark?view=graph-rest-beta&preserve-view=true) и [QnA](/graph/api/resources/search-qna?view=graph-rest-beta&preserve-view=true) в качестве [ответов административного поиска для пользователей в организации](search-concept-answers.md).


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
