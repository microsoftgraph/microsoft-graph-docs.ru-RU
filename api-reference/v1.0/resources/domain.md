---
title: тип ресурса домена
description: Представляет домен, связанный с клиентом.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 62c48eca4f3672113c9eabbee7c420f7e2c9e4c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962464"
---
# <a name="domain-resource-type"></a>тип ресурса домена

Пространство имен: microsoft.graph

Представляет домен, связанный с клиентом.

Используйте операции домена, чтобы связать домены с клиентом, проверить владение доменом и настроить поддерживаемые службы.  Операции домена позволяют регистраторам автоматизировать связь домена для таких служб, как Microsoft 365. Например, в рамках регистрации домена регистратор может включить домен тщеславия для электронной почты, веб-сайтов, проверки подлинности и т.д.

Связать домен с клиентом:

1. [Связать](../api/domain-post-domains.md) домен с клиентом.

2. [Извлечение](../api/domain-list-verificationdnsrecords.md) записей проверки домена. Добавьте сведения о записи проверки в файл зоны домена с помощью регистратора домена или конфигурации сервера DNS.

3. [Проверка](../api/domain-verify.md) владения доменом. Это проверит домен и застроит **свойство isVerified** `true` к .

4. [Указать](../api/domain-update.md) поддерживаемые службы, которые планируется использовать с доменом.

5. [Настройка поддерживаемых](../api/domain-list-serviceconfigurationrecords.md) служб путем ирисовки списка записей, необходимых для обеспечения служб для домена. Добавьте сведения о записи конфигурации в файл зоны домена с помощью регистратора домена или конфигурации сервера DNS.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Получение домена](../api/domain-get.md) | [domain](domain.md); | Чтение свойств и связей объекта домена.|
|[Создание домена](../api/domain-post-domains.md) | [domain](domain.md); | Добавление домена в клиент. |
|[List domainNameReference](../api/domain-list-domainnamereferences.md) |Коллекция [directoryObject](directoryobject.md)| Извлечение списка объектов каталога со ссылкой на домен.|
|[Служба ListConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[коллекция domainDnsRecord](domaindnsrecord.md)|  Извлечение списка записей DNS домена для конфигурации домена.|
|[Проверка спискаDnsRecords](../api/domain-list-verificationdnsrecords.md) |[коллекция domainDnsRecord](domaindnsrecord.md)|  Извлечение списка записей DNS домена для проверки домена.|
|[Обновление домена](../api/domain-update.md) | [domain](domain.md); |Обновляет домен.|
|[Удаление домена](../api/domain-delete.md) | Нет |Удаляет домен.|
|[Домен ForceDelete](../api/domain-forcedelete.md)|Нет|Удаляет домен с помощью асинхронной операции.|
|[Проверка домена](../api/domain-verify.md)|[domain](domain.md);|Проверка права собственности на домен.|

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|authenticationType|String| Указывает настроенный тип проверки подлинности для домена. Значение либо `Managed` или `Federated` . `Managed` указывает на облачный управляемый домен, в котором Azure AD выполняет проверку подлинности пользователей. `Federated` указывает, что проверка подлинности передается поставщику удостоверений, например локальной службе Active Directory клиента с помощью служб Федерации Active Directory. Это свойство является только для чтения и не является недействительным. |
|availabilityStatus|String| Это свойство всегда за `null` исключением случаев, когда [используется](../api/domain-verify.md) действие проверки. Когда используется [действие](../api/domain-verify.md) проверки, **объект домена** возвращается в ответ. Свойство **availabilityStatus** объекта **домена** в ответе либо `AvailableImmediately` или `EmailVerifiedDomainTakeoverScheduled` .|
|id|String| Полное имя домена. Ключ, неуменяемый, не nullable, уникальный. |
|isAdminManaged|Boolean| Значение свойства в том случае, если управление записями DNS домена было делегировано `false` Microsoft 365. В противном случае значение `true` . Не является недействительным |
|isDefault|Boolean| `true` если это домен по умолчанию, используемый для создания пользователя. Существует только один домен по умолчанию для одной компании. Не является недействительным |
|isInitial|Boolean| `true` если это начальный домен, созданный Microsoft Online Services (companyname.onmicrosoft.com). На одну компанию имеется только один начальный домен. Не является недействительным |
|isRoot|Boolean| `true` если домен является проверенным корневым доменом. В `false` противном случае, если домен является поддоменом или непроверенным. Не является недействительным |
|isVerified|Boolean| `true` если домен завершил проверку владения доменом. Не является недействительным |
|passwordNotificationWindowInDays|Int32|Указывает количество дней до получения пользователем уведомления о том, что срок действия пароля истекает. Если свойство не установлено, будет использоваться значение по умолчанию в 14 дней.|
|passwordValidityPeriodInDays|Int32| Указывает продолжительность действия пароля перед его сменой. Если свойство не установлено, будет использоваться значение по умолчанию в 90 дней. |
|supportedServices|Коллекция строк| Возможности, присвоенные домену. Может включать `0` или `1` более следующих значений: `Email` , , , , , , , `Sharepoint` , `EmailInternalRelayOnly` `OfficeCommunicationsOnline` `SharePointDefaultDomain` `FullRedelegation` `SharePointPublic` `OrgIdAuthentication` `Yammer` `Intune` . Значения, которые можно добавить или удалить с помощью API Graph: `Email` , `OfficeCommunicationsOnline` , `Yammer` . Не является недействительным|
|state|[domainState](domainstate.md)| Состояние асинхронных операций, запланированных для домена. |

## <a name="relationships"></a>Связи

Связи между доменом и другими объектами в каталоге, такими как его записи проверки и записи конфигурации служб, подвергаются воздействию с помощью свойств навигации. Эти отношения можно прочитать, нацелив эти свойства навигации в запросах.

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|domainNameReferences|Коллекция [directoryObject](directoryobject.md)| Только для чтения, недействительный|
|serviceConfigurationRecords|[коллекция domainDnsRecord](domaindnsrecord.md)| DNS записи клиента добавляет в DNS-файл зоны домена, прежде чем домен может быть использован службами Microsoft Online. Только для чтения, недействительный |
|verificationDnsRecords|[коллекция domainDnsRecord](domaindnsrecord.md)| DNS записи, которые клиент добавляет в файл зоны DNS домена, прежде чем клиент может завершить проверку владения доменом с помощью Azure AD. Только для чтения, недействительный|

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

