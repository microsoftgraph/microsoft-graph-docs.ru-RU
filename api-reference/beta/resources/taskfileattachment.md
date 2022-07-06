---
title: Тип ресурса taskFileAttachment
description: Представляет файл, например текстовый файл или документ Word, вложенный в todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1724222d362edae4f053af58ce52680052a15be7
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645762"
---
# <a name="taskfileattachment-resource-type"></a>Тип ресурса taskFileAttachment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет файл, например текстовый файл или документ Word, вложенный в [todoTask](../resources/todotask.md).
При создании вложения файла для задачи включите `"@odata.type": "#microsoft.graph.taskFileAttachment"` и имя **свойства и** **contentBytes**.

Наследуется от [attachmentBase](../resources/attachmentbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список вложений](../api/todotask-list-attachments.md)|[Коллекция taskFileAttachment](../resources/taskfileattachment.md)|Получение списка объектов [taskFileAttachment](../resources/taskfileattachment.md) и их свойств.|
|[Создание вложения](../api/todotask-post-attachments.md)|[Коллекция taskFileAttachment](../resources/taskfileattachment.md)|Добавьте новый [объект taskFileAttachment](../resources/taskfileattachment.md) в [todoTask](../resources/todotask.md).|
|[Создание сеанса отправки](../api/taskfileattachment-createuploadsession.md)|[Коллекция taskFileAttachment](../resources/taskfileattachment.md)|Создайте сеанс отправки для итеративной отправки диапазонов файла в виде вложения в [todoTask](../resources/todotask.md).|
|[Получение вложения](../api/taskfileattachment-get.md)|[taskFileAttachment](../resources/taskfileattachment.md)|Чтение свойств и связей объекта [taskFileAttachment](../resources/taskfileattachment.md) .|
|[Удаление вложения](../api/taskfileattachment-delete.md)|Нет|Удаление объекта [taskFileAttachment](../resources/taskfileattachment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentBytes|Двоичный|Содержимое файла в кодировке base64.|
|contentType|String|Тип контента этого вложения. Наследуется от [attachmentBase](../resources/attachmentbase.md).|
|id|String|Идентификатор вложения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения. Наследуется от [attachmentBase](../resources/attachmentbase.md).|
|name|String|Имя текста, отображаемого под значком, представляющий внедренное вложение. Он может не быть фактическим именем файла. Наследуется от [attachmentBase](../resources/attachmentbase.md).|
|size|Int32|Размер вложения в байтах. Наследуется от [attachmentBase](../resources/attachmentbase.md).|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taskFileAttachment",
  "baseType": "microsoft.graph.attachmentBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskFileAttachment",
  "contentBytes": "Binary",
  "contentType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": "Int32"
}
```

