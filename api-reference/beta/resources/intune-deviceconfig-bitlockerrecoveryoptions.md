---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e381b559c291a3da86b7ee6f9a70a67dedf63bb7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260623"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Тип ресурса Битлоккеррековерйоптионс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры восстановления BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|блоккдатарековеряжент|Boolean|Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.|
|рековерипассвордусаже|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|рековерикэйусаже|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|хидерековерйоптионс|Boolean|Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.|
|енаблерековеринформатионсаветосторе|Boolean|Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.|
|рековеринформатионтосторе|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части данных восстановления BitLocker хранятся в AD DS. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|енаблебитлоккерафтеррековеринформатионтосторе|Boolean|Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.|

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




