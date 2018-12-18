---
title: Тип ресурса bitLockerRecoveryOptions
description: Варианты восстановления BitLocker.
author: tfitzmac
ms.openlocfilehash: c85ce3111ed88ce8e8bf54c98d5fd3122571a0be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310607"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Тип ресурса bitLockerRecoveryOptions

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Варианты восстановления BitLocker.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|blockDataRecoveryAgent|Boolean.|Указывает, следует ли блокировать агентом восстановления данных на основе сертификатов.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает ли пользователи могут или должны создавать пароль восстановления из 48 цифр основных или системный диск. Возможные значения: `blocked`, `required`, `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает ли пользователям разрешено или необходимо создание ключа восстановления 256-разрядный основных или системный диск. Возможные значения: `blocked`, `required`, `allowed`.|
|hideRecoveryOptions|Boolean.|Указывает ли разрешать отображение параметры восстановления в мастер установки BitLocker основных или системный диск.|
|enableRecoveryInformationSaveToStore|Boolean.|Указывает, следует ли разрешить сведения о восстановлении BitLocker для хранения в Доменных службах Active Directory.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части сведения о восстановлении BitLocker хранятся в Доменных службах Active Directory. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Boolean.|Указывает, следует ли включить BitLocker до восстановления данные хранятся в Доменных службах Active Directory.|

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





