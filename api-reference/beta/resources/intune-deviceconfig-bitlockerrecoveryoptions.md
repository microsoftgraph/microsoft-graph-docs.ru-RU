---
title: Тип ресурса bitLockerRecoveryOptions
description: Варианты восстановления BitLocker.
ms.openlocfilehash: 46af5b52d8305932d0d67ef57d6a1f356182a469
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076870"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Тип ресурса bitLockerRecoveryOptions

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Варианты восстановления BitLocker.
## <a name="properties"></a>Свойства
|Свойство|Тип|Description|
|:---|:---|:---|
|blockDataRecoveryAgent|Логический|Указывает, следует ли блокировать агентом восстановления данных на основе сертификатов.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает ли пользователи могут или должны создавать пароль восстановления из 48 цифр основных или системный диск. Возможные значения: `blocked`, `required`, `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает ли пользователям разрешено или необходимо создание ключа восстановления 256-разрядный основных или системный диск. Возможные значения: `blocked`, `required`, `allowed`.|
|hideRecoveryOptions|Логический|Указывает ли разрешать отображение параметры восстановления в мастер установки BitLocker основных или системный диск.|
|enableRecoveryInformationSaveToStore|Логический|Указывает, следует ли разрешить сведения о восстановлении BitLocker для хранения в Доменных службах Active Directory.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части сведения о восстановлении BitLocker хранятся в Доменных службах Active Directory. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Логический|Указывает, следует ли включить BitLocker до восстановления данные хранятся в Доменных службах Active Directory.|

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





