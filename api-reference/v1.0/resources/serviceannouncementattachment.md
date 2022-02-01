---
title: тип ресурса serviceAnnouncementAttachment
description: Представляет вложение, связанное с объектом serviceUpdateMessage.
author: payiAzure
ms.localizationpriority: medium
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 7acc5906e0054ccd78097caff0863c651fa97dd3
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291262"
---
# <a name="serviceannouncementattachment-resource-type"></a>тип ресурса serviceAnnouncementAttachment

Пространство имен: microsoft.graph

Представляет вложение, связанное с [объектом serviceUpdateMessage](../resources/serviceupdatemessage.md) .

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get serviceAnnouncementAttachment](../api/serviceannouncementattachment-get.md)|[serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md)|Ознакомьтесь с свойствами и отношениями объекта [serviceAnnouncementAttachment](../resources/serviceannouncementattachment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|содержимое|Поток|Содержимое вложения.|
|contentType|String|Тип контента этого вложения.|
|id|String|Идентификатор вложения. Наследуется [от сущности](../resources/entity.md).|
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
