---
title: Тип ресурса bitLockerRecoveryOptions
description: Варианты восстановления BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398515"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>Тип ресурса bitLockerRecoveryOptions

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Варианты восстановления BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|blockDataRecoveryAgent|Логический|Указывает, следует ли блокировать агентом восстановления данных на основе сертификатов.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает ли пользователи могут или должны создавать пароль восстановления из 48 цифр основных или системный диск. Возможные значения: `blocked`, `required`, `allowed`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает ли пользователям разрешено или необходимо создание ключа восстановления 256-разрядный основных или системный диск. Возможные значения: `blocked`, `required`, `allowed`.|
|hideRecoveryOptions|Логический|Указывает ли разрешать отображение параметры восстановления в мастер установки BitLocker основных или системный диск.|
|enableRecoveryInformationSaveToStore|Логический|Указывает, следует ли разрешить сведения о восстановлении BitLocker для хранения в Доменных службах Active Directory.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части сведения о восстановлении BitLocker хранятся в Доменных службах Active Directory. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Логический|Указывает, следует ли включить BitLocker до восстановления данные хранятся в Доменных службах Active Directory.|

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




