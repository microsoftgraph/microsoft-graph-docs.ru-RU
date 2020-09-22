---
title: Тип ресурса Макосаппливентрецеивер
description: Представляет процесс, который может принимать уведомления о событиях Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db781ad536e8fe918257f74d87fa104f4b2a23f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055451"
---
# <a name="macosappleeventreceiver-resource-type"></a>Тип ресурса Макосаппливентрецеивер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет процесс, который может принимать уведомления о событиях Apple.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|кодерекуиремент|String|Требования к коду для приложения или двоичных файлов, которые получают событие Apple.|
|идентификатор|String|Идентификатор пакета приложения или пути к файлу процесса или исполняемого файла, который получает событие Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Используйте идентификатор пакета для приложения или пути для процесса или исполняемого файла, который получает событие Apple. Возможные значения: `bundleID`, `path`.|
|разрешенных|Boolean|Разрешить или запретить получение событий Apple для этого приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```






