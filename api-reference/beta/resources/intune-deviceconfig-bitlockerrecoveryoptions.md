---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c77cb413202ce713ce658da633f351f07286a03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527038"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Тип ресурса Битлоккеррековерйоптионс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры восстановления BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|блоккдатарековеряжент|Логический|Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.|
|рековерипассвордусаже|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр. Возможные значения: `blocked`, `required`, `allowed`.|
|рековерикэйусаже|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска. Возможные значения: `blocked`, `required`, `allowed`.|
|хидерековерйоптионс|Логический|Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.|
|енаблерековеринформатионсаветосторе|Логический|Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.|
|рековеринформатионтосторе|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части данных восстановления BitLocker хранятся в AD DS. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|енаблебитлоккерафтеррековеринформатионтосторе|Логический|Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```



