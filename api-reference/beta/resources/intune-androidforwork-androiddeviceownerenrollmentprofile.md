---
title: тип ресурса androidDeviceOwnerEnrollmentProfile
description: Профиль регистрации, используемый для регистрации Enterprise устройств с помощью облачного управления Google.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8be1f18327a7573022c02b31d1699848f71f111
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339670"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a>тип ресурса androidDeviceOwnerEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль регистрации, используемый для регистрации Enterprise устройств с помощью облачного управления Google.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidDeviceOwnerEnrollmentProfiles](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|[коллекция androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Список свойств и связей [объектов androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Get androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md);|Чтение свойств и связей [объекта androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Создание androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md);|Создайте новый [объект androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Удаление androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|Нет|Удаляет [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).|
|[Обновление androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md);|Обновление свойств объекта [androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[revokeToken action](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|Нет|Н/Д|
|[Действие createToken](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accountId|String|GUID клиента, которому принадлежит профиль регистрации.|
|id|String|Уникальный GUID профиля регистрации.|
|displayName|String|Отображаемое имя для профиля регистрации.|
|description|Строка|Описание профиля регистрации.|
|enrollmentMode|[androidDeviceOwnerEnrollmentMode](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|Режим регистрации устройств, которые используют этот профиль регистрации. Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`, `corporateOwnedAOSPUserlessDevice`, `corporateOwnedAOSPUserAssociatedDevice`.|
|enrollmentTokenType|[androidDeviceOwnerEnrollmentTokenType](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|Тип маркера регистрации для профиля регистрации. Возможные значения: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.|
|createdDateTime|DateTimeOffset|Дата и время создания профиля регистрации.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения профиля регистрации.|
|tokenValue|String|Значение последнего созданного маркера для этого профиля регистрации.|
|tokenCreationDateTime|DateTimeOffset|Дата создания последнего созданного маркера.|
|tokenExpirationDateTime|DateTimeOffset|Дата и время, когда истекает срок действия последнего созданного маркера.|
|enrolledDeviceCount|Int32|Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.|
|enrollmentTokenUsageCount|Int32|Общее число устройств AOSP, которые зарегистрировались с помощью текущего маркера.|
|qrCodeContent|String|Строка, используемая для создания QR-кода маркера.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Строка, используемая для создания QR-кода маркера.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|
|wifiSsid|String|Строка, содержаная ssid входа wi-fi|
|wifiPassword|String|Строка с паролем входа в Wi-Fi|
|wifiSecurityType|[aospWifiSecurityType](../resources/intune-androidforwork-aospwifisecuritytype.md)|Строка, содержаная тип безопасности Wi-Fi. Возможные значения: `none`, `wpa`, `wep`.|
|wifiHidden|Boolean|Boolean, который указывает, включены ли скрытые сети Wi-Fi|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "enrollmentMode": "String",
  "enrollmentTokenType": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "enrollmentTokenUsageCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "roleScopeTagIds": [
    "String"
  ],
  "wifiSsid": "String",
  "wifiPassword": "String",
  "wifiSecurityType": "String",
  "wifiHidden": true
}
```




