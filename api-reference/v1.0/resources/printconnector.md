---
title: тип ресурса printConnector
description: Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c0d24ff6dca0a8866165b40f440ecc2e0d31c1f118d3d3e8a8a41dda96f6038d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205285"
---
# <a name="printconnector-resource-type"></a>тип ресурса printConnector

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет соединители печати, зарегистрированные с помощью подписки универсальной печати. Ресурс printConnector можно использовать для просмотра состояния соединитетеля и обновления свойств.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
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