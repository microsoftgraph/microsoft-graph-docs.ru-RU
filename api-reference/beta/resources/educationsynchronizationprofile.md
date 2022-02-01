---
title: тип ресурса educationSynchronizationProfile
description: Представляет набор конфигураций, используемых для синхронизации сущностями образования и сведениями реестра из источника каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемого в Синхронизация сведений о школе.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 09ae4b8fc02c1a1f13a91102241b119727e8bed2
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62289932"
---
# <a name="educationsynchronizationprofile-resource-type"></a>тип ресурса educationSynchronizationProfile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций, используемых для синхронизации сущностями образования и сведениями реестра из источника каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемого в [Синхронизация сведений о школе](https://sds.microsoft.com).

## <a name="methods"></a>Методы

| Метод                                                                    | Возвращаемый тип                                                 | Описание                                                                                                                    |
| :------------------------------------------------------------------------ | :---------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------- |
| [Профили списков](../api/educationsynchronizationprofile-list.md)           | [коллекция educationSynchronizationProfile]                | Получите список всех профилей синхронизации в клиенте.                                                                  |
| [Получение профиля](../api/educationsynchronizationprofile-get.md)              | [educationSynchronizationProfile]                           | Извлечение определенного профиля с учетом идентификатора профиля.                                                                      |
| [Создание профиля](../api/educationsynchronizationprofile-post.md)          | Нет                                                        | Создайте новый профиль синхронизации.                                                                                          |
| [Удаление профиля](../api/educationsynchronizationprofile-delete.md)        | [educationSynchronizationProfile]                           | Удалите определенный профиль с учетом идентификатора профиля.                                                                        |
| [Профиль паузы](../api/educationsynchronizationprofile-pause.md)          | Нет                                                        | Приостановка текущей синхронизации.                                                                                              |
| [Профиль резюме](../api/educationsynchronizationprofile-resume.md)        | Нет                                                        | Возобновление приостановки синхронизации.                                                                                               |
| [Сброс профиля](../api/educationsynchronizationprofile-reset.md)          | Нет                                                        | Сброс состояния профиля и синхронизация перезапуска.                                                                    |
| [Запуск профиля CSV](../api/educationsynchronizationprofile-start.md)      | [educationFileSynchronizationVerificationMessagecollection] | Проверьте загруженные исходные файлы и запустите синхронизацию. Применяется только в том случае, если поставщиком данных является [educationCsvDataProvider]. |
| [Получить URL-адрес загрузки CSV](../api/educationsynchronizationprofile-uploadurl.md) | string                                                      | Верни короткий URL-адрес для отправки файлов данных CSV. Применяется только в том случае, если поставщиком данных является [educationCsvDataProvider].        |
| [Получить состояние](../api/educationsynchronizationprofilestatus-get.md)         | [educationsynchronizationProfileStatus]                     | Возвращаем состояние определенного профиля синхронизации.                                                                       |
| [Получить ошибки](../api/educationsynchronizationerrors-get.md)                | [коллекция educationSynchronizationError]                  | Получите все ошибки, созданные во время синхронизации.                                                                           |

## <a name="properties"></a>Свойства

| Свойство                             | Тип                                                   | Описание                                                                                                                       |
| :----------------------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| id                                   | String                                                 | Уникальный идентификатор ресурса. (только для чтения)                                                                               |
| displayName                          | String                                                 | Имя профиля конфигурации для синхронизации удостоверений.                                                                         |
| dataProvider                         | [educationSynchronizationDataProvider]                 | Поставщик данных, используемый для профиля.                                                                                           |
| expirationDate                       | Date                                                   | Дата, когда профиль должен считаться истекшим, и прекратить синхронизацию. Когда `null`. срок действия профиля никогда не истекает. (необязательный)       |
| handleSpecialCharacterConstraint     | Логический                                                   | Определяет, следует ли Синхронизация сведений о школе автоматически заменить неподтверченные специальные символы при синхронизации из источника.             |
| identitySynchronizationConfiguration | [educationIdentitySynchronizationConfiguration]        | Определяет, как профиль должен [создавать новые или][fullsync] [соответствовать существующим AAD][dirsync] пользователям.                                  |
| licensesToAssign                     | [коллекция educationSynchronizationLicenseAssignment] | Конфигурация настройки лицензии.                                                                                                      |
| state                                | educationSynchronizationProfileState                   | Состояние профиля. Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`. |

## <a name="relationships"></a>Связи

| Связь  | Тип                                       | Описание                                              |
| :------------ | :----------------------------------------- | :------------------------------------------------------- |
| ошибки        | [коллекция educationSynchronizationError] | Все ошибки, связанные с этим профилем синхронизации. |
| profileStatus | [educationSynchronizationProfileStatus]    | Состояние синхронизации.                              |

## <a name="data-providers"></a>Data Providers

[Каждый поставщик данных educationSynchronizationProfile] должен указать один из последующих поставщиков данных, который будет использовать в качестве источника синхронизации.

| Поставщик данных                                                             | Описание                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | CSV-файлы, загруженные на [URL-адрес SAS профиля](../api/educationsynchronizationprofile-uploadurl.md) |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | API PowerSchool                                                                                    |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса **educationSynchronizationProfile** .

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
  "handleSpecialCharacterConstraint": "Boolean",
  "expirationDate": "Date"
}
```

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationsynchronizationprofilestatus]: educationsynchronizationProfileStatus.md
[educationsynchronizationerror]: educationSynchronizationError.md
[educationfilesynchronizationverificationmessage]: educationFileSynchronizationVerificationMessage.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationidentitysynchronizationconfiguration]: educationIdentitySynchronizationConfiguration.md
[educationsynchronizationlicenseassignment]: educationSynchronizationLicenseAssignment.md
[fullsync]: educationidentitycreationconfiguration.md
[dirsync]: educationidentitycreationconfiguration.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSynchronizationProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
}-->


