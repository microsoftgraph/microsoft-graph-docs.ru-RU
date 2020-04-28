---
title: Тип ресурса Едукатионсинчронизатионпрофиле
description: Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7cea993bfaeaf7de82268747518288aaac836198
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500088"
---
# <a name="educationsynchronizationprofile-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофиле

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в [School Data Sync](https://sds.microsoft.com).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Профили синхронизации списка](../api/educationsynchronizationprofile-list.md) | Коллекция **едукатионсинчронизатионпрофиле** | Получение списка всех профилей синхронизации в клиенте. |
| [Получение профиля синхронизации](../api/educationsynchronizationprofile-get.md) | **едукатионсинчронизатионпрофиле** | Получение определенного профиля с учетом заданного идентификатора профиля. |
| [Создание профиля синхронизации](../api/educationsynchronizationprofile-post.md) | Нет | Создание нового профиля синхронизации. |
| [Удаление профиля синхронизации](../api/educationsynchronizationprofile-delete.md) | **едукатионсинчронизатионпрофиле** | Удаление определенного профиля с учетом идентификатора профиля. |
| [Приостановка текущей синхронизации](../api/educationsynchronizationprofile-pause.md) | Нет | Приостановите текущую синхронизацию. |
| [Возобновление приостановленной синхронизации](../api/educationsynchronizationprofile-resume.md) | Нет | Возобновление приостановленной синхронизации. |
| [Сброс синхронизации](../api/educationsynchronizationprofile-reset.md) | Нет | Сбросьте состояние профиля и перезапустите синхронизацию. |
| [Запуск синхронизации для отправленных файлов](../api/educationsynchronizationprofile-start.md) | Коллекция [едукатионфилесинчронизатионверификатионмессаже](educationfilesynchronizationverificationmessage.md)| Проверьте отправленные исходные файлы и запустите синхронизацию. Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер](educationcsvdataprovider.md). |
| [Получение URL-адреса отправки](../api/educationsynchronizationprofile-uploadurl.md) | string | Возвращает кратковременный URL-адрес для отправки CSV-файлов данных. Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер](educationcsvdataprovider.md). |
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | Возврат состояния определенного профиля синхронизации. |
| [Получение ошибок синхронизации](../api/educationsynchronizationerrors-get.md) | Коллекция [educationSynchronizationError](educationsynchronizationerror.md)| Получение всех ошибок, возникших во время синхронизации. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **displayName** | string |  Имя профиля конфигурации для удостоверений синхронизации.         |
| **Предоставление dataProvider** | [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md) |  Поставщик данных, используемый для профиля.         |
| **идентитисинчронизатионконфигуратион** | [едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md) | [Создание](educationidentitycreationconfiguration.md) удостоверения или [соответствующая](educationidentitymatchingconfiguration.md) конфигурация.        |
| **лиценсестоассигн** | Коллекция [едукатионсинчронизатионлиценсеассигнмент](educationsynchronizationlicenseassignment.md)|  Конфигурация установки лицензий.        |
| **state** | едукатионсинчронизатионпрофилестате |  Состояние профиля. Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.          |

## <a name="relationships"></a>Связи

| Свойство | Тип | Описание |
|:-|:-|:-|
| **errors** | Коллекция [educationSynchronizationError](educationsynchronizationerror.md)| Все ошибки, связанные с этим профилем синхронизации. |
| **профилестатус** | [едукатионсинчронизатионпрофилестатус](educationsynchronizationprofilestatus.md) | Состояние синхронизации. |

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
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "microsoft.graph.educationCsvDataProvider" },
    "identitySynchronizationConfiguration": { "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
