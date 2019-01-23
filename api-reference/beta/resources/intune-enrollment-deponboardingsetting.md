---
title: Тип ресурса depOnboardingSetting
description: DepOnboardingSetting представляет экземпляр службы Apple DEP, onboarded для Intune. Экземпляр службы onboarded управляет Apple маркеров используется для синхронизации данных между Apple и Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c0e5bcbdf0a687d4601aa92c8fe0eacdd675cd2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423771"
---
# <a name="deponboardingsetting-resource-type"></a>Тип ресурса depOnboardingSetting

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|dataSharingConsentGranted|Логический|Предоставляются разрешения для данных, общий доступ к службе Dep Apple|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
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
  "dataSharingConsentGranted": true
}
```




