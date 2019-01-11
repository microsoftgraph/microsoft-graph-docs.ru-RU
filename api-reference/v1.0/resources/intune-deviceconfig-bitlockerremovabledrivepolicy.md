---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fc9fe3350fd9f4b5c5808de2c35fa3451943e449
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830837"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a>Тип ресурса bitLockerRemovableDrivePolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика BitLocker в отношении съемных дисков.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для съемных дисков. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Boolean|Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.  Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.|
|blockCrossOrganizationWriteAccess|Boolean|Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.|

## <a name="relationships"></a>Связи
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



