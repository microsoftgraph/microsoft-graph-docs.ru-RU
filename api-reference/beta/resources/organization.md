---
title: Тип ресурса organization
description: 'Представляет клиента Azure Active Directory клиента. '
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 916da77d59fb4aee607145ffdbcd8cc40b7669e6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691577"
---
# <a name="organization-resource-type"></a>Тип ресурса organization

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет клиента Azure Active Directory, в который выполнен вход пользователем или приложением. Для этого ресурса поддерживаются только операции чтения и обновления. Создание и удаление не поддерживаются. Наследуется от [directoryObject](directoryobject.md).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Get organization](../api/organization-get.md) | Коллекция объектов [organization](organization.md)|Считывание свойств и связей объекта организации.|
|[Обновление организации](../api/organization-update.md) | [organization](organization.md)  |Обновление объекта организации. Обновляются только следующие свойства: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** и **privacyProfile**. |
| [Получить параметры организации](../api/organizationsettings-get.md) | [organisationSettings](organizationsettings.md) | Ознакомьтесь с объектом параметры организации. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../api/schemaextension-post-schemaextensions.md) | [schemaExtension](schemaextension.md) | Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Лицензии организации**| | |
|[activateService](../api/organization-activateservice.md) | Нет |  Активация службы для организации. |
|**Фирменная символика организации**| | |
|[Получение organizationalBranding](../api/organizationalbranding-get.md) | [organizationalBranding](organizationalbranding.md) | Получение стандартного объекта фирменной символики организации. |
|[Обновление organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | Обновление стандартного объекта фирменной символики организации. |
|[Создание organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Создание новой фирменной символики локализации (для определенного языка) и стандартного объекта фирменной символики, если он не существует. |
|[Список organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | Коллекция [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Извлечение всех объектов фирменной символики локализации в клиенте. |
|[Получение organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Чтение свойств объекта фирменной символики локализации. |
|[Обновление organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Обновление объекта фирменной символики локализации. |
|[Удаление organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md) | [organizationalBrandingLocalization](organizationalbrandinglocalization.md) | Удаление объекта фирменной символики локализации. |
<!--|[Удаление organizationalBranding](../api/organizationalbranding-update.md) | [organizationalBranding](organizationalbranding.md) | Удаление стандартного объекта фирменной символики организации. |

**ПРИМЕЧАНИЕ. Для восстановления операции удаления organizationalBranding в таблицу после операции обновления organizationalBranding, если устранены все несоответствия.-->

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| assignedPlans | Коллекция [assignedPlan](assignedplan.md) | Коллекция планов обслуживания, сопоставленных с клиентом. Значение null не допускается. |
| businessPhones | Коллекция String | Номера телефонов пользователя. Несмотря на то что это коллекция строк, в качестве значения этого свойства можно указать только одно число. |
| city | String | Название города в адресе организации. |
| country | String | Название страны или региона в адресе организации. |
| countryLetterCode | String | Сокращение страны или региона для организации в формате ISO 3166-2. |
| createdDateTime | DateTimeOffset | Метка времени создания организации. Значение не может изменяться и заполняется автоматически, когда создается организация. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
| deletedDateTime | DateTimeOffset | Представляет дату и время удаления клиента Azure AD в формате ISO 8601 (время всегда указывается в формате UTC). Например, полночь 1 января 2014 г. в формате UTC представляется в виде `2014-01-01T00:00:00Z`. Только для чтения. |
| directorySizeQuota | [directorySizeQuota](directorySizeQuota.md) | Сведения о квоте размера каталога организации. |
| displayName | String | Отображаемое имя для клиента. |
| id | String | Уникальный идентификатор клиента, представляющий организацию (или клиента). Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
| isMultipleDataLocationsForServicesEnabled | Boolean | `true` если организация включена в Multi-Geo; `false` если организация не включена в Multi-Geo; `null` (по умолчанию). Только для чтения. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](/sharepoint/dev/solution-guidance/multigeo-introduction). |
| marketingNotificationEmails | Коллекция String | Значение null не допускается. |
| objectType | String | Строка, которая определяет тип объекта. Для клиентов значение всегда `Company` .|
| onPremisesLastSyncDateTime | DateTimeOffset | Время и дата последней синхронизации клиента с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| onPremisesSyncEnabled | Логический | `true` если этот объект синхронизирован из локального каталога; если этот объект был первоначально синхронизирован из локального каталога, но `false` больше не синхронизирован; Nullable. Используется значение `null`, если этот объект никогда не синхронизировался из локального каталога (по умолчанию). |
| postalCode | String | Почтовый индекс в адресе организации. |
| preferredLanguage | String | Предпочитаемый язык для организации. Он должен быть представлен в формате ISO 639-1, например `en`. |
| privacyProfile | [privacyProfile](privacyprofile.md) | Профиль конфиденциальности организации. |
| provisionedPlans | Коллекция [provisionedPlan](provisionedplan.md) | Значение null не допускается. |
| securityComplianceNotificationMails | Коллекция String ||
| securityComplianceNotificationPhones | Коллекция String ||
| state | String | Название республики, области или края в адресе организации. |
| street | String | Название улицы в адресе организации. |
| technicalNotificationMails |Коллекция String | Значение null не допускается. |
| verifiedDomains | [коллекция verifiedDomain](verifieddomain.md)|Коллекция доменов, сопоставленных с этим клиентом. Значение null не допускается. |

## <a name="relationships"></a>Отношения

| Связь  | Тип  |Описание|
|:---------------|:--------|:----------|
|certificateBasedAuthConfiguration|Коллекция [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md)| Свойство навигации для управления конфигурацией проверки подлинности на основе сертификатов. В коллекции можно создать только один экземпляр объекта certificateBasedAuthConfiguration.  |
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для ресурса организации. Допускается значение null.| 
|organizationalBranding|Коллекция [organizationalBranding](organizationalbranding.md)| Ресурс для управления брендингом по умолчанию для организации. Допускается значение null.|
|settings|[organisationSettings](organizationsettings.md) | Извлечение свойств и связей объекта organizationSettings. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["String"],
  "city": "String",
  "country": "String",
  "countryLetterCode": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
  "displayName": "String",
  "id": "String (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "Boolean",
  "marketingNotificationEmails": ["String"],
  "objectType": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "String",
  "preferredLanguage": "String",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["String"],
  "securityComplianceNotificationPhones": ["String"],
  "state": "String",
  "street": "String",
  "technicalNotificationMails": ["String"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
