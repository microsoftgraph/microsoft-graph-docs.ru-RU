---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: e26203ef0a8846f611d570d98f30fd17dd6db4b3
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183920"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

В этой статье представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Полный список обновлений API см. в разделах [Июнь](changelog.md#june-2020) и [Май](changelog.md#may-2020) журнала изменений API. 

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и средства, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступного (GA) состояния. Не используйте функции предварительной версии в рабочих приложениях.

## <a name="july-2020-new-and-generally-available"></a>Июль 2020 г.: новые и общедоступные возможности
      
### <a name="change-notifications"></a>Уведомления об изменениях
Удалено ошибочно реализованное свойство **sequenceNumber** из ресурса [changeNotification](/graph/api/resources/changenotification).

### <a name="groups"></a>Группы
Общая доступность следующих свойств объекта [group](/graph/api/resources/group?view=graph-rest-v1.0): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage** и **theme**.

### <a name="identity-and-access"></a>Удостоверение и доступ
Удаление пользователя в качестве зарегистрированного владельца или пользователя [устройства](/graph/api/resources/device).

### <a name="schema-extensions"></a>Расширения схемы
Функция [расширения схемы](/graph/api/resources/schemaextension) теперь общедоступна в [Microsoft Cloud for US Government](/graph/deployments).

## <a name="july-2020-new-in-preview-only"></a>Июль 2020 г.: новые возможности только в предварительной версии

### <a name="cloud-communications"></a>Облачные коммуникации
Подписка на уведомления об изменениях о доступности пользователя в Microsoft Teams, представленной ресурсом [presence](/graph/api/resources/presence?view=graph-rest-beta).

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Использование разрешения приложений `Printer.ReadWrite.All` и [шифрования Internet Printing Protocol (IPP)](https://tools.ietf.org/html/rfc8010) для [обновления принтера](/graph/api/printer-update?view=graph-rest-beta).
- Использование разрешений приложений `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All` или `PrintJob.ReadWrite.All` для [получения задания печати](/graph/api/printjob-get?view=graph-rest-beta) или [перечисления заданий печати для принтера](/graph/api/printer-list-jobs?view=graph-rest-beta).
- При [получении задания печати](/graph/api/printjob-get?view=graph-rest-beta) используйте `$expand` для получения [задач печати](/graph/api/resources/printtask?view=graph-rest-beta), выполняемых или выполненных в рамках задания. Задачи печати, [определения задач](/graph/api/resources/printtaskdefinition?view=graph-rest-beta) и [триггеры задач](/graph/api/resources/printtasktrigger?view=graph-rest-beta) используются при [печати по запросу](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Перенаправление задания печати](/graph/api/printjob-redirect?view=graph-rest-beta) на другой принтер в рамках печати по запросу.

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июль](changelog.md#july-2020) в бета-версии.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Включение уровней риска пользователя (`low`, `medium`, `high`, `none`) при рассмотрении применения [политики условного доступа](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta).
- [Использование смены пароля в качестве предоставления управления](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta#special-considerations-when-using-passwordchange-as-a-control), чтобы пройти политику условного доступа.

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Люди и рабочая аналитика | Настройка карточки профиля
Администраторы могут [настроить свойства, представленные в карточке профиля для своих организаций](add-properties-profilecard.md), используя API-интерфейс для [свойств карточки профиля](/graph/api/resources/profilecardproperty?view=graph-rest-beta).

### <a name="workbooks-and-charts"></a>Книги и диаграммы
[Получение состояния и любого результата](/graph/api/workbookoperation-get?view=graph-rest-beta) длительной [операции](/graph/api/resources/workbookoperation?view=graph-rest-beta) в [книге](/graph/api/resources/workbook?view=graph-rest-beta).

## <a name="june-2020-new-and-generally-available"></a>Июнь 2020 г.: новые и общедоступные возможности

### <a name="cloud-communications--online-meeting"></a>Облачные коммуникации | Онлайн-собрание
- Использование `Accept-Language` заголовка HTTP при [создании онлайнового собрания](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0) для предоставления объединенной информации на основе языковой среды.
- Использование [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0) для возврата онлайнового собрания с указанным значением **externalId** или его создание в случае отсутствия, чтобы упростить внедрение получившегося собрания в стороннем календаре.

### <a name="files"></a>Файлы
- Улучшенная поддержка синхронизации:
  - Использование свойства **pendingOperations** для определения [операций](/graph/api/resources/pendingoperations), которые могут обновить бинарное содержание файла [driveItem](/graph/api/resources/driveitem), ожидающего выполнения.
  - [Восстановление](/graph/api/driveitem-restore) объекта **driveItem**, который был удален и находится в корзине OneDrive персональный.
- Получение или настройка ориентации ресурса [photo](/graph/api/resources/photo). Настройка поддерживается в OneDrive персональный.
- Использование защищенного алгоритма хэширования (SHA-256) для улучшения безопасности и целостности данных ресурса [file](/graph/api/resources/file).
- Использование параметра `deferCommit` для откладывания окончательного создания при [передаче, как правило, большого файла](/graph/api/driveitem-createuploadsession) в OneDrive для бизнеса до тех пор, пока приложение не выполнит запрос на выполнение передачи.
- Использование свойства **fileSize** для предоставления оценки как части параметра **item**, чтобы проверить квоту до [передачи файла](/graph/api/driveitem-createuploadsession) в OneDrive персональный.
- Поиск [storagePlanInformation](/graph/api/resources/storageplaninformation) с помощью свойства **quota** ресурса [drive](/graph/api/resources/drive), чтобы проверить доступность планов с более высокими квотами на хранение.

### <a name="groups"></a>Группы
Использование разрешений приложений `Group.Read.All` и `Group.ReadWrite.All` для получения ресурсов группы [беседа](/graph/api/resources/conversation) и [цепочки беседы](/graph/api/resources/conversationthread).

### <a name="identity-and-access"></a>Удостоверение и доступ 
- Общедоступная версия из двух наборов API для [защиты удостоверения](/graph/api/resources/identityprotectionroot): API [выявления рисков](/graph/api/resources/riskdetection) и [рискованных пользователей](/graph/api/resources/riskyuser).

### <a name="security"></a>Безопасность
- Отслеживание указанного ниже как свойств [оповещения](/graph/api/resources/alert?view=graph-rest-1.0):
  - Идентификаторы инцидентов, связанных с оповещением.
  - Идентификация [ресурса](/graph/api/resources/securityResource?view=graph-rest-1.0#securityresourcetype-values) как атакованного или как связанного ресурса в оповещении.
  - Указание начального и конечного расположений [сетевого подключения](/graph/api/resources/networkconnection?view=graph-rest-1.0), связанных с оповещением.

### <a name="sites-and-lists"></a>Сайты и списки
Указание геолокационных данных в [определении столбца](/graph/api/resources/columndefinition) для ресурса [списка](/graph/api/resources/list) SharePoint.

### <a name="teamwork"></a>Командная работа
- Использование делегированного разрешения [AppCatalog.Read.All](/graph/permissions-reference#appcatalog-resource-permissions) для перечисления [приложений](/graph/api/resources/teamsapp?view=graph-rest-1.0) из каталога приложений Microsoft Teams.
- [Получение информации о папке](/graph/api/channel-get-filesfolder) с сопоставлением вкладки **Файлы** [канала](/graph/api/resources/channel) Teams.
- [Получение канала по умолчанию](/graph/api/team-get-primarychannel) с меткой **Общие** [команды](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Июнь 2020 г.: новые возможности только в предварительной версии

### <a name="calendar"></a>Календарь
Помимо отслеживания инкрементных изменений событий в **calendarView** (коллекции или событий, ограниченных начальными _и_ конечными данными), применяется функция [delta](/graph/api/event-delta?view=graph-rest-beta) к событиям в почтовом ящике пользователя или к событиям в календаре определенного пользователя.

### <a name="cloud-communications--presence"></a>Облачные коммуникации | Присутствие
[Получение статуса присутствия](/graph/api/presence-get?view=graph-rest-beta) всех пользователей в организации или определенного пользователя организации.

### <a name="devices-and-apps--cloud-printing"></a>Устройства и приложения | Облачная печать
- Указание [полей печати](/graph/api/resources/printmargin?view=graph-rest-beta) при настройке [документа для печати](/graph/api/resources/printdocument?view=graph-rest-beta).
- Поддержка следующих [возможностей принтера](/graph/api/resources/printercapabilities?view=graph-rest-beta):
  - направления подачи;
  - печати диапазонов страниц;
  - разрешение печати в точках на дюйм;
  - максимальный размер очереди заданий печати в байтах;
  - входные лотки;
  - поля;
  - разбор по копиям;
  - масштабирование документов.
- Поддержка разрешения печати (в точках на дюйм) и масштабирование документов как часть [настроек принтера по умолчанию](/graph/api/resources/printerdefaults?view=graph-rest-beta).
- Поддержка следующих настроек [конфигурации документов](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta):
  - входные лотки;
  - выходные лотки;
  - размеры носителей;
  - поля;
  - типы носителей;
  - финишная обработка, например сшивание или брошюрование;
  - количество страниц на лист;
  - многостраничный макет с указанием направления при размещении страниц на листе;
  - разбор по копиям;
  - масштабирование.
- Расширение документов при [перечислении заданий печати](/graph/api/printer-list-jobs?view=graph-rest-beta).
- [Регистрация принтера]() и использование ресурса [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta) для отслеживания и проверки регистрации принтера.
- [Получение долгосрочной регистрации принтера](/graph/api/printoperation-get?view=graph-rest-beta) для текущего пользователя или клиента приложения.
- Несколько переименований свойств и типов нумерации. Более подробные сведения приведены в обновлениях журнала изменений для облачной печати за [июнь](changelog.md#june-2020).

### <a name="devices-and-apps--corporate-management"></a>Устройства и приложения | Корпоративное управление
Обновления Intune за [июнь](changelog.md#june-2020) в бета-версии.

### <a name="education"></a>Образование
- Возможность использовать делегированные разрешения `EduRoster.ReadBasic` для [получения](/graph/api/educationuser-get?view=graph-rest-beta) идентификатора [преподавателя](/graph/api/resources/educationteacher?view=graph-rest-beta) или [учащегося](/graph/api/resources/educationstudent?view=graph-rest-beta) во внешней исходной программе как свойство **externalId**.
- Использование свойства **externalSource** для отслеживания значения `lms`, если [организация](/graph/api/resources/educationorganization?view=graph-rest-beta) или [класс](/graph/api/resources/educationclass?view=graph-rest-beta) в сфере образования созданы в системе управления обучением (LMS).

### <a name="identity-and-access"></a>Удостоверение и доступ
- ИТ-специалисты могут использовать ресурсы [connector](/graph/api/resources/connector?view=graph-rest-beta). Это легкие агенты для подключения к [прокси приложения Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy) и [внешней публикации локальных веб-приложений](/graph/api/resources/onpremisespublishing?view=graph-rest-beta), чтобы удаленные пользователи организации могли безопасно получить доступ к этим приложениям.
- Управление [политикой проверки подлинности](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta) на уровне клиента для включения или отключения [регистрации с самообслуживанием](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta) внешних пользователей.
- [Подготовка учетной записи пользователя по требованию](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta) и возможность указывать объекты для выполнения правил подготовки и синхронизации.

### <a name="search"></a>Поиск
- Использование улучшения [свойства](/graph/api/resources/property?view=graph-rest-beta) в [схеме](/graph/api/resources/schema?view=graph-rest-beta) **isRefinable** для включения фильтрации результатов поиска и более точного управления взаимодействием при поиске, а также **псевдонимов** и **меток** для повышения релевантности.
- Возможность указать до 128 ресурсов **свойства** в **схеме**.
- Использование [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta) для диагностики.

### <a name="users"></a>Пользователи
- Использование свойства **userPurpose** [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) для выявления и дифференциации почтового ящика для одного пользователя от общего почтового ящика и почтового ящика оборудования в Exchange Online. 
- Использование [настроек пользователей](/graph/api/resources/usersettings?view=graph-rest-beta) для [получения](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta) или [обновления](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta) [предпочитаемых языков и региональных настроек](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta).
- Настройки пользователей — это взаимосвязь, доступная через [пользователя](/graph/api/resources/user?view=graph-rest-beta), которая обеспечивает единообразное взаимодействие с пользователем в разных приложениях за счет использования профиля Azure AD для применения одних и тех же предпочтений пользователя. См. статью [Чем отличаются пользовательские настройки от настроек почтового ящика](/graph/api/resources/user?view=graph-rest-beta#user-preferences-for-languages-and-regional-formats).


## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?

Вот несколько способов, которые можно использовать.

- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Некоторые новые функции реализуются на основе распространенных запросов сообщества разработчиков. Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

    1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

    2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Microsoft 365](https://developer.microsoft.com/office/dev-program), получите бесплатную подписку на Microsoft 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).

