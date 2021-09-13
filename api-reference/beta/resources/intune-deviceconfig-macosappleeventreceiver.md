---
title: тип ресурса macOSAppleEventReceiver
description: Представляет процесс, который может получать уведомление о событии Apple.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a325bed4eca6ca554f391f1127cf454ea50d774a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081334"
---
# <a name="macosappleeventreceiver-resource-type"></a>тип ресурса macOSAppleEventReceiver

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет процесс, который может получать уведомление о событии Apple.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|codeRequirement|String|Требование кода для приложения или двоичного приложения, которое получает событие Apple.|
|идентификатор|String|Набор ID пути приложения или файла процесса или исполняемого, который получает событие Apple.|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|Используйте ID пакета для приложения или пути для процесса или исполняемого, который получает событие Apple. Возможные значения: `bundleID`, `path`.|
|разрешено|Boolean|Разрешить или заблокировать это приложение от получения событий Apple.|

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



