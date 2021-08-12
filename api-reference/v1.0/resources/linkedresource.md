---
title: тип ресурса linkedResource
description: Представляет источник todoTask
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8164e0436cdedee66c59fbc83b7f4fa7d594a4623c2a62bcab6d19cca4c52d28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237630"
---
# <a name="linkedresource-resource-type"></a>тип ресурса linkedResource

Пространство имен: microsoft.graph


Представляет элемент в партнерском приложении, связанном с [todoTask.](./todotask.md) В качестве примера можно привести сообщение электронной почты, из которой была создана задача. Объект **linkedResource хранит** сведения об этом источнике приложения и позволяет вернуться к связанному элементу. Вы можете увидеть **linkedResource в** представлении сведений о задачах, как показано.

![Связанный ресурс в области сведений о задачах](/graph/images/todo-linkedresource-taskdetail.png)

Некоторые **объекты linkedResource** не связаны с веб-URL-адресами, в этом случае свойство **webUrl** не требуется. Например, связанный элемент может быть из настраиваемого бизнес-приложения или приложения-платформы, например sms-приложения на мобильном телефоне. Вот как **появляется linkedResource с** URL-адресом и без него.

![Связанный ресурс с URL-адресом и без него](/graph/images/todo-linkedresource.png)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список linkedResources](../api/todotask-list-linkedresources.md)|[коллекция linkedResource](../resources/linkedresource.md)|Получите linkedResources из свойства навигации linkedResources.|
|[Создание linkedResource](../api/todotask-post-linkedresources.md)|[linkedResource](../resources/linkedresource.md)|Создайте новый объект linkedResources.|
|[Получить linkedResource](../api/linkedresource-get.md)|[linkedResource](../resources/linkedresource.md)|Ознакомьтесь с свойствами и отношениями объекта [linkedResource.](../resources/linkedresource.md)|
|[Обновление linkedResource](../api/linkedresource-update.md)|[linkedResource](../resources/linkedresource.md)|Обновление свойств объекта [linkedResource.](../resources/linkedresource.md)|
|[Удаление linkedResource](../api/linkedresource-delete.md)|Нет|Удаляет объект [linkedResource.](../resources/linkedresource.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationName|String|Поле, указывающее имя приложения источника, отправляющее **linkedResource.**|
|displayName|String|Поле, указывающее название **linkedResource**.|
|externalId|String|Id объекта, связанного с этой задачей в стороной или партнерской системе.|
|id|String|Созданный сервером ID для **linkedResource**. Наследуется от [сущности](../resources/entity.md).|
|webUrl|String|Глубокая ссылка на **linkedResource**.|

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



