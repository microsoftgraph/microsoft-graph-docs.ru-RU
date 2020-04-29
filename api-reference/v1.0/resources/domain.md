---
title: Тип ресурса domain
description: Представляет домен, связанный с клиентом.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fea245c8e564c22a28d963c829c094535e540a6e
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181667"
---
# <a name="domain-resource-type"></a>Тип ресурса domain

Пространство имен: microsoft.graph

Представляет домен, связанный с клиентом.

Используйте операции с доменами, чтобы связать домены с клиентом, проверить владение доменом и настроить поддерживаемые службы.  Операции с доменами позволяют регистраторам автоматизировать сопоставление доменов для таких служб, как Office 365. Например, в рамках регистрации в домене регистратор может включить домен запоминающийся для электронной почты, веб-сайтов, проверки подлинности и т. д.

Чтобы связать домен с клиентом:

1. [Свяжите](../api/domain-post-domains.md) домен с клиентом.

2. [Получение](../api/domain-list-verificationdnsrecords.md) записей проверки домена. Добавьте сведения об проверочной записи в файл зоны домена с помощью средства регистратора доменных имен или DNS-сервера.

3. [Проверьте](../api/domain-verify.md) принадлежность домена. Это позволит проверить домен и присвоить свойству *вере* значение *true*.

4. [Укажите](../api/domain-update.md) Поддерживаемые службы, которые планируется использовать в домене.

5. [Настройте](../api/domain-list-serviceconfigurationrecords.md) Поддерживаемые службы, получая список записей, необходимых для включения служб для домена. Добавьте сведения о записи конфигурации в файл зоны домена с помощью средства регистратора доменных имен или DNS-сервера.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Получение домена](../api/domain-get.md) | [domain](domain.md); | Чтение свойств и связей объекта домена.|
|[Создание домена](../api/domain-post-domains.md) | [domain](domain.md); | Добавление домена в клиент. |
|[Список domainNameReference](../api/domain-list-domainnamereferences.md) |Коллекция [directoryObject](directoryobject.md)| Получение списка объектов каталога со ссылкой на домен.|
|[Список serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |Коллекция [domainDnsRecord](domaindnsrecord.md)|  Получение списка DNS-записей домена для настройки домена.|
|[Список verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |Коллекция [domainDnsRecord](domaindnsrecord.md)|  Получение списка DNS-записей домена для проверки домена.|
|[Обновление домена](../api/domain-update.md) | [domain](domain.md); |Обновляет домен.|
|[Удаление домена](../api/domain-delete.md) | Нет |Удаляет домен.|
|[Домен Форцеделете](../api/domain-forcedelete.md)|Нет|Удаляет домен, используя асинхронную операцию.|
|[Verify domain](../api/domain-verify.md)|[domain](domain.md);|Проверка права собственности на домен.|

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|authenticationType|String| Указывает настроенный тип проверки подлинности для домена. Значение может быть *управляемым* или *федеративными*.<br> *Managed* указывает облачный управляемый домен, в котором Azure AD выполняет проверку подлинности пользователей.<br>*Федеративная* указывает на то, что проверка подлинности федеративного поставщика удостоверений, например локальной службы Active Directory клиента, через службы федерации Active Directory. Это свойство доступно только для чтения и не может иметь значение null. |
|availabilityStatus|String| Это свойство всегда имеет значение null, за исключением случаев, когда используется действие [проверки](../api/domain-verify.md) . При использовании действия [Verify](../api/domain-verify.md) в ответе возвращается **Доменная** сущность. Свойство **аваилабилитистатус** объекта **domain** в отклике имеет значение *аваилаблеиммедиатели* или *емаилверифиеддомаинтакеоверсчедулед*.|
|id|String| Полное доменное имя домена. Key, неизменяемая, не допускающая значение null, уникальная |
|исадминманажед|Boolean| Значение свойства равно false, если управление записями DNS домена было делегировано в Office 365. В противном случае — значение true. Не допускает значение null |
|isDefault|Boolean| Значение true, если это домен по умолчанию, используемый для создания пользователя. Для каждой компании существует только один домен по умолчанию. Не допускает значение null |
|при инициализации|Boolean| Имеет значение true, если это начальный домен, созданный Microsoft Online Services (companyname.onmicrosoft.com). Для каждой компании существует только один начальный домен. Не допускает значение null |
|Корень|Boolean| True, если домен является проверенным корневым доменом. В противном случае — false, если домен является поддоменом или непроверенным. Не допускает значение null |
|Проверка|Boolean| True, если домен выполнил проверку владения доменом. Не допускает значение null |
|пассворднотификатионвиндовиндайс|Int32|Указывает количество дней до того, как пользователь получит уведомление о том, что срок действия пароля не истечет. Если свойство не задано, будет использоваться значение по умолчанию (14 дней).|
|пассвордвалидитипериодиндайс|Int32| Указывает период времени, в течение которого пароль должен быть действителен до его изменения. Если свойство не задано, будет использоваться значение по умолчанию (90 дней). |
|суппортедсервицес|Коллекция объектов string| Возможности, назначенные для домена.<br><br>Может содержать 0, 1 или более следующих значений: *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*<br><br> При использовании Graph API можно добавить или удалить следующие значения: *Email*, *OfficeCommunicationsOnline*, *Yammer*<br>Не допускает значение null|
|state|[домаинстате](domainstate.md)| Состояние асинхронных операций, запланированных для домена. |

## <a name="relationships"></a>Связи

Отношения между доменом и другими объектами в каталоге, такими как записи проверки и записи конфигурации службы, предоставляются через свойства навигации. Эти отношения можно прочитать, нацеливания эти свойства навигации в запросах.

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|домаиннамереференцес|Коллекция [directoryObject](directoryobject.md)| Только для чтения, Nullable|
|serviceConfigurationRecords|Коллекция [domainDnsRecord](domaindnsrecord.md)| DNS-записи, которые клиент добавляет в файл зоны DNS домена, прежде чем домен можно будет использовать в Microsoft Online Services.<br>Только для чтения, Nullable |
|verificationDnsRecords|Коллекция [domainDnsRecord](domaindnsrecord.md)| DNS-записи, которые клиент добавляет в файл зоны DNS домена, прежде чем клиент сможет выполнять проверку владения доменом с помощью Azure AD.<br>Только для чтения, Nullable|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "passwordNotificationWindowInDays": 14,
  "passwordValidityPeriodInDays": 90,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
