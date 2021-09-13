---
title: тип ресурса bitLockerRecoveryOptions
description: Параметры восстановления BitLocker.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c9798225a4d9cb6fe44221a7030e6836803ff51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146725"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a>тип ресурса bitLockerRecoveryOptions

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры восстановления BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|blockDataRecoveryAgent|Логический|Указывает, следует ли блокировать агент восстановления данных на основе сертификатов.|
|recoveryPasswordUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешено ли пользователям создавать 48-значный пароль восстановления для фиксированного или системного диска. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|recoveryKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешено ли пользователям создавать 256-битный ключ восстановления для фиксированного или системного диска. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|hideRecoveryOptions|Логическое|Указывает, следует ли разрешить показ параметров восстановления в мастере установки BitLocker для фиксированного или системного диска.|
|enableRecoveryInformationSaveToStore|Логическое|Указывает, следует ли разрешить хранение данных о восстановлении BitLocker в AD DS.|
|recoveryInformationToStore|[bitLockerRecoveryInformationType](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|Настройте, какие части данных восстановления BitLocker хранятся в AD DS. Возможные значения: `passwordAndKey`, `passwordOnly`.|
|enableBitLockerAfterRecoveryInformationToStore|Логическое|Указывает, следует ли включить BitLocker до хранения сведений о восстановлении в AD DS.|

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



