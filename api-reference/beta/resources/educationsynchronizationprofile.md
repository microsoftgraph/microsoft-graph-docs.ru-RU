---
title: Тип ресурса Едукатионсинчронизатионпрофиле
description: Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в School Data Sync.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e1b81ff14aca2b0f81a7f50e01aed6281d03d14d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542883"
---
# <a name="educationsynchronizationprofile-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофиле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор конфигураций, используемых для синхронизации сущностей образования и сведений о подкаталогах из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс предоставляет программное представление, используемое в [School Data Sync](https://sds.microsoft.com).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Профили синхронизации списка](../api/educationsynchronizationprofile-list.md) | Коллекция **едукатионсинчронизатионпрофиле** | Получение списка всех профилей синхронизации в клиенте. |
| [Получение профиля синхронизации](../api/educationsynchronizationprofile-get.md) | **Едукатионсинчронизатионпрофиле** | Получение определенного профиля с учетом заданного идентификатора профиля. |
| [Создание профиля синхронизации](../api/educationsynchronizationprofile-post.md) | Нет | Создание нового профиля синхронизации. |
| [Удаление профиля синхронизации](../api/educationsynchronizationprofile-delete.md) | **Едукатионсинчронизатионпрофиле** | Удаление определенного профиля с учетом идентификатора профиля. |
| [ПриОстановка текущей синхронизации](../api/educationsynchronizationprofile-pause.md) | Нет | ПриОстановите текущую синхронизацию. |
| [ВозОбновление приостановленной синхронизации](../api/educationsynchronizationprofile-resume.md) | Нет | ВозОбновление приостановленной синхронизации. |
| [Сброс синхронизации](../api/educationsynchronizationprofile-reset.md) | Нет | Сбросьте состояние профиля и перезапустите синхронизацию. |
| [Запуск синхронизации для отправленных файлов](../api/educationsynchronizationprofile-start.md) | Коллекция [едукатионфилесинчронизатионверификатионмессаже](educationfilesynchronizationverificationmessage.md)| Проверьте отправленные исходные файлы и запустите синхронизацию. Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер](educationcsvdataprovider.md). |
| [Получение URL-адреса отправки](../api/educationsynchronizationprofile-uploadurl.md) | string | Возвращает кратковременный URL-адрес для отправки CSV-файлов данных. Применяется только в том случае, если поставщик данных — [едукатионксвдатапровидер](educationcsvdataprovider.md). |
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | Возврат состояния определенного профиля синхронизации. |
| [Получение ошибок синхронизации](../api/educationsynchronizationerrors-get.md) | Коллекция [educationSynchronizationError](educationsynchronizationerror.md)| Получение всех ошибок, возникших во время синхронизации. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **displayName** | string |  Имя профиля конфигурации для удостоверений синхронизации.         |
| **Предоставление dataProvider** | [Едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md) |  Поставщик данных, используемый для профиля.         |
| **Идентитисинчронизатионконфигуратион** | [Едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md) | [Создание](educationidentitycreationconfiguration.md) удостоверения или [соответствующая](educationidentitymatchingconfiguration.md) конфигурация.        |
| **Лиценсестоассигн** | Коллекция [едукатионсинчронизатионлиценсеассигнмент](educationsynchronizationlicenseassignment.md)|  Конфигурация установки лицензий.        |
| **state** | Едукатионсинчронизатионпрофилестате |  Состояние профиля. Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.          |

## <a name="relationships"></a>Связи

| Свойство | Тип | Описание |
|:-|:-|:-|
| **errors** | Коллекция [educationSynchronizationError](educationsynchronizationerror.md)| Все ошибки, связанные с этим профилем синхронизации. |
| **Профилестатус** | [Едукатионсинчронизатионпрофилестатус](educationsynchronizationprofilestatus.md) | Состояние синхронизации. |

## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено представление ресурса **едукатионсинчронизатионпрофиле** в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
