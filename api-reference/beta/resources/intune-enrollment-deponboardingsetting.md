---
title: Тип ресурса depOnboardingSetting
description: DepOnboardingSetting представляет экземпляр службы Apple DEP, onboarded для Intune. Экземпляр службы onboarded управляет Apple маркеров используется для синхронизации данных между Apple и Intune.
ms.openlocfilehash: 7991b03b8307db10d3a300b1b85be3fc1b825819
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082240"
---
# <a name="deponboardingsetting-resource-type"></a>Тип ресурса depOnboardingSetting

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

DepOnboardingSetting представляет экземпляр службы Apple DEP, onboarded для Intune. Экземпляр службы onboarded управляет Apple маркеров используется для синхронизации данных между Apple и Intune.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) коллекции|Свойства списка и связей объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Получение depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Чтение свойства и связи объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Создание depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Удаление depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|Нет|Удаляет [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[Обновление depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Обновление свойства объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[функция getEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|Получение маркера открытого ключа, используемого для шифрования программы регистрации устройства Apple|
|[Действие uploadDepToken](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Нет|Загружает новый маркер программы регистрации устройства|
|[Действие syncWithAppleDeviceEnrollmentProgram](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Нет|Выполняет синхронизацию между программой регистрации устройства Apple и Intune|
|[Действие shareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Нет|Н/Д|
|[Действие unshareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|appleIdentifier|String|Apple идентификатор, используемый для получения текущего маркера.|
|tokenExpirationDateTime|DateTimeOffset|Маркер истечения срока действия.|
|lastModifiedDateTime|DateTimeOffset|Когда служба была onboarded.|
|lastSuccessfulSyncDateTime|DateTimeOffset|При последней syned службы с помощью Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Когда Intune запрашивает последней синхронизации.|
|shareTokenWithSchoolDataSyncService|Логический|Ли Dep маркеров общий доступ к включается со службой синхронизации данных School.|
|lastSyncErrorCode|Int32|Код ошибки Apple во время последней синхронизации dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md);|Получает или задает тип токена Dep. Возможные значения: `none`, `dep`, `appleSchoolManager`.|
|tokenName|String|Понятное имя для маркера Dep|
|syncedDeviceCount|Int32|Получает количество синхронизированных устройства|
|defaultProfileDisplayName|String|Получает количество синхронизированных устройства|
|dataSharingConsentGranted|Логический|Предоставляются разрешения для данных, общий доступ к службе Dep Apple|

## <a name="relationships"></a>Связи
|Связь|Тип|Description|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Операций ввода-вывода по умолчанию профиля подачи заявок|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Профиль по умолчанию MacOs подачи заявок|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) коллекции|Профили заявок через Интернет.|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) коллекции|Импортированные удостоверений устройства Apple.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1024,
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": 1024,
  "defaultProfileDisplayName": "String",
  "dataSharingConsentGranted": true
}
```





