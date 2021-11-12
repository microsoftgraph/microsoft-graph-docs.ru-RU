---
title: тип ресурса печати
description: В сопровождении подписки универсальной печати функция Print позволяет управлять принтерами и открывать печатные точки, которые можно использовать для управления принтерами и заданиями печати в Universal Print.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 018ec497e5eccc94b668fe86d2a2d691c58f98d2
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936994"
---
# <a name="print-resource-type"></a>тип ресурса печати

Пространство имен: microsoft.graph

В сопровождении подписки универсальной печати функция Print позволяет управлять принтерами и открывать печатные [точки,](printserviceendpoint.md) которые можно использовать для управления принтерами и заданиями печати в Universal Print.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Перечисление соединителей](../api/print-list-connectors.md) | [коллекция printConnector](printconnector.md) | Получите список соединители печати. |
| [Перечисление принтеров](../api/print-list-printers.md) | [коллекция принтеров](printer.md) | Получите список принтеров. |
| [Перечисление общих ресурсов](../api/print-list-shares.md) | [коллекция printerShare](printershare.md) | Получите список акций принтера. |
| [Службы списка](../api/print-list-services.md) | [коллекция printService](printservice.md) | Получите список служб. |
| [Создание printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Создайте новую долю принтера, разместив в **коллекции акций.** |
| [Создание принтера](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Обновление параметров](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Обновляет параметры для службы универсальной печати для клиента. |
| [Перечисление taskDefinitions](../api/print-list-taskdefinitions.md) | [printTaskDefinition collection](printtaskdefinition.md) | Получите список распечатокTaskDefinitions, созданных в универсальной печати. |
| [Создание taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте новый шрифтTaskDefinition. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settings|[printSettings](../resources/printsettings.md)|Параметры для службы универсальной печати для клиента.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|службы|[коллекция printService](printservice.md)|Список доступных конечных точек службы универсальной печати.|
|принтеры|[коллекция принтеров](printer.md)|Список принтеров, зарегистрированных в клиенте.|
|shares|[коллекция printerShare](printershare.md)|Список акций принтера, зарегистрированных в клиенте.|
|соединители|[коллекция printConnector](printconnector.md)|Список доступных соединители печати.|
|operations|[коллекция printOperation](../resources/printoperation.md)|Список длительных операций печати.|
|службы|[коллекция printService](../resources/printservice.md)|Список экземпляров служб печати для различных компонентов инфраструктуры печати.|
|taskDefinitions|[printTaskDefinition collection](../resources/printtaskdefinition.md)|Список абстрактного определения задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

