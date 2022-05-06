---
title: Тип ресурса домена
description: Представляет домен, связанный с клиентом.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: bcc45acf0bab837c9724967bb826e37d55573c83
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246701"
---
# <a name="domain-resource-type"></a>Тип ресурса домена

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет домен, связанный с клиентом.

Используйте операции домена, чтобы связать домены с клиентом, проверить владение доменом и настроить поддерживаемые службы.  Операции домена позволяют регистраторам автоматизировать сопоставление домена для таких служб, как Microsoft 365. Например, в рамках регистрации домена регистратор может включить личный домен для электронной почты, веб-сайтов, проверки подлинности и т. д.

Чтобы связать домен с клиентом:

1. [Свяжите](../api/domain-post-domains.md) домен с клиентом.

2. [Получение](../api/domain-list-verificationdnsrecords.md) записей проверки домена. Добавьте сведения о записи проверки в файл зоны домена с помощью регистратора домена или конфигурации DNS-сервера.

3. [Проверьте](../api/domain-verify.md) владение доменом. Это позволит проверить домен и задать для **свойства isVerified** значение `true`.

4. [Укажите](../api/domain-update.md) поддерживаемые службы, которые вы планируете использовать с доменом.

5. [Настройте](../api/domain-list-serviceconfigurationrecords.md) поддерживаемые службы, извлекая список записей, необходимых для включения служб для домена. Добавьте сведения о записи конфигурации в файл зоны домена с помощью регистратора домена или конфигурации DNS-сервера.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип |Описание|
|:---------------|:--------|:----------|
|[Получение домена](../api/domain-get.md) | [domain](domain.md); | Чтение свойств и связей объекта домена.|
|[Создание домена](../api/domain-post-domains.md) | [domain](domain.md); | Добавление домена в клиент. |
|[Список доменов](../api/domain-list.md) | [domain](domain.md); | Получение всех доменов, связанных с клиентом. |
|[Перечисление domainNameReference](../api/domain-list-domainnamereferences.md) |Коллекция [directoryObject](directoryobject.md)| Получение списка объектов каталога со ссылкой на домен.|
|[Перечисление объектов serviceConfigurationRecord](../api/domain-list-serviceconfigurationrecords.md) |[Коллекция domainDnsRecord](domaindnsrecord.md)|  Получение списка записей DNS домена для конфигурации домена.|
|[Перечисление объектов verificationDnsRecord](../api/domain-list-verificationdnsrecords.md) |[Коллекция domainDnsRecord](domaindnsrecord.md)|  Получение списка записей DNS домена для проверки домена.|
|[Обновление домена](../api/domain-update.md) | [domain](domain.md); |Обновляет домен.|
|[Удаление домена](../api/domain-delete.md) | Нет |Удаляет домен.|
|[Домен ForceDelete](../api/domain-forcedelete.md)|Нет|Удаляет домен с помощью асинхронной операции.|
|[Проверка домена](../api/domain-verify.md)|[domain](domain.md);|Проверка права собственности на домен.|

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|authenticationType|String| Указывает настроенный тип проверки подлинности для домена. Значение равно "или `Managed` " `Federated`. `Managed`указывает облачный управляемый домен, Azure AD выполняет проверку подлинности пользователя. `Federated`указывает, что проверка подлинности выполняется в федерации с поставщиком удостоверений, таким как клиентский локальная служба Active Directory через службы федерации Active Directory (AD FS). Это свойство доступно только для чтения и не допускает значения NULL. |
|availabilityStatus|String| Это свойство всегда за исключением `null` [случаев, когда](../api/domain-verify.md) используется действие проверки. При использовании [действия](../api/domain-verify.md) проверки **в** ответе возвращается сущность домена. Свойство **availabilityStatus** сущности **домена** в ответе имеет значение либо `AvailableImmediately` .`EmailVerifiedDomainTakeoverScheduled`|
|id|String| Полное имя домена. Ключ, неизменяемый, не допускающий значения NULL, уникальный. |
|isAdminManaged|Boolean| Значение свойства равно, `false` если управление записями DNS домена делегировано Microsoft 365. В противном случае значение равно `true`. Не допускает значения NULL |
|isDefault|Boolean| `true` Значение , если это домен по умолчанию, используемый для создания пользователя. Существует только один домен по умолчанию для каждой компании. Не допускает значения NULL |
|isInitial|Boolean| `true` Значение , если это исходный домен, созданный службами Microsoft Online Services (companyname.onmicrosoft.com). Существует только один исходный домен для каждой компании. Не допускает значения NULL |
|isRoot|Boolean| `true` Значение , если домен является проверенным корневым доменом. В противном `false` случае, если домен является поддоменом или непроверенным. Не допускает значения NULL |
|isVerified|Boolean| `true` Значение , если домен завершил проверку владения доменом. Не допускает значения NULL |
|passwordNotificationWindowInDays|Int32|Указывает количество дней до получения пользователем уведомления о том, что срок действия пароля истекает. Если свойство не задано, будет использоваться значение по умолчанию 14 дней.|
|passwordValidityPeriodInDays|Int32| Указывает срок действия пароля перед его изменением. Если свойство не задано, будет использоваться значение по умолчанию 90 дней. |
|supportedServices|Коллекция строк| Возможности, назначенные домену. Может включать `0`или `1` более следующих значений: `Email`, `Sharepoint`, , `EmailInternalRelayOnly`, `OfficeCommunicationsOnline`,`SharePointDefaultDomain`, `FullRedelegation`, `SharePointPublic`, `OrgIdAuthentication`, `Yammer``Intune`. Значения, которые можно добавить или удалить с помощью API Graph: `Email`, `OfficeCommunicationsOnline`, `Yammer`. Значение null не допускается.|
|state|[domainState](domainstate.md)| Состояние асинхронных операций, запланированных для домена. |

## <a name="relationships"></a>Связи

Связи между доменом и другими объектами в каталоге, такими как записи проверки и записи конфигурации службы, предоставляются через свойства навигации. Эти связи можно прочитать, нацелив эти свойства навигации в запросах.

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|domainNameReferences|Коллекция [directoryObject](directoryobject.md)| Объекты, такие как пользователи и группы, которые ссылаются на идентификатор домена. Только для чтения, допускает значение NULL. Поддерживает и `$expand` тип `$filter` возвращаемых объектов OData. Например, `/domains/{domainId}/domainNameReferences/microsoft.graph.user` и `/domains/{domainId}/domainNameReferences/microsoft.graph.group`.|
|serviceConfigurationRecords|[Коллекция domainDnsRecord](domaindnsrecord.md)| Записи DNS, которые клиент добавляет в файл зоны DNS домена перед использованием домена службами Microsoft Online. Только для чтения, допускает значение NULL. Поддерживает `$expand`. |
|verificationDnsRecords|[Коллекция domainDnsRecord](domaindnsrecord.md)| Записи DNS, которые клиент добавляет в файл зоны DNS домена, прежде чем клиент сможет завершить проверку владения доменом с помощью Azure AD. Только для чтения, допускает значение NULL. Поддерживает `$expand`.|
|federationConfiguration|[internalDomainFederation](../resources/internaldomainfederation.md)| Параметры домена, настроенные клиентом при федерации с Azure AD. Поддерживает `$expand`.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


