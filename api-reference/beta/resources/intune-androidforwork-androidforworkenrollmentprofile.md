---
title: Тип ресурса androidForWorkEnrollmentProfile
description: Профиль регистрации, используемый для регистрации устройств COSU с помощью управления облачными клиентами от Google.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84436012a9c536e1917b6170df3ecd04cd5e0b72
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792626"
---
# <a name="androidforworkenrollmentprofile-resource-type"></a>Тип ресурса androidForWorkEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль регистрации, используемый для регистрации устройств COSU с помощью управления облачными клиентами от Google.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidForWorkEnrollmentProfiles](../api/intune-androidforwork-androidforworkenrollmentprofile-list.md)|Коллекция [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Список свойств и связей объектов [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Получение объекта androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Чтение свойств и связей объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Создание объекта androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-create.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Создание объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Удаление объекта androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-delete.md)|Нет|Удаление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Обновление объекта androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[revokeToken action](../api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken.md)|Нет|Н/Д|
|[Действие createToken](../api/intune-androidforwork-androidforworkenrollmentprofile-createtoken.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accountId|String|GUID клиента, которому принадлежит профиль регистрации.|
|id|Строка|Уникальный GUID профиля регистрации.|
|displayName|Строка|Отображаемое имя для профиля регистрации.|
|description|Строка|Описание профиля регистрации.|
|createdDateTime|DateTimeOffset|Дата и время создания профиля регистрации.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения профиля регистрации.|
|tokenValue|String|Значение последнего созданного маркера для этого профиля регистрации.|
|tokenExpirationDateTime|DateTimeOffset|Дата и время, когда истекает срок действия последнего созданного маркера.|
|enrolledDeviceCount|Int32|Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.|
|qrCodeContent|String|Строка, используемая для создания QR-кода маркера.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Строка, используемая для создания QR-кода маркера.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



