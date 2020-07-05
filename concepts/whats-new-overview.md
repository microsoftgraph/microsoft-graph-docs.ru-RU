---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: d0e462ab93b60796e8cbb4463c19799ba9033cd2
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038648"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API [можно](changelog.md#may-2020) найти в разделах и [июньах](changelog.md#june-2020) , а также в разделах журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="july-2020-new-and-generally-available"></a>Июль 2020: новый и обычно доступный

### <a name="change-notifications"></a>Уведомления об изменениях
Удалено представленное свойство **SequenceNumber** ерронаусли из ресурса [чанженотификатион](/graph/api/resources/changenotification) .

## <a name="july-2020-new-in-preview-only"></a>Июль 2020: Новая версия только для предварительного просмотра

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
Используйте разрешения приложения `Printer.ReadWrite.All` и [кодировку Internet Print Protocol (IPP)](https://tools.ietf.org/html/rfc8010) для [обновления принтера](/graph/api/printer-update?view=graph-rest-beta).

## <a name="june-2020-new-and-generally-available"></a>Июнь 2020: новый и обычно доступный

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
- Используйте `Accept-Language` заголовок HTTP при [создании собрания по сети](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) для предоставления сведений о соединении на основе языкового стандарта.
- Используйте [креатеоржет](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) , чтобы вернуть собрание по сети, которое содержит указанное значение **екстерналид** , или создайте его, если он уже существует, для упрощения внедрения результирующего собрания в сторонний календарь.

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:
  - Используйте свойство **пендингоператионс** , чтобы определить все [операции](/graph/api/resources/pendingoperations) , которые могут обновить двоичный контент файла [driveItem](/graph/api/resources/driveitem) , ожидающие завершения.
  - [Восстановление](/graph/api/driveitem-restore) **driveItem** , который был удален и находится в корзине в OneDrive персональный.
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo). Настройка поддерживается в OneDrive персональный.
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file).
- Используйте `deferCommit` параметр, чтобы отложить завершающее создание при [отправке большого файла](/graph/api/driveitem-createuploadsession) в OneDrive для бизнеса, пока приложение не выполнит запрос на завершение отправки.
- Используйте свойство **филесизе** для предоставления в качестве части параметра **Item** оценки, поэтому для проверки квоты перед [отправкой файла](/graph/api/driveitem-createuploadsession) в OneDrive персональный.
- Найдите [storagePlanInformation](/graph/api/resources/storageplaninformation) через свойство **Quota** ресурса [Drive](/graph/api/resources/drive) , чтобы проверить наличие более высоких планов квот хранилища.

### <a name="groups"></a>Группы
Используйте разрешения приложения `Group.Read.All` , `Group.ReadWrite.All` чтобы получить ресурсы групповых [бесед](/graph/api/resources/conversation) и [бесед](/graph/api/resources/conversationthread) .

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Дж двух наборов API для [защиты идентификации](/graph/api/resources/identityprotectionroot): [Обнаружение риска](/graph/api/resources/riskdetection) и [рискованные пользовательские](/graph/api/resources/riskyuser) API.

### <a name="security"></a>Безопасность
- Отслеживайте следующие свойства [оповещения](/graph/api/resources/alert?view=graph-rest-1.0):
  - Идентификаторы инцидентов, связанных с оповещением.
  - Определите [ресурс](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) как атаковать или как связанный ресурс в оповещении.
  - Укажите расположение источника и назначения для [сетевого подключения](/graph/api/resources/networkconnection?view=graph-rest-1.0) , связанного с оповещением.

### <a name="sites-and-lists"></a>Сайты и списки
Указание данных географического расположения в [определении столбца](/graph/api/resources/columndefinition) для ресурса [списка](/graph/api/resources/list) SharePoint.

### <a name="teamwork"></a>Командная работа
- Используйте делегированное разрешение [CamlQuery. Read. ALL](/graph/permissions-reference#appcatalog-resource-permissions) , чтобы перечислить [приложения](/graph/api/resources/teamsapp?view=graph-rest-1.0) из каталога приложений Microsoft Teams.
- [Получение сведений о папке](/graph/api/channel-get-filesfolder) , которая сопоставлена с вкладкой " **файлы** " в [канале](/graph/api/resources/channel)Teams.
- [Получить канал по умолчанию](/graph/api/team-get-primarychannel), обозначенный как **Общий**, для [команды](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Июнь 2020: Новая версия только для предварительного просмотра

### <a name="calendar"></a>Календарь
Кроме отслеживания добавочных изменений событий в **calendarView** (коллекция или события, разделенные датами начала _и_ окончания), используйте функцию [Delta](/graph/api/event-delta?view=graph-rest-beta) для событий в почтовом ящике пользователя или событиях в определенном календаре пользователя.

### <a name="cloud-communications--presence"></a>Взаимодействие с облаком | Знак
[Получение сведений о присутствии](/graph/api/presence-get?view=graph-rest-beta) всех пользователей в организации или определенного пользователя в Организации. гргр

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Указание [полей печати](/graph/api/resources/printmargin?view=graph-rest-beta) при настройке [документа для печати](/graph/api/resources/printdocument?view=graph-rest-beta).
- Поддержка следующих [возможностей принтера](/graph/api/resources/printercapabilities?view=graph-rest-beta):
  - направления подачи
  - Печать диапазонов страниц
  - разрешение печати в точках на дюйм
  - максимальный размер очереди заданий печати в байтах
  - входные лотки
  - поля
  - параметры сортировки
  - масштабирование документов
- Поддержка разрешения печати (DPI) и масштабирование документа в составе [параметров принтера по умолчанию](/graph/api/resources/printerdefaults?view=graph-rest-beta).
- Поддержка следующих параметров [конфигурации документов](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta) :
  - входные лотки
  - выходные лотки
  - размеры носителей
  - поля
  - типы мультимедиа
  - завершения, такие как сшивка и привязывание
  - страниц на листе
  - многостраничный макет, указывающий направление разметки страниц на листе
  - параметры сортировки
  - масштабирование
- Раскрывать документы при [перечислении заданий Принг](/graph/api/printer-list-jobs?view=graph-rest-beta).
- [Зарегистрируйте принтер]() и используйте ресурс [принтеркреатеоператион](/graph/api/resources/printercreateoperation?view=graph-rest-beta) для отслеживания и проверки регистрации принтера.
- [Получение длительной операции регистрации принтера](/graph/api/printoperation-get?view=graph-rest-beta) в текущем пользователе или в клиенте приложения.
- Несколько переименованных свойств и перечисляемых типов — подробные сведения об обновлениях журнала изменений в [июне](changelog.md#june-2020) для облачной печати.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
В качестве бета-версии за [Июнь](changelog.md#june-2020) вы обновляете.

### <a name="education"></a>Образование
- Можно использовать делегированные разрешения `EduRoster.ReadBasic` для [получения](/graph/api/educationuser-get?view=graph-rest-beta) идентификатора [преподавателя](/graph/api/resources/educationteacher?view=graph-rest-beta) или [учащегося](/graph/api/resources/educationstudent?view=graph-rest-beta) во внешней программе, как свойство **екстерналид** .
- Используйте свойство **екстерналсаурце** , чтобы отслеживать значение, `lms` Если в системе управления обучением создается [Организация](/graph/api/resources/educationorganization?view=graph-rest-beta) или [класс](/graph/api/resources/educationclass?view=graph-rest-beta) образования.

### <a name="identity-and-access"></a>Удостоверение и доступ
- ИТ-специалисты могут использовать ресурсы [соединителей](/graph/api/resources/connector?view=graph-rest-beta) , которые являются упрощенными агентами для подключения к [прокси-серверу приложений Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy), и [публикации локальных приложений веб-приложений извне](/graph/api/resources/onpremisespublishing?view=graph-rest-beta), чтобы удаленные пользователи их организаций могли безопасно получать доступ к этим приложениям.
- Управление [политикой проверки подлинности](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta) на уровне клиента для включения или отключения [самостоятельной регистрации](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta) внешних пользователей.
- [Предоставление учетной записи пользователя по требованию](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta)и возможность указать объекты для подготовки и правила синхронизации для выполнения.

### <a name="search"></a>Search
- Используйте улучшения для [Свойства](/graph/api/resources/property?view=graph-rest-beta) в [схеме](/graph/api/resources/schema?view=graph-rest-beta) **, чтобы включить** фильтрацию результатов поиска и более качественное управление опытом поиска, а также **псевдонимы** и **метки** для обеспечения лучшей релевантности.
- Возможность указать в **схеме**до 128 ресурсов **свойств** .
- Используйте [Get екстерналитем](/graph/api/externalitem-get?view=graph-rest-beta) для целей диагностики.

### <a name="users"></a>Пользователи
- Используйте свойство **усерпурпосе** объекта [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) для определения и различения почтового ящика одного пользователя из общего почтового ящика и почтового ящика оборудования в Exchange Online. 
- Используйте [Параметры пользователя](/graph/api/resources/usersettings?view=graph-rest-beta) для [получения](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta) или [обновления](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta) [предпочитаемых лангуаес и региональных параметров](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta).
- Пользовательские параметры — это отношение, доступное [пользователям](/graph/api/resources/user?view=graph-rest-beta) , которое обеспечивает единообразное взаимодействие с пользователем в разных приложениях, нажимая в профиле пользователя Azure AD, чтобы отразить те же предпочтения пользователя. Узнайте, [как параметры пользователя отличаются от параметров почтовых ящиков](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Подпишитесь на [программу для разработчиков microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и начните разработку!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

