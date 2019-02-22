---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94481902b7038ab9de9c845c938aac9bc9d409b9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154924"
---
# <a name="mobileapp-resource-type"></a>Тип ресурса mobileApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileApps](../api/intune-apps-mobileapp-list.md)|Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)|Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).|
|[Получение объекта mobileApp](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|[assign action](../api/intune-apps-mobileapp-assign.md)|Нет|Н/Д|
|[Функция getMobileAppCount](../api/intune-apps-mobileapp-getmobileappcount.md)|Int64|Н/Д|
|[Функция getTopMobileApps](../api/intune-apps-mobileapp-gettopmobileapps.md)|Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|String|Администратор предоставил или импортировал название приложения.|
|description|Строка|Описание приложения.|
|publisher|String|Издатель приложения.|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Большой значок, отображается в сведениях о приложении и используется для отправки значка.|
|createdDateTime|DateTimeOffset|Дата и время создания приложения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения.|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором.|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности.|
|informationUrl|String|URL-адрес с дополнительными сведениями.|
|owner|String|Владелец приложения.|
|developer|String|Разработчик приложения.|
|notes|String|Примечания к приложению.|
|uploadState|Int32|Состояние отправки.|
|publishingState|[Мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации приложения. Приложение не может быть назначено, если оно не опубликовано. Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Логический|Значение, указывающее, назначено ли приложение по крайней мере одной группе.|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения.|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения.|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Сводка по установке мобильного приложения.|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения.|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  ]
}
```




