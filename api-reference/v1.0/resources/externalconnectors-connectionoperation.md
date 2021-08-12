---
title: тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7cf9310eef057bbd4bcda57273089f05a24501986c90b6bffbc072d39932cac2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121286"
---
# <a name="connectionoperation-resource-type"></a>тип ресурса connectionOperation

Пространство имен: microsoft.graph.externalConnectors



Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) [подключения.](externalconnectors-schema.md)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get connectionOperation](../api/externalconnectors-connectionoperation-get.md)|[connectionOperation](../resources/externalconnectors-connectionoperation.md)|Ознакомьтесь с свойствами и отношениями объекта [connectionOperation.](../resources/externalconnectors-connectionoperation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|error|publicError| Если `status` это `failed` так, предоставляет дополнительные сведения об ошибке, которая привела к сбою.|
|id|String| Уникальный идентификатор для подключенияOperation. Только для чтения. |
|status|microsoft.graph.externalConnectors.connectionOperationStatus| Указывает состояние асинхронной операции. Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "status": "String"
}
```

