---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9af6be0fc03dbd8ffffcdc85e5ec60296ca1ba24
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469667"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a>Тип ресурса bitLockerRemovableDrivePolicy

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика BitLocker в отношении съемных дисков.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[битлоккеренкриптионмесод](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для съемных дисков. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Boolean|Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.  Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.|
|blockCrossOrganizationWriteAccess|Boolean|Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



