---
title: Тип ресурса Линкедресаурце
description: Представляет источник Тодотаск
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3cbfaa0bf809a1996fe7a7c7df7014324406bcf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058111"
---
# <a name="linkedresource-resource-type"></a>Тип ресурса Линкедресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элемент партнерского приложения, связанный с [тодотаск](./todotask.md). Примером является сообщение электронной почты, создавшее задачу. Объект **линкедресаурце** хранит сведения об этом исходном приложении и позволяет вернуться обратно к связанному элементу.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Линкедресаурцес](../api/todotask-list-linkedresources.md)|Коллекция [линкедресаурце](../resources/linkedresource.md)|Получение Линкедресаурцес из свойства навигации Линкедресаурцес.|
|[Создание Линкедресаурце](../api/todotask-post-linkedresources.md)|[линкедресаурце](../resources/linkedresource.md)|Создание нового объекта Линкедресаурцес.|
|[Получение Линкедресаурце](../api/linkedresource-get.md)|[линкедресаурце](../resources/linkedresource.md)|Чтение свойств и связей объекта [линкедресаурце](../resources/linkedresource.md) .|
|[Обновление Линкедресаурце](../api/linkedresource-update.md)|[линкедресаурце](../resources/linkedresource.md)|Обновление свойств объекта [линкедресаурце](../resources/linkedresource.md) .|
|[Удаление Линкедресаурце](../api/linkedresource-delete.md)|Нет|Удаляет объект [линкедресаурце](../resources/linkedresource.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationName|String|Поле, указывающее имя приложения источника, отправляющего **линкедресаурце**.|
|displayName|String|Поле, указывающее название **линкедресаурце**.|
|externalId|String|Идентификатор объекта, связанного с этой задачей в сторонней системе или партнерской системе.|
|id|String|Созданный сервером идентификатор **линкедресаурце**. Наследуется от [объекта Entity](../resources/entity.md).|
|webUrl|String|Глубокая ссылка на **линкедресаурце**.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```



