---
title: Тип ресурса windowsWebApp
description: Содержит свойства и унаследованные свойства для Windows веб-приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 693949e3940531c52caea71c0173405fc6734c6e
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858897"
---
# <a name="windowswebapp-resource-type"></a>Тип ресурса windowsWebApp

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для Windows веб-приложений.


Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windowsWebApps](../api/intune-apps-windowswebapp-list.md)|[Коллекция windowsWebApp](../resources/intune-apps-windowswebapp.md)|Список свойств и связей объектов [windowsWebApp](../resources/intune-apps-windowswebapp.md) .|
|[Получение windowsWebApp](../api/intune-apps-windowswebapp-get.md)|[windowsWebApp](../resources/intune-apps-windowswebapp.md)|Чтение свойств и связей объекта [windowsWebApp](../resources/intune-apps-windowswebapp.md) .|
|[Создание windowsWebApp](../api/intune-apps-windowswebapp-create.md)|[windowsWebApp](../resources/intune-apps-windowswebapp.md)|Создайте объект [windowsWebApp](../resources/intune-apps-windowswebapp.md) .|
|[Удаление windowsWebApp](../api/intune-apps-windowswebapp-delete.md)|Нет|Удаляет [windowsWebApp](../resources/intune-apps-windowswebapp.md).|
|[Обновление windowsWebApp](../api/intune-apps-windowswebapp-update.md)|[windowsWebApp](../resources/intune-apps-windowswebapp.md)|Обновление свойств объекта [windowsWebApp](../resources/intune-apps-windowswebapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|uploadState|Int32|Состояние отправки. Возможные значения: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению хотя бы одна группа. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|dependentAppCount|Int32|Общее количество зависимостей, которые имеет дочернее приложение. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersedingAppCount|Int32|Общее количество приложений, которые это приложение прямо или косвенно заменяет. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersededAppCount|Int32|Общее количество приложений, на которые это приложение прямо или косвенно заменяется. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|appUrl|String|URL-адрес веб-приложения.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|userStatuses|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|Отношения|[Коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWebApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWebApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
  "appUrl": "String"
}
```




