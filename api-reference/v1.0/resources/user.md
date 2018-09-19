# <a name="user-resource-type"></a>Тип ресурса user

Представляет учетную запись пользователя Azure AD. Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает:

- Добавление собственных данных к настраиваемым свойствам в качестве [расширений](../../../concepts/extensibility_overview.md).
- Подписка на [уведомления об изменении](../../../concepts/webhooks.md).
- Использование [разностного запроса](../../../concepts/delta_query_overview.md) для отслеживания изменений, связанных с добавлениями, удалениями и обновлениями, при помощи функции [delta](../api/user_delta.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление пользователей](../api/user_list.md) |Коллекция объектов [user](user.md)| Получение списка, включающего объекты user.|
|[Создание пользователя](../api/user_post_users.md) |[пользователь](user.md)| Создание объекта user.|
|[Получение пользователя](../api/user_get.md) | [пользователь](user.md) |Чтение свойств и связей объекта пользователя.|
|[Обновление пользователя](../api/user_update.md) | [пользователь](user.md) |Обновление объекта пользователя. |
|[Удаление пользователя](../api/user_delete.md) | Нет |Удаление объекта пользователя. |
|[Список сообщений](../api/user_list_messages.md) |Коллекция [Message](message.md)| Получение всех сообщений в почтовом ящике вошедшего пользователя.|
|[Создание объекта Message](../api/user_post_messages.md) |[Message](message.md)| Создание объекта Message путем добавления в коллекцию сообщений.|
|[Список объектов mailFolder](../api/user_list_mailfolders.md) |Коллекция [MailFolder](mailfolder.md)| Получение коллекции папок почты в корневой папке вошедшего пользователя. |
|[Создание объекта MailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| Создание объекта MailFolder путем добавления в коллекцию папок почты.|
|[sendMail](../api/user_sendmail.md)|Нет|Отправка сообщения, указанного в теле запроса.|
|[Получение списка событий](../api/user_list_events.md) |Коллекция [Event](event.md)| Получение списка объектов event в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/user_post_events.md) |[Event](event.md)| Создание объекта Event путем добавления в коллекцию событий.|
|[Список календарей](../api/user_list_calendars.md) |Коллекция [Calendar](calendar.md)| Получение коллекции объектов Calendar.|
|[Создание календаря](../api/user_post_calendars.md) |[Calendar](calendar.md)| Создание объекта Calendar путем добавления в коллекцию календарей.|
|[Список объектов calendarGroup](../api/user_list_calendargroups.md) |Коллекция [CalendarGroup](calendargroup.md)| Получение коллекции объектов CalendarGroup.|
|[Создание объекта calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Создание объекта CalendarGroup путем записи в коллекцию групп календарей.|
|[Список calendarView](../api/user_list_calendarview.md) |Коллекция [Event](event.md)| Получение коллекции объектов Event.|
|[Список контактов](../api/user_list_contacts.md) |Коллекция [Contact](contact.md)| Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя.|
|[Создание контакта](../api/user_post_contacts.md) |[Contact](contact.md)| Создание объекта Contact путем добавления в коллекцию контактов.|
|[Список объектов contactFolder](../api/user_list_contactfolders.md) |Коллекция [ContactFolder](contactfolder.md)| Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.|
|[Создание объекта ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| Создание объекта ContactFolder путем добавления в коллекцию папок контактов.|
|[Список directReports](../api/user_list_directreports.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей и контактов, являющихся подчиненными данного пользователя, из свойства навигации directReports.|
|[Получение руководителя](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | Получение пользователя или контакта, являющегося руководителем пользователя, из свойства навигации manager.|
|[Список memberOf](../api/user_list_memberof.md) |Коллекция [directoryObject](directoryobject.md)| Получение групп и ролей каталога, непосредственным участником которых является пользователь, из свойства навигации memberOf.|
|[Список ownedDevices](../api/user_list_owneddevices.md) |Коллекция [directoryObject](directoryobject.md)| Получение устройств, принадлежащих пользователю, из свойства навигации ownedDevices.|
|[Список ownedObjects](../api/user_list_ownedobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение объектов каталога, принадлежащих пользователю, из свойства навигации ownedObjects.|
|[Список registeredDevices](../api/user_list_registereddevices.md) |Коллекция [directoryObject](directoryobject.md)| Получение устройств, зарегистрированных для пользователя, из свойства навигации registeredDevices.|
|[Список createdObjects](../api/user_list_createdobjects.md) |Коллекция [directoryObject](directoryobject.md)| Получение объектов каталога, созданных пользователем, из свойства навигации createdObjects.|
|[assignLicense](../api/user_assignlicense.md)|[пользователь](user.md)|Добавление или удаление подписок пользователя. Вы также можете включать и отключать отдельные планы, связанные с подпиской.|
|[Перечисление licenseDetails](../api/user_list_licensedetails.md) |Коллекция объектов [licenseDetails](licensedetails.md)| Получение коллекции объектов licenseDetails.|
|[checkMemberGroups](../api/user_checkmembergroups.md)|Коллекция строк|Проверка членства в списке групп. Это транзитивная проверка.|
|[getMemberGroups](../api/user_getmembergroups.md)|Коллекция строк|Возвращает все группы, в которых состоит пользователь. Это транзитивная проверка.|
|[getMemberObjects](../api/user_getmemberobjects.md)|Коллекция строк| Возвращает все группы и роли каталога, участником которых является пользователь. Это транзитивная проверка. |
|[reminderView](../api/user_reminderview.md)|Коллекция [Reminder](reminder.md)|Возвращает список напоминаний календаря за указанный период времени.|
|[delta](../api/user_delta.md)|Коллекция пользователей| Получение добавочных изменений для пользователей. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../../../concepts/extensibility_schema_groups.md) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|aboutMe|Строка|Свободное текстовое поле, где пользователь может рассказать о себе.|
|accountEnabled|Логический| Значение **true** указывает на то, что учетная запись включена. В противном случае используется значение **false**. Это свойство обязательно использовать при создании пользователя. Поддерживает $filter.    |
|ageGroup|Строка|Задает возрастную группу пользователя. Допустимые значения: `null`, `minor`, `notAdult` и `adult`. Обратитесь к [определению свойств группы возраста юридической дееспособности](#legal-age-group-property-definitions) для получения дополнительных сведений. |
|assignedLicenses|Коллекция [assignedLicense](assignedlicense.md)|Лицензии, назначенные пользователю. Значение null не допускается.            |
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|Планы, назначенные пользователю. Только для чтения. Значение null не допускается. |
|birthday|DateTimeOffset|День рождения пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`|
|businessPhones|Коллекция строк|Номера телефонов пользователя. ПРИМЕЧАНИЕ. Несмотря на то что это коллекция строк, в качестве этого свойства можно указать только одно число.|
|city|Строка|Город, в котором находится пользователь. Поддерживает параметр $filter.|
|companyName | Строка | Название организации, с которой связан пользователь. Только для чтения. |
|consentProvidedForMinor|Строка|Задает, было ли получено разрешение для несовершеннолетних лиц. Допустимые значения: `null`, `granted`, `denied` и `notRequired`. Обратитесь к [определению свойств группы возраста юридической дееспособности](#legal-age-group-property-definitions) для получения дополнительных сведений.|
|country|Строка|Страна или регион, в котором находится пользователь, например "США" или "Соединенное Королевство". Поддерживает параметр $filter.|
|createdDateTime | DateTimeOffset |Дата создания объекта пользователя. |
|department|Строка|Название отдела, в котором работает пользователь. Поддерживает параметр $filter.|
|displayName|Строка|Отображаемое имя пользователя в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. Поддерживает параметры $filter и $orderby.|
|givenName|Строка|Простое имя пользователя. Поддерживает параметр $filter.|
|hireDate|DateTimeOffset|Дата найма пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`|
|id|Строка|Уникальный идентификатор пользователя. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|imAddresses|Коллекция строк|Адреса SIP/VoIP для пользователя. Только для чтения.|
|interests|Коллекция строк|Список интересов пользователя.|
|jobTitle|Строка|Должность пользователя. Поддерживает $filter.|
|legalAgeGroupClassification|Строка| Используется корпоративными приложениями для определения группы возраста юридической дееспособности пользователя. Это свойство предназначается только для чтения и вычисляемых на основе `ageGroup` и `consentProvidedForMinor` свойств. Допустимые значения: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` и `adult`. Обратитесь к [определению свойств группы возраста юридической дееспособности](#legal-age-group-property-definitions) для получения дополнительных сведений.|
|mail|Строка|SMTP-адрес пользователя, например "gregory@contoso.onmicrosoft.com". Только для чтения. Поддерживает параметр $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Параметры основного почтового ящика пользователя, выполнившего вход. Вы можете [получить](../api/user_get_mailboxsettings.md) или [обновить](../api/user_update_mailboxsettings.md) параметры языкового стандарта, часового пояса, отправки автоматических ответов на входящие сообщения.|
|mailNickname|Строка|Почтовый псевдоним для пользователя. Это свойство должно быть указано при создании пользователя. Поддерживает параметр $filter.|
|mobilePhone|Строка|Основной сотовый телефон пользователя.|
|mySite|Строка|URL-адрес личного сайта пользователя.|
|officeLocation|Строка|Расположение офиса на месте работы пользователя.|
|onPremisesDomainName|Строка| Содержит локальный объект `domainFQDN`, также называемый dnsDomainName, который синхронизируется из локального каталога. Свойство заполняется только для клиентов, которые выполняют синхронизацию своего локального каталога для Azure Active Directory с помощью Azure AD Connect. Только для чтения. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|Содержит extensionAttributes 1 – 15 для пользователя. Обратите внимание, что атрибуты отдельных расширения не доступны ни для выбор, ни для фильтрации. Для пользователя `onPremisesSyncEnabled` этот набор свойств создается локально и доступен только для чтения. Для пользователя только в облаке (где `onPremisesSyncEnabled` имеет значение false) эти свойства могут быть установлены во время создания или обновления. |
|onPremisesImmutableId|Строка|Это свойство используется для сопоставления локальной учетной записи Active Directory с объектом пользователя Azure AD. Его необходимо указывать при создании учетной записи пользователя в Graph, если в качестве свойства **userPrincipalName** (имени участника-пользователя) используется федеративный домен. **Важно!** В этом свойстве не допускается использование символов **$** и **_**. Поддерживает параметр $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Указывает время последней синхронизации объекта с локальным каталогом, например: "2013-02-16T03:04:54Z". Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|onPremisesProvisioningErrors|Коллекция [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Ошибки при использовании синхронизации продукта Майкрософт во время подготовки. |
|onPremisesSamAccountName|Строка| Содержит локальной объект, `samAccountName` который синхронизируется из локального каталога. Свойство заполняется только для клиентов, которые выполняют синхронизацию своего локального каталога для Azure Active Directory с помощью Azure AD Connect. Только для чтения. |
|onPremisesSecurityIdentifier|Строка|Содержит локальный идентификатор безопасности (SID) локальной группы, синхронизированной с облаком. Только для чтения.|
|onPremisesSyncEnabled|Логическое| Значение **true** указывает, что этот объект синхронизируется из локального каталога. Значение **false** указывает, что этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Значение **null** указывает, что этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). Только для чтения |
|onPremisesUserPrincipalName|Строка| Содержит локальной объект, `userPrincipalName` который синхронизируется из локального каталога. Свойство заполняется только для клиентов, которые выполняют синхронизацию своего локального каталога для Azure Active Directory с помощью Azure AD Connect. Только для чтения. |
|passwordPolicies|Строка|Задает политики паролей для пользователя. Это свойство представляет собой перечисление с единственным возможным значением — "DisableStrongPassword". Оно позволяет использовать менее надежные пароли, чем предусмотрено политикой по умолчанию. Вы также можете указать значение "DisablePasswordExpiration". Эти значения можно указать одновременно. Пример: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Задает профиль пароля для пользователя. Профиль содержит пароль пользователя. Это свойство обязательно указывать при создании пользователя. Пароль в профиле должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies**. По умолчанию требуется надежный пароль.|
|pastProjects|Коллекция строк|Список предыдущих проектов пользователя.|
|postalCode|Строка|Почтовый индекс адреса пользователя. Формат почтового индекса зависит от страны или региона пользователя. В США для этого атрибута используется ZIP-код.|
|preferredLanguage|Строка|Предпочитаемый язык для пользователя. Он должен быть представлен в формате ISO 639-1, например "ru-RU".|
|preferredName|Строка|Предпочитаемое имя пользователя.|
|provisionedPlans|Коллекция [ProvisionedPlan](provisionedplan.md)|Планы, подготовленные для пользователя. Только для чтения. Значение null не допускается. |
|proxyAddresses|Коллекция строк|Пример: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. В выражениях фильтра для свойств с несколькими значениями требуется оператор **any**. Только для чтения. Значение null не допускается. Поддерживает параметр $filter.          |
|responsibilities|Коллекция строк|Список обязанностей пользователя.|
|schools|Коллекция строк|Список учебных заведений, которые посещал пользователь.|
|skills|Коллекция строк|Список навыков пользователя.|
|state|Строка|Область, республика, край или округ в адресе пользователя. Поддерживает параметр $filter.|
|streetAddress|Строка|Почтовый адрес места работы пользователя.|
|surname|Строка|Фамилия пользователя. Поддерживает параметр $filter.|
|usageLocation|Строка|Двухбуквенный код страны (по стандарту ISO 3166). Необходим для пользователей, которым будут назначены лицензии, в связи с законодательным требованием проверять доступность служб в разных странах.  Примеры: "RU", "JP" и "GB". Значение null не допускается. Поддерживает параметр $filter.|
|userPrincipalName|Строка|Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. Доступ к проверенным доменам клиента можно получить с помощью свойства **verifiedDomains** объекта [organization](organization.md). Поддерживает параметры $filter и $orderby.
|userType|Строка|Строковое значение, с помощью которого можно классифицировать типы пользователей в каталоге, например, как «Участник» и «Гость». Поддерживает $filter.          |

### <a name="legal-age-group-property-definitions"></a>Определения свойств группы возраста юридической дееспособности

В этом разделе объясняется, как три свойства группы возраста (`legalAgeGroupClassification`, `ageGroup` и `consentProvidedForMinor`) используются администраторами Azure AD и разработчиками корпоративных приложений, чтобы обеспечить соблюдение нормативов, связанных с возрастными ограничениями.

Например, Кэмерон является администратором справочника начальной школы в деревне Холипорт в Великобритании. В начале учебного года он использует формы документации приемной комиссии для получения разрешения от родителей несовершеннолетнего учащегося в соответствии с нормативами Великобритании, связанных с возрастными ограничениями. Разрешение, полученное от родителя, позволяет школе Холипорта и приложениям Майкрософт использовать учетную запись несовершеннолетнего учащегося. Затем Кэмерон создает все учетные записи и задает значение "minor" (несовершеннолетний) для параметра ageGroup (группа возраста) и значение "granted" (предоставлено) для параметра consentProvidedForMinor (предоставление разрешения для несовершеннолетнего). После этого приложения, используемые его учащимися, могут отключать функции, которые ограничивают доступ для несовершеннолетних.

#### <a name="legal-age-group-classification"></a>Классификация группы возраста юридической дееспособности

Это свойство, предназначенное только для чтения, используется разработчиками корпоративных приложений для обеспечения взаимодействия с пользователем в соответствии с его группой возраста юридической дееспособности. Оно вычисляется на основе свойств `ageGroup` и `consentProvidedForMinor` пользователя.

| Значение    | #  |Описание|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию, параметр `ageGroup` не был задан для пользователя.|
|minorWithoutParentalConsent |1|(Зарезервировано для будущего использования)|
|minorWithParentalConsent|2| Пользователь считается несовершеннолетним на основании нормативов, связанных с возрастными ограничениями, которые действуют в его стране или регионе. Администратор учетной записи получил соответствующее разрешение от родителя или опекуна.|
|adult|3|Пользователь, считающийся взрослым на основании нормативов, связанных с возрастными ограничениями, которые действуют в его стране или регионе.|
|notAdult|4|Пользователь проживает в стране или регионе, где применяются дополнительные нормативы, связанные с возрастными ограничениями (например, США, Великобритания, Европейский союз или Южная Корея), а возраст пользователя находится в пределах между возрастом несовершеннолетнего и взрослого (в соответствии с правилами данной страны или региона). Как правило, это означает, что подростки считаются `notAdult` в регулируемых странах.|
|minorNoParentalConsentRequired|5|Пользователь является несовершеннолетним, но он проживает в стране или регионе, где не применяются нормативы, связанные с возрастными ограничениями.|

#### <a name="age-group-and-minor-consent"></a>Группа возраста и разрешение для несовершеннолетних

Свойства группы возраста и разрешения для несовершеннолетних – это необязательные свойства, используемые администраторами Azure AD, чтобы гарантировать, что использование учетной записи производится надлежащим образом на основании связанных с возрастными ограничениями нормативных правил, которые действуют в стране или регионе пользователя.

#### <a name="agegroup-property"></a>Свойство ageGroup

| Значение    | #  |Описание|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию, параметр `ageGroup` не был задан для пользователя.|
|minor|1|Пользователь считается несовершеннолетним.|
|notAdult|2|Пользователь проживает в стране, где действуют соответствующие нормативные положения (США, Великобритания, Европейский союз или Южная Корея), а возраст пользователя превышает максимальный возраст ребенка (согласно правилам страны) и меньше, чем нижний предел возраста для взрослых (в соответствии с правилами данной страны или региона). По сути, подростки считаются `notAdult` в регулируемых странах.|
|adult|3|Пользователя следует считать взрослым.|

#### <a name="consentprovidedforminor-property"></a>Свойство consentProvidedForMinor

| Значение    | #  |Описание|
|:---------------|:--------|:----------|
|null|0|Значение по умолчанию, параметр `consentProvidedForMinor` не был задан для пользователя.|
|granted|1|Согласие на предоставление учетной записи пользователю было получено.|
|denied|2|Согласие на предоставление учетной записи пользователю не было получено.|
|notRequired|3|Место проживания пользователя не требует согласия.|
 
## <a name="relationships"></a>Связи

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|activities|Коллекция объектов [userActivity](projectrome_activity.md)|Действия пользователя по устройствам. Только для чтения. Допускается значение null.|
|calendar|[Calendar](calendar.md)|Основной календарь пользователя. Только для чтения.|
|calendarGroups|Коллекция [CalendarGroup](calendargroup.md)|Группы календарей пользователя. Только для чтения. Допускается значение null.|
|calendarView|Коллекция [Event](event.md)|Представление календаря. Только для чтения. Допускается значение null.|
|calendars|Коллекция [Calendar](calendar.md)|Календари пользователя. Только для чтения. Допускается значение null.|
|contactFolders|Коллекция [ContactFolder](contactfolder.md)|Папки контактов пользователя. Только для чтения. Допускается значение null.|
|contacts|Коллекция [Contact](contact.md)|Контакты пользователя. Только для чтения. Допускается значение null.|
|createdObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, созданные пользователем. Только для чтения. Допускается значение null.|
|directReports|Коллекция [directoryObject](directoryobject.md)|Пользователи и контакты, являющиеся подчиненными пользователя (пользователи и контакты, у которых в свойстве manager указан этот пользователь). Только для чтения. Допускается значение null. |
|drive|[drive](drive.md)|Хранилище OneDrive пользователя. Только для чтения.|
|drives|Коллекция [drive](drive.md)| Коллекция дисков, доступных для этого пользователя. Только для чтения. |
|events|Коллекция [Event](event.md)|События пользователя. По умолчанию отображаются события в стандартном календаре. Только для чтения. Допускается значение null.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для пользователя. Только для чтения. Допускается значение null.|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | Классификация релевантности сообщений пользователя, основанная на явных обозначениях, переопределяющих заданные параметры релевантности или важности. |
|licenseDetails|Коллекция [LicenseDetails](licensedetails.md)|Коллекция сведений о лицензии для этого пользователя. Допускается значение null.|
|mailFolders|Коллекция [MailFolder](mailfolder.md)| Почтовые папки пользователя. Только для чтения. Допускается значение null.|
|manager|[directoryObject](directoryobject.md)|Пользователь или контакт, являющийся руководителем пользователя. Только для чтения. (Методы HTTP: GET, PUT, DELETE.)|
|memberOf|Коллекция [directoryObject](directoryobject.md)|Группы и роли каталога, участником которых является пользователь. Только для чтения. Допускается значение null.|
|messages|Коллекция [Message](message.md)|Сообщения в почтовом ящике или папке. Только для чтения. Допускается значение null.|
|onenote|[Onenote](onenote.md)| Только для чтения.|
|outlook|[OutlookUser](outlookuser.md)| Только для чтения.|
|ownedDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, принадлежащие пользователю. Только для чтения. Допускается значение null.|
|ownedObjects|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, принадлежащие пользователю. Только для чтения. Допускается значение null.|
|people|Коллекция объектов [person](person.md)| Люди, которые относятся к пользователю. Только для чтения. Допускается значение null.
|photo|[profilePhoto](profilephoto.md)| Фотография профиля пользователя. Только для чтения.|
|planner|[plannerUser](planneruser.md)| Точка входа в ресурс Планировщика, который может существовать для пользователя. Только для чтения.|
|registeredDevices|Коллекция [directoryObject](directoryobject.md)|Устройства, зарегистрированные для пользователя. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в группы с помощью расширений схемы](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
