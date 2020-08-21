---
title: Тип ресурса linkedResource
description: Представляет источник объекта todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a386cd8ed714a6f7127ea0a872a4170997bb8b9
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850081"
---
# <a name="linkedresource-resource-type"></a>Тип ресурса linkedResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элемент в партнерском приложении, связанном [с todoTask.](./todotask.md) В качестве примера можно приступить к созданию задачи. В **объекте linkedResource** хранятся сведения о исходном приложении и позволяет связывать его обратно с соответствующим элементом.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление linkedResources](../api/todotask-list-linkedresources.md)|[Коллекция linkedResource](../resources/linkedresource.md)|Получение linkedResources из свойства навигации linkedResources.|
|[Создание linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Создание объекта linkedResources.|
|[Получение linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|Чтение свойств и связей [объекта linkedResource.](../resources/linkedresource.md)|
|[Обновление linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|Обновление свойств объекта [linkedResource.](../resources/linkedresource.md)|
|[Удаление linkedResource](../api/linkedresource-delete.md)|Нет|Удаляет объект [linkedResource.](../resources/linkedresource.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationName|String|Поле, указывающее имя приложения источника, отправляющего **linkedResource.**|
|displayName|String|Поле, обозначающее **заголовок связанного ресурса.**|
|externalId|String|Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе.|
|id|String|Созданный сервером ИД **для linkedResource.** Наследуется от [объекта.](../resources/entity.md)|
|webUrl|String|Глубокая ссылка **на связанныйресурс.**|

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

