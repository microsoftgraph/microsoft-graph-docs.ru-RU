---
title: тип ресурса serviceAnnouncementAttachment
description: Представляет вложение, связанное с объектом serviceUpdateMessage.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b00cacb19784f34700089d59de22183b8f6e98a
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072760"
---
# <a name="serviceannouncementattachment-resource-type"></a>тип ресурса serviceAnnouncementAttachment

Пространство имен: microsoft.graph

Представляет вложение, связанное с [объектом serviceUpdateMessage.](../resources/serviceupdatemessage.md)

Наследует от [вложения](../resources/attachment.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceAnnouncementAttachment](../api/serviceannouncementattachment-get.md)|[serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|Ознакомьтесь с свойствами и отношениями объекта [serviceAnnouncementAttachment.](../resources/serviceannouncementattachment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|содержимое|Поток|Содержимое вложения.|
|contentType|String|Тип контента этого вложения.|
|id|String|Идентификатор вложения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения вложения.|
|name|String|Имя вложения.|
|size|Int32|Размер вложения в байтах.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncementAttachment",
  "baseType": "microsoft.graph.attachment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncementAttachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": "Integer",
  "isInline": "Boolean",
  "content": "Stream"
}
```
