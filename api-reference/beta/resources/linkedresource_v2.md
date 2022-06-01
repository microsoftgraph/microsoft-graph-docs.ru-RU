---
title: linkedResource_v2 типа ресурса
description: Представляет элемент в партнерского приложения, связанного с baseTask
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 720fd4e10664f4f83a0c050d6b4838d68e3f59c7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821003"
---
# <a name="linkedresource_v2-resource-type-deprecated"></a>linkedResource_v2 ресурса (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Представляет элемент в партнерского приложения, связанного с [baseTask](./basetask.md). Примером является сообщение электронной почты, из которого была создана задача. Объект **linkedResource** хранит сведения об этом исходном приложении и позволяет вернуться к связанному элементу. **LinkedResource можно увидеть в** представлении сведений о задаче, как показано ниже.

![Снимок экрана: карточка связанного ресурса в области сведений о задаче. На карточке связанного ресурса отображается окно "Открыть в Jira", которое является именем партнерского приложения, и "План социальных сетей", который является заголовком связанного ресурса.](/graph/images/todo-linkedresource-taskdetail.png)

Некоторые **объекты linkedResource** не связаны с веб-URL-адресами, в этом случае свойство **webUrl** не требуется. Например, связанный элемент может быть из пользовательского бизнес-приложения или приложения собственной платформы, например из SMS на мобильном телефоне. Вот как отображается **linkedResource** с URL-адресом и без нее.

![Изображение, показывающее, как отображается связанная карточка ресурса с URL-адресом и без нее. Связанная карточка ресурса с URL-адресом содержит open with partner application Name, а карточка связанного ресурса без URL-адреса содержит только имя приложения партнера.](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список linkedResource_v2](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Получение списка [объектов linkedResource_v2 и](../resources/linkedresource_v2.md) их свойств.|
|[Создание linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Создайте [новый linkedResource_v2](../resources/linkedresource_v2.md) объекта.|
|[Получение linkedResource_v2](../api/linkedresource_v2-get.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Чтение свойств и связей [linkedResource_v2 объекта](../resources/linkedresource_v2.md) .|
|[Обновление linkedResource_v2](../api/linkedresource_v2-update.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Обновите [свойства linkedResource_v2 объекта](../resources/linkedresource_v2.md) .|
|[Удаление linkedResource_v2](../api/linkedresource_v2-delete.md)|Нет|Удаляет [linkedResource_v2 объекта.](../resources/linkedresource_v2.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationName|String|Поле, указывающее имя приложения источника, отправляющего **linkedResource**.|
|displayName|Строка|Поле, указывающее заголовок **объекта linkedResource**.|
|externalId|String|Идентификатор объекта, связанного с этой задачей в сторонней или партнерской системе.|
|id|Строка|Идентификатор, созданный сервером для **linkedResource**. Наследуется от [сущности](../resources/entity.md).|
|webUrl|String|Прямая ссылка на **linkedResource**.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource_v2",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource_v2",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)"
}
```

