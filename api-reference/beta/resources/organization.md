---
title: Тип ресурса organization
description: 'Представляет клиента Azure Active Directory. '
ms.openlocfilehash: 053656eb042ca04f2d487d47ee62624875fa4e17
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191146"
---
# <a name="organization-resource-type"></a>Тип ресурса organization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет клиента Azure Active Directory. 

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

Поддерживается только операций чтения и обновления клиентов; Создание и удаление не поддерживаются. Наследуется от [directoryObject](directoryobject.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Get organization](../api/organization-get.md) | [organization](organization.md) |Считывание свойств и связей объекта организации.|
|[Update](../api/organization-update.md) | [organization](organization.md)  |Обновление объекта организации. Обновлять можно только эти свойства: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** и **privacyProfile**. |
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignedPlans|Коллекция [assignedPlan](assignedplan.md)|Коллекция планов обслуживания, сопоставленных с клиентом. Значение NULL не допускается.            |
|city|String| Название города в адресе организации |
|companyLastDirSyncTime|DateTimeOffset|Дата и время последней синхронизации клиента с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|country|String| Название страны или региона в адресе организации. |
|countryLetterCode|String| Сокращенное название страны или региона для организации. |
|createdDateTime|DateTimeOffset| Метка времени создания организации. Значение не могут быть изменены и заполняется автоматически при создании организации. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|deletionTimestamp|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|dirSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).|
|displayName|String|Отображаемое имя для клиента.|
|id|String|Уникальный идентификатор клиента. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения.|
|isMultipleDataLocationsForServicesEnabled|Boolean|**значение true,** Если организация — ферма с несколькими-географически включено; **значение false,** Если организация не включена несколькими географически; **значение NULL** (по умолчанию). Только для чтения. Для получения дополнительных сведений см [OneDrive Online Multi-географически](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|marketingNotificationEmails|Коллекция String| Значение null не допускается.            |
|objectType|String|Строка, которая определяет тип объекта. Для клиентов всегда задается значение Company. |
|postalCode|String| Почтовый индекс в адресе организации |
|preferredLanguage|String| Предпочитаемый язык для организации. Он должен быть представлен в формате ISO 639-1. Пример: ru. |
|privacyProfile|[privacyProfile](privacyprofile.md)| Профиль конфиденциальности организации.            |
|provisionedPlans|Коллекция [ProvisionedPlan](provisionedplan.md)| Значение null не допускается.            |
|provisioningErrors|Коллекция ProvisioningError| Значение null не допускается.            |
|securityComplianceNotificationMails|Коллекция String||
|securityComplianceNotificationPhones|Коллекция String||
|state|String| Название республики, области или края в адресе организации |
|street|String| Название улицы в адресе организации |
|technicalNotificationMails|Коллекция String| Значение null не допускается. |
|telephoneNumber|String| Номер телефона организации |
|verifiedDomains|Коллекция [VerifiedDomain](verifieddomain.md)|Коллекция доменов, сопоставленных с этим клиентом. Значение null не допускается.            |

## <a name="relationships"></a>Связи
| расширения | набор [расширений](extension.md) | Коллекция open расширения, определенных для ресурсов организации. Допускает значение NULL. |

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
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
