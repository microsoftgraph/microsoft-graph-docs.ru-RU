---
title: Тип ресурса androidManagedStoreAccountEnterpriseSettings
description: Корпоративные параметры для Android управляемой учетной записи хранилища.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a14f0327c4a4c4cf2bc78e56b63686208e97d4b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933816"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>Тип ресурса androidManagedStoreAccountEnterpriseSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Корпоративные параметры для Android управляемой учетной записи хранилища.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Чтение свойства и связи объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Обновление androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md);|Обновление свойства объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Действие requestSignupUrl](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|Н/Д|
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Нет|Н/Д|
|[Действие syncApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Нет|Н/Д|
|[Действие unbind](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Нет|Н/Д|
|[Действие createGooglePlayWebToken](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|Создает веб-маркера, который используется в встраиваемые компонента.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Android хранения идентификатора параметров учетной записи предприятия|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Привязка состояния клиента с помощью API EMM Google. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Результат последней синхронизации приложения. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Название организации, используемые при адаптация новых сотрудников предприятия Android|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения для Android Корпоративные параметры|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Указывает пользователей, которые можно зарегистрировать устройств в управление устройствами Android предприятия. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|
|deviceOwnerManagementEnabled|Boolean|Указывает, если эта учетная запись flighting для Android владелец управление устройствами с CloudDPC.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```





