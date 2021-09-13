---
title: тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) подключения.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dac175f73b517e3f96c6d5e03ce747d32b2b8f64
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123463"
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
|id|Строка| Уникальный идентификатор для подключенияOperation. Только для чтения. |
|status|microsoft.graph.externalConnectors.connectionOperationStatus| Указывает состояние асинхронной операции. Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.|

## <a name="relationships"></a>Отношения
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

