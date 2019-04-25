---
title: Тип ресурса depOnboardingSetting
description: DepOnboardingSetting представляет экземпляр службы Apple DEP, входящей в Intune. Встроенный экземпляр службы управляет маркером Apple, используемым для синхронизации данных между Apple и Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56f25c3e187671e0ba91f2d9124bf5f2d801e663
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573930"
---
# <a name="deponboardingsetting-resource-type"></a>Тип ресурса depOnboardingSetting

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

DepOnboardingSetting представляет экземпляр службы Apple DEP, входящей в Intune. Встроенный экземпляр службы управляет маркером Apple, используемым для синхронизации данных между Apple и Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|Коллекция [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Список свойств и связей объектов [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Получение depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Чтение свойств и связей объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Создание depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Удаление depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|Нет|Удаляет объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[Обновление depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Обновление свойств объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Функция getEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|Получение открытого ключа, используемого для шифрования маркера программы регистрации устройств Apple|
|[Действие uploadDepToken](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Нет|Отправка нового маркера программы регистрации устройств|
|[Действие syncWithAppleDeviceEnrollmentProgram](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Нет|Синхронизация между программой регистрации устройств Apple и Intune|
|[Действие shareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Нет|Н/Д|
|[Действие unshareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|appleIdentifier|String|Идентификатор Apple ID, используемый для получения текущего маркера.|
|tokenExpirationDateTime|DateTimeOffset|По истечении срока действия маркера.|
|lastModifiedDateTime|DateTimeOffset|При подключении службы.|
|Ластсукцессфулсинкдатетиме|DateTimeOffset|Когда служба последний синед с Intune|
|Ластсинктригжереддатетиме|DateTimeOffset|При последнем запросе синхронизации в Intune.|
|Свойства sharetokenwithschooldatasyncservice|Boolean|Указывает, включен ли общий доступ к маркеру DEP для службы School Data Sync.|
|Lastsyncerrorcode к объекту|Int32|Код ошибки, полученный от Apple во время последней синхронизации DEP.|
|Токентипе|[depTokenType](../resources/intune-enrollment-deptokentype.md);|Получает или задает тип токена DEP. Возможные значения: `none`, `dep`, `appleSchoolManager`.|
|Токеннаме|String|Понятное имя для токена DEP|
|Синцеддевицекаунт|Int32|Получает число синхронизированных устройств|
|dataSharingConsentGranted|Boolean|Разрешение, предоставленное для предоставления общего доступа к данным с помощью службы Apple DEP|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Дефаултиосенроллментпрофиле|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Профиль регистрации iOS по умолчанию|
|Дефаултмакосенроллментпрофиле|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Профиль регистрации MacOs по умолчанию|
|enrollmentProfiles|Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|Коллекция [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортированные удостоверения устройств Apple.|

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```





