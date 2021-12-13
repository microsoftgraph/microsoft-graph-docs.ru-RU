---
title: linkedResource_v2 типа ресурса
description: Представляет элемент в партнерском приложении, связанном с baseTask
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b3c84cf8c4f08800e22841e6928ef85b1162a2e3
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61425099"
---
# <a name="linkedresource_v2-resource-type"></a>linkedResource_v2 типа ресурса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет элемент в партнерском приложении, связанном с [baseTask.](./basetask.md) В качестве примера можно привести сообщение электронной почты, из которой была создана задача. Объект **linkedResource хранит** сведения об этом источнике приложения и позволяет вернуться к связанному элементу. Вы можете увидеть **linkedResource в** представлении сведений о задачах, как показано.

![Снимок экрана, показывающий связанную карточку ресурса в области сведений о задачах. Карточка связанных ресурсов показывает Open in Jira ( имя приложения-партнера) и план социальных сетей, который является заголовком связанного ресурса.](/graph/images/todo-linkedresource-taskdetail.png)

Некоторые **объекты linkedResource** не связаны с веб-URL-адресами, в этом случае свойство **webUrl** не требуется. Например, связанный элемент может быть из настраиваемого бизнес-приложения или приложения-платформы, например sms-приложения на мобильном телефоне. Вот как **появляется linkedResource с** URL-адресом и без него.

![Изображение, показывающая отображение связанной карточки ресурса с URL-адресом и без него. Связанная карточка ресурса с URL-адресом содержит Имя приложения-партнера, а связанная карточка ресурса без URL-адреса содержит только имя приложения-партнера.](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список linkedResource_v2](../api/basetask-list-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md) коллекции|Получите список объектов [linkedResource_v2](../resources/linkedresource_v2.md) и их свойств.|
|[Создание linkedResource_v2](../api/basetask-post-linkedresources.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Создание нового [linkedResource_v2](../resources/linkedresource_v2.md) объекта.|
|[Получить linkedResource_v2](../api/linkedresource_v2-get.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Ознакомьтесь с свойствами и отношениями linkedResource_v2 [объекта.](../resources/linkedresource_v2.md)|
|[Обновление linkedResource_v2](../api/linkedresource_v2-update.md)|[linkedResource_v2](../resources/linkedresource_v2.md)|Обновление свойств объекта [linkedResource_v2.](../resources/linkedresource_v2.md)|
|[Удаление linkedResource_v2](../api/linkedresource_v2-delete.md)|Нет|Удаляет объект [linkedResource_v2.](../resources/linkedresource_v2.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationName|String|Поле, указывающее имя приложения источника, отправляющее **linkedResource.**|
|displayName|Строка|Поле, указывающее название **linkedResource**.|
|externalId|String|Id объекта, связанного с этой задачей в стороной или партнерской системе.|
|id|Строка|Созданный сервером ID для **linkedResource**. Наследуется от [сущности](../resources/entity.md).|
|webUrl|String|Глубокая ссылка на **linkedResource**.|

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

