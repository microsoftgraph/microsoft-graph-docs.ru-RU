---
title: Тип ресурса Макосаппливентрецеивер
description: Представляет процесс, который может принимать уведомления о событиях Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 073adb9d5a8668d825b3ee7d1fbd6f9fe35131fa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693943"
---
# <a name="macosappleeventreceiver-resource-type"></a>Тип ресурса Макосаппливентрецеивер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет процесс, который может принимать уведомления о событиях Apple.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|кодерекуиремент|Строка|Требования к коду для приложения или двоичных файлов, которые получают событие Apple.|
|идентификатор|Строка|Идентификатор пакета приложения или пути к файлу процесса или исполняемого файла, который получает событие Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Используйте идентификатор пакета для приложения или пути для процесса или исполняемого файла, который получает событие Apple. Возможные значения: `bundleID`, `path`.|
|разрешенных|Логический|Разрешить или запретить получение событий Apple для этого приложения.|

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





