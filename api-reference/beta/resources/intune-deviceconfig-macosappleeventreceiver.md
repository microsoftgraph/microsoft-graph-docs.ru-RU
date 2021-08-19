---
title: тип ресурса macOSAppleEventReceiver
description: Представляет процесс, который может получать уведомление о событии Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 514caa91cdf788575c7326e7ac2d27a54362891cdb86c96d6e736c4600245b80
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183157"
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




