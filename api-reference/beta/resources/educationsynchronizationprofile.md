---
title: Тип ресурса educationSynchronizationProfile
description: Представляет набор, использовавшееся для синхронизации education объектов и данных участников из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс содержит программного представления, используемые в синхронизации данных School.
ms.openlocfilehash: 89b605a7044526975f8caa6d7a1b6a716f012921
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082125"
---
# <a name="educationsynchronizationprofile-resource-type"></a>Тип ресурса educationSynchronizationProfile

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет набор, использовавшееся для синхронизации education объектов и данных участников из исходного каталога в Azure Active Directory (Azure AD). Этот ресурс содержит программного представления, используемые в [Синхронизации данных School](https://sds.microsoft.com).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Список синхронизации профилей](../api/educationsynchronizationprofile-list.md) | **educationSynchronizationProfile** коллекции | Получение списка всех синхронизации профилей в клиента. |
| [Начало синхронизации профилей](../api/educationsynchronizationprofile-get.md) | **educationSynchronizationProfile** | Получение определенного профиля, заданного идентификатора профилей. |
| [Создание синхронизации профилей](../api/educationsynchronizationprofile-post.md) | Нет | Создание нового профиля синхронизации. |
| [Удаление синхронизации профилей](../api/educationsynchronizationprofile-delete.md) | **educationSynchronizationProfile** | Удалите конфигурацию заданного профиля идентификатора. |
| [Приостановка текущей синхронизации](../api/educationsynchronizationprofile-pause.md) | Нет | Приостановка текущей синхронизации. |
| [Возобновление приостановленной синхронизации](../api/educationsynchronizationprofile-resume.md) | Нет | Возобновление приостановленной синхронизации. |
| [Сброс синхронизации](../api/educationsynchronizationprofile-reset.md) | Нет | Сбросить состояние профиля и перезапустите синхронизации. |
| [Запуск синхронизации переданных файлов](../api/educationsynchronizationprofile-start.md) | [educationFileSynchronizationVerificationMessage](educationfilesynchronizationverificationmessage.md) коллекции| Проверка загруженному исходных файлов и запуск синхронизации. Применяется только в том случае, когда поставщик данных является [educationCsvDataProvider](educationcsvdataprovider.md). |
| [Получение URL-адрес отправки](../api/educationsynchronizationprofile-uploadurl.md) | string | Возвращает кратковременного URL-адрес для отправки данных CSV-файлов. Применяется только в том случае, когда поставщик данных является [educationCsvDataProvider](educationcsvdataprovider.md). |
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | [status](educationsynchronizationprofilestatus.md) | Возвращает состояние определенного синхронизации профилей. |
| [Получение ошибки синхронизации](../api/educationsynchronizationerrors-get.md) | [educationSynchronizationError](educationsynchronizationerror.md) коллекции| Получение всех ошибок, возникших в процессе синхронизации. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:-|:-|:-|
| **displayName** | строка |  Имя профиля конфигурации синхронизации удостоверения.         |
| **dataProvider** | [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md) |  Поставщик данных, используемый для профиля.         |
| **identitysynchronizationconfiguration** | [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md) | Конфигурация [создания](educationidentitycreationconfiguration.md) или [соответствия](educationidentitymatchingconfiguration.md) удостоверений.        |
| **licensesToAssign** | [educationSynchronizationLicenseAssignment](educationsynchronizationlicenseassignment.md) коллекции|  Настройка установки лицензии.        |
| **state** | строка |  Состояние профиля. Возможные значения: `provisioning`, `provisioned`, `provisioningFailed`, `deleting`, `deletionFailed`.          |

## <a name="relationships"></a>Связи

| Свойство | Тип | Description |
|:-|:-|:-|
| **errors** | [educationSynchronizationError](educationsynchronizationerror.md) коллекции| Все ошибки, связанные с этой синхронизации профилей. |
| **profileStatus** | [educationSynchronizationProfileStatus](educationsynchronizationprofilestatus.md) | Состояние синхронизации. |

## <a name="json-representation"></a>Представление JSON
Ниже представлена JSON **educationSynchronizationProfile** ресурсов.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile"
}-->

```json
{
    "displayName": "String",
    "state": { "@odata.type": "microsoft.graph.educationSynchronizationProfileState" },
    "profileStatus": {"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"},
    "errors": [{"@odata.type": "microsoft.graph.educationSynchronizationProfileStatus" }],
    "dataProvider": { "@odata.type": "#microsoft.graph.educationcsvdataprovider" },
    "identitySynchronizationConfiguration": { "@odata.type": "#microsoft.graph.educationIdentitySynchronizationConfiguration" },
    "licensesToAssign": [{"@odata.type":"microsoft.graph.educationSynchronizationLicenseAssignment"}],
    "handleSpecialCharacterConstraint": "Boolean"
}
```
