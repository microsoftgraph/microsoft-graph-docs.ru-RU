---
title: Тип ресурса domain
description: Представляет домен, связанный с клиентом.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9474d476a27fe0822955ae7bbc4147a5f4a8949c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979763"
---
# <a name="domain-resource-type"></a>Тип ресурса domain

Представляет домен, связанный с клиентом.

Это ресурс позволяет связать домены с клиентом, подтвердить право собственности на домен и настроить поддерживаемые службы.  С его помощью регистраторы могут автоматизировать связь домена для таких служб, как Office 365. Например, в процессе регистрации домена регистратор может включить личный домен для электронной почты, веб-сайтов, аутентификации и т. д.

Чтобы связать домен с клиентом:

1. [Свяжите](../api/domain-post-domains.md) домен с клиентом.

2. [Получите](../api/domain-list-verificationdnsrecords.md) записи о проверке домена. Добавьте сведения из записи о проверке в файл зоны домена, используя конфигурацию регистратора доменных имен или DNS-сервера.

3. [Подтвердите](../api/domain-verify.md) право собственности на домен. После этого для свойства *isVerified* будет установлено значение *true*.

4. [Укажите](../api/domain-update.md) поддерживаемые службы, которые вы планируете использовать в домене.

5. [Настройте](../api/domain-list-serviceconfigurationrecords.md) поддерживаемые службы, получив список записей, необходимых для работы служб домена. Добавьте данные из записи конфигурации в файл зоны домена, используя конфигурацию регистратора доменных имен или DNS-сервера.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Получение домена](../api/domain-get.md) | [domain](domain.md) | Чтение свойств и отношений объекта domain.|
|[Создание домена](../api/domain-post-domains.md) | [domain](domain.md) | Добавление домена в клиент. |
|[Перечисление domainNameReference](../api/domain-list-domainnamereferences.md) |Коллекция [directoryObject](directoryobject.md)| Получение списка объектов каталога со ссылкой на домен.|
|[Перечисление serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |Коллекция [domainDnsRecord](domaindnsrecord.md)|  Получение списка записей DNS домена для настройки домена.|
|[Перечисление verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |Коллекция [domainDnsRecord](domaindnsrecord.md)|  Получение списка записей DNS домена для проверки домена.|
|[Обновление домена](../api/domain-update.md) | [domain](domain.md) |Обновление домена.|
|[Удаление домена](../api/domain-delete.md) | Нет |Удаление домена.|
|[ForceDelete домена](../api/domain-forcedelete.md)|Нет|Удаление домена, с помощью асинхронной операции.|
|[Проверка домена](../api/domain-verify.md)|[domain](domain.md)|Проверка права собственности на домен.|

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|authenticationType|Строка| Указывает тип аутентификации, настроенный для домена. Возможные значения: *Managed* и *Federated*.<br> *Managed* означает управляемый домен, аутентификацию пользователей в котором выполняет Azure AD.<br>*Federated* означает, что аутентификацию выполняет поставщик удостоверений, например локальная служба Active Directory клиента, через службы федерации Active Directory (AD FS). Не допускает значение null. |
|availabilityStatus|Строка| Это свойство всегда имеет значение null, когда не используется действие [verify](../api/domain-verify.md). Когда используется действие [verify](../api/domain-verify.md), в ответе возвращается объект **domain**. Свойство **availabilityStatus** объекта **domain** в ответе — либо *AvailableImmediately*, либо *EmailVerifiedDomainTakeoverScheduled*.|
|id|Строка| Полное имя домена. Ключ, неизменяемое, не допускает значение null, уникальное. |
|isAdminManaged|Логический| Свойство имеет значение false, если управление записью DNS домена делегировано в Office 365. В противном случае возвращается значение true. Не допускает значение null. |
|isDefault|Логический| Значение true, если это домен по умолчанию, который используется для создания пользователя. У компании может быть только один домен по умолчанию. Не допускает значение null. |
|isInitial|Логический| Значение true, если это исходный домен, созданный веб-службами Майкрософт (companyname.onmicrosoft.com). У компании может быть только один исходный домен. Не допускает значение null. |
|isRoot|Логический| Значение true, если это проверенный корневой домен. Значение false, если домен является поддоменом или не проверен. Не допускает значение null. |
|isVerified|Логический| Значение true, если право собственности на домен подтверждено. Не допускает значение null. |
|supportedServices|Коллекция String| Возможности, назначенные домену.<br><br>Могут включать ноль, одно или несколько из следующих значений: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.<br><br> Значения, которые можно добавлять и удалять с помощью API Graph: *Email*, *OfficeCommunicationsOnline*, *Yammer*.<br>Не допускает значение null.|
|state|[domainState](domainstate.md)| Состояние асинхронных операций, запланированных для домена. |

## <a name="relationships"></a>Связи

Отношения между доменом и другими объектами в каталоге, такими как записи проверки и записи конфигурации служб, предоставляются через свойства навигации. Сведения о таких отношениях можно прочесть, указав соответствующие свойства навигации в запросах.

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|domainNameReferences|Коллекция [directoryObject](directoryobject.md)| Только для чтения, допускает значение null.|
|serviceConfigurationRecords|Коллекция [domainDnsRecord](domaindnsrecord.md)| DNS-записи, которые клиент добавляет в файл зоны DNS домена, чтобы использовать домен с Microsoft Online Services.<br>Только для чтения, допускает значение null. |
|verificationDnsRecords|Коллекция [domainDnsRecord](domaindnsrecord.md)| DNS-записи, которые клиент добавляет в файл зоны DNS домена, чтобы подтвердить право собственности на домен в Azure AD.<br>Только для чтения, допускает значение null.|

## <a name="json-representation"></a>Представление в формате JSON
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
