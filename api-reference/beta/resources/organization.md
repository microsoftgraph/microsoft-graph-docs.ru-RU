---
title: Тип ресурса organization
description: 'Представляет клиента Azure Active Directory. '
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ea21e90c720962c7fc047edd6f19630c3918b352
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721350"
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
|[Обновление организации](../api/organization-update.md) | [organization](organization.md)  |Обновление объекта организации. Обновлять можно только эти свойства: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** и **privacyProfile**. |
| [Получить параметры организации](../api/organizationsettings-get.md) | [organisationSettings](organizationsettings.md) | Ознакомьтесь с объектом параметры организации. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](../api/schemaextension-post-schemaextensions.md) | [schemaExtension](schemaextension.md) | Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|[Создание organizationalBrandingProperties](../api/organizationalbrandingproperties-create.md) | [organizationalBrandingProperties](organizationalbrandingproperties.md) | Создайте новую организациюBrandingProperties, разместив в коллекции брендинга. |
|[Получить брендинг](../api/organizationalbrandingproperties-get.md) | [коллекция organizationalBrandingProperties](organizationalbrandingproperties.md) | Получите коллекцию объектов organizationalBrandingProperties. |

## <a name="properties"></a>Свойства 
| Свойство | Тип   | Описание |
|:-------- |:---- |:----------- |
| assignedPlans | Коллекция [assignedPlan](assignedplan.md) | Коллекция планов обслуживания, сопоставленных с клиентом. Значение null не допускается. |
| businessPhones | Коллекция String | Номер телефона организации. **Примечание.** Несмотря на то что это коллекция строк, для этого свойства можно задать только один номер. |
| city | String | Название города в адресе организации. |
| country | String | Название страны или региона в адресе организации. |
| countryLetterCode | String | Сокращенное название страны или региона для организации. |
| createdDateTime | DateTimeOffset | Метка времени создания организации. Значение не может изменяться и заполняется автоматически, когда создается организация. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
| deletedDateTime | DateTimeOffset | Представляет дату и время удаления клиента Azure AD с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
| directorySizeQuota | [directorySizeQuota](directorySizeQuota.md) | Сведения о квоте размера каталога организации. |
| displayName | String | Отображаемое имя для клиента. |
| id | String | Уникальный идентификатор клиента, представляющий организацию (или клиента). Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
| isMultipleDataLocationsForServicesEnabled | Boolean | Используется значение **true**, если в организации включена поддержка нескольких регионов. Используется значение **false**, если поддержка нескольких регионов в организации не включена. По умолчанию используется значение **null**. Только для чтения. Дополнительные сведения см. в статье [OneDrive Online с поддержкой нескольких регионов](/sharepoint/dev/solution-guidance/multigeo-introduction). |
| marketingNotificationEmails | Коллекция String | Значение null не допускается. |
| objectType | String | Строка, которая определяет тип объекта. Для клиентов всегда задается значение Company. |
| onPremisesLastSyncDateTime | DateTimeOffset | Время и дата последней синхронизации клиента с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
| onPremisesSyncEnabled | Boolean | Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию). |
| postalCode | String | Почтовый индекс в адресе организации. |
| preferredLanguage | String | Предпочитаемый язык для организации. Он должен быть представлен в формате ISO 639-1. Пример: ru. |
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
|certificateBasedAuthConfiguration|Коллекция [certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md)| Свойство Navigation для управления конфигурацией проверки подлинности на основе сертификатов. В коллекции можно создать только один экземпляр объекта certificateBasedAuthConfiguration.  |
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для ресурса организации. Допускается значение null.| 
|organizationalBranding|[коллекция organizationalBrandingProperties](organizationalbrandingproperties.md)| Брендинг для организации. Допускается значение null.|
|параметры|[organisationSettings](organizationsettings.md) | Извлечение свойств и связей объекта organizationSettings. Допускается значение null.|

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
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "objectType": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
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
