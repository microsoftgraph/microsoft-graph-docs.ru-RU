---
title: тип ресурса printConnector
description: Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 184a2bc57252b3190754a4eb61e8415114a3c8d0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945014"
---
# <a name="printconnector-resource-type"></a>тип ресурса printConnector

Пространство имен: microsoft.graph

Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Перечисление соединителей](../api/print-list-connectors.md) | [printConnector](printconnector.md) | Извлечение списка соединитений печати. |
| [Получение соединителя](../api/printconnector-get.md) | [printConnector](printconnector.md) | Ознакомьтесь с свойствами и отношениями объекта соединители. |
| [Соединители обновления](../api/printconnector-update.md) | [printConnector](printconnector.md) | Обновление объекта соединители. |
| [Удаление соединителя](../api/printconnector-delete.md) | Нет | Unregister the connector from the Universal Print service. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| Только для чтения.|
|displayName|String|Имя соединитетеля.|
|fullyQualifiedDomainName|String|Имя хост-имени соединители.|
|operatingSystem|String|Версия операционной системы соединитетеля.|
|appVersion|String|Версия соединиттеля.|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение соединитетеля.|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации соединитетеля.|
|registeredBy|[userIdentity](useridentity.md)|Пользователь, зарегистрировавший соединители.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```
