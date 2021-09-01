---
title: тип ресурса depOnboardingSetting
description: DepOnboardingSetting представляет экземпляр службы DeP Apple, которая находится на борту в Intune. Экземпляр бортовой службы управляет маркером Apple, используемым для синхронизации данных между Apple и Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff9302af392e260dce9e24a54aba386687928d31
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801082"
---
# <a name="deponboardingsetting-resource-type"></a>тип ресурса depOnboardingSetting

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

DepOnboardingSetting представляет экземпляр службы DeP Apple, которая находится на борту в Intune. Экземпляр бортовой службы управляет маркером Apple, используемым для синхронизации данных между Apple и Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[коллекция depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Список свойств и связей объектов [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[Получить depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Чтение свойств и связей [объекта depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[Создание depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Создайте [новый объект depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[Удаление depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|Нет|Удаляет [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[Обновление depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Обновление свойств объекта [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[функция getEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|Строка|Получите общедоступный ключ для шифрования маркера программы регистрации устройств Apple|
|[generateEncryptionPublicKey action](../api/intune-enrollment-deponboardingsetting-generateencryptionpublickey.md)|Строка|Создание общедоступных ключей для шифрования маркера программы регистрации устройств Apple|
|[Действие uploadDepToken](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Нет|Загрузка нового маркера программы регистрации устройств|
|[Действие syncWithAppleDeviceEnrollmentProgram](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Нет|Синхронизация между программой регистрации устройств Apple и Intune|
|[Действие shareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Нет|Н/Д|
|[Действие unshareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Нет|Н/Д|
|[функция getExpiringVppTokenCount](../api/intune-enrollment-deponboardingsetting-getexpiringvpptokencount.md)|Int32|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|appleIdentifier|String|ID Apple, используемый для получения текущего маркера.|
|tokenExpirationDateTime|DateTimeOffset|По истечении срока действия маркера.|
|lastModifiedDateTime|DateTimeOffset|Когда служба была на борту.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Когда служба последний раз синхронизирована с Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Когда Intune в последний раз запрашивала синхронизацию.|
|shareTokenWithSchoolDataSyncService|Логический|Включено ли совместное использование маркеров Dep с Синхронизация сведений о школе службой.|
|lastSyncErrorCode|Int32|Код ошибки, сообщаемой Apple во время последней синхронизации dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md);|Получает или задает тип маркера Dep. Возможные значения: `none`, `dep`, `appleSchoolManager`.|
|tokenName|Строка|Friendly Name for Dep Token|
|syncedDeviceCount|Int32|Получает синхронизированное количество устройств|
|dataSharingConsentGranted|Логический|Согласие, предоставленное для обмена данными с службой Apple Dep|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Профиль регистрации iOS по умолчанию|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Профиль регистрации MacOs по умолчанию|
|enrollmentProfiles|[коллекция enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Профили регистрации.|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity collection](../resources/intune-enrollment-importedappledeviceidentity.md)|Импортируемые удостоверения устройств Apple.|

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



