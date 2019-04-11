---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5652add71ba19b1eba102a0579a787d7410d6c89
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791476"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Тип ресурса Битлоккеррековерйоптионс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры восстановления BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Блоккдатарековеряжент|Boolean|Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.|
|Рековерипассвордусаже|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр. Возможные значения: `blocked`, `required`, `allowed`.|
|Рековерикэйусаже|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска. Возможные значения: `blocked`, `required`, `allowed`.|
|Хидерековерйоптионс|Boolean|Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.|
|Енаблерековеринформатионсаветосторе|Boolean|Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.|
|Рековеринформатионтосторе|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части данных восстановления BitLocker хранятся в AD DS. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|Енаблебитлоккерафтеррековеринформатионтосторе|Boolean|Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.|

## <a name="relationships"></a>Отношения
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





