---
title: Тип ресурса Едукатионсинчронизатионпрофиле
description: Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 05babeebb25130350e64d98ccfc408381547829e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790917"
---
# <a name="educationsynchronizationprofile-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофиле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в [School Data Sync](https://sds.microsoft.com).

## <a name="methods"></a>Методы

| Метод                                                                    | Возвращаемый тип                                                 | Описание                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [Список профилей](../api/educationsynchronizationprofile-list.md)           | Коллекция [едукатионсинчронизатионпрофиле]                | Получение списка всех профилей синхронизации в клиенте.                                                                  |
| [Получение профиля](../api/educationsynchronizationprofile-get.md)              | [едукатионсинчронизатионпрофиле]                           | Получение определенного профиля с учетом заданного идентификатора профиля.                                                                      |
| [Создание профиля](../api/educationsynchronizationprofile-post.md)          | Нет                                                        | Создание нового профиля синхронизации.                                                                                          |
| [Удаление профиля](../api/educationsynchronizationprofile-delete.md)        | [едукатионсинчронизатионпрофиле]                           | Удаление определенного профиля с учетом идентификатора профиля.                                                                        |
| [Приостановить профиль](../api/educationsynchronizationprofile-pause.md)          | Нет                                                        | Приостановите текущую синхронизацию.                                                                                              |
| [Профиль возобновления](../api/educationsynchronizationprofile-resume.md)        | Нет                                                        | Возобновление приостановленной синхронизации.                                                                                               |
| [Сброс профиля](../api/educationsynchronizationprofile-reset.md)          | Нет                                                        | Сбросьте состояние профиля и перезапустите синхронизацию.                                                                    |
| [Начальный CSV-профиль](../api/educationsynchronizationprofile-start.md)      | Коллекция [едукатионфилесинчронизатионверификатионмессаже] | Проверьте отправленные исходные файлы и запустите синхронизацию. Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер]. |
| [Получение URL-адреса отправки CSV-файла](../api/educationsynchronizationprofile-uploadurl.md) | string                                                      | Возвращает кратковременный URL-адрес для отправки CSV-файлов данных. Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер].        |
| [Получение состояния](../api/educationsynchronizationprofilestatus-get.md)         | [едукатионсинчронизатионпрофилестатус]                     | Возврат состояния определенного профиля синхронизации.                                                                       |
| [Получение ошибок](../api/educationsynchronizationerrors-get.md)                | Коллекция [educationSynchronizationError]                  | Получение всех ошибок, возникших во время синхронизации.                                                                           |

## <a name="properties"></a>Свойства

| Свойство                             | Тип                                                   | Описание                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| displayName                          | string                                                 | Имя профиля конфигурации для удостоверений синхронизации.                                                                         |
| Предоставление dataProvider                         | [едукатионсинчронизатиондатапровидер]                 | Поставщик данных, используемый для профиля.                                                                                           |
| идентитисинчронизатионконфигуратион | [едукатионидентитисинчронизатионконфигуратион]        | Определяет, как профиль должен [создавать новые][fullsync] или [сопоставляться с имеющимися][dirsync] пользователями AAD.                                  |
| лиценсестоассигн                     | Коллекция [едукатионсинчронизатионлиценсеассигнмент] | Конфигурация установки лицензий.                                                                                                      |
| state                                | едукатионсинчронизатионпрофилестате                   | Состояние профиля. Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`. |

## <a name="relationships"></a>Связи

| Связь  | Тип                                       | Описание                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| ошибки        | Коллекция [educationSynchronizationError] | Все ошибки, связанные с этим профилем синхронизации. |
| профилестатус | [едукатионсинчронизатионпрофилестатус]    | Состояние синхронизации.                              |

## <a name="data-providers"></a>Data Providers

Каждый [едукатионсинчронизатионпрофиле] должен указать одного из указанных ниже поставщиков данных, который будет использоваться в качестве источника синхронизации.

| Поставщик данных                       | Описание                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| [едукатионксвдатапровидер]          | CSV-файлы, отправленные на [URL-адрес профиля SAS](../api/educationsynchronizationprofile-uploadurl.md) |
| [едукатиононеростерапидатапровидер](educationonerosterapidataprovider.md) | API OneRoster 1.1                                                                                 |
| [едукатионповерсчулдатапровидер]  | API PowerSchool                                                                                    |

## <a name="json-representation"></a>Представление JSON

Ниже представлено представление ресурса **едукатионсинчронизатионпрофиле** в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "state": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileState"
  },
  "profileStatus": {
    "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
  },
  "errors": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
    }
  ],
  "dataProvider": {
    "@odata.type": "microsoft.graph.educationCsvDataProvider"
  },
  "identitySynchronizationConfiguration": {
    "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
  },
  "licensesToAssign": [
    {
      "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
    }
  ],
  "handleSpecialCharacterConstraint": "Boolean"
}
```

[едукатионсинчронизатионпрофиле]: educationsynchronizationprofile.md
[едукатионсинчронизатионпрофилестатус]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[едукатионфилесинчронизатионверификатионмессаже]: educationFileSynchronizationVerificationMessage.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md
[едукатионсинчронизатиондатапровидер]: educationSynchronizationDataProvider.md
[едукатионидентитисинчронизатионконфигуратион]: educationIdentitySynchronizationConfiguration.md
[едукатионсинчронизатионлиценсеассигнмент]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[едукатионповерсчулдатапровидер]: educationPowerSchoolDataProvider.md
[едукатионксвдатапровидер]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationSynchronizationProfile/dataProvider:\r\n      Referenced type microsoft.graph.educationSynchronizationDataProvider is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
