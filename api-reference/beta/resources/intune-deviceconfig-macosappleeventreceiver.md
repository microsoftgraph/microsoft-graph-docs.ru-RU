---
title: тип ресурса macOSAppleEventReceiver
description: Представляет процесс, который может получать уведомление о событии Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14f68bfa31c41b96e2a2dd160fa732d2c38e9b2f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58810653"
---
# <a name="macosappleeventreceiver-resource-type"></a>тип ресурса macOSAppleEventReceiver

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет процесс, который может получать уведомление о событии Apple.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|codeRequirement|Строка|Требование кода для приложения или двоичного приложения, которое получает событие Apple.|
|идентификатор|Строка|Набор ID пути приложения или файла процесса или исполняемого, который получает событие Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Используйте ID пакета для приложения или пути для процесса или исполняемого, который получает событие Apple. Возможные значения: `bundleID`, `path`.|
|разрешено|Логический|Разрешить или заблокировать это приложение от получения событий Apple.|

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



