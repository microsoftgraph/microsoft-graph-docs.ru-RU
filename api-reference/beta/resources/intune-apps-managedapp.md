---
title: Тип ресурса managedApp
description: Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 25fb9d2fc774aa370728077a28687514e47d04b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422812"
---
# <a name="managedapp-resource-type"></a>Тип ресурса managedApp

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.


Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedApps](../api/intune-apps-managedapp-list.md)|Коллекция [managedApp](../resources/intune-apps-managedapp.md)|Список свойств и связей объектов [managedApp](../resources/intune-apps-managedapp.md).|
|[Получение managedApp](../api/intune-apps-managedapp-get.md)|[managedApp](../resources/intune-apps-managedapp.md)|Считывание свойств и связей объекта [managedApp](../resources/intune-apps-managedapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|String|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Большой значок, который отображается в сведениях о приложении и используется для отправки значка. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Примечания к приложению. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Состояние передачи. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Логический|Значение, указывающее, назначена ли приложение по крайней мере одной группы. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|roleScopeTagIds|Коллекция String|Список идентификаторов тег области для данного мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|Доступность приложения. Возможные значения: `global`, `lineOfBusiness`.|
|version|String|Версия приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Сводка по установке мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) коллекции|Список состояния установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) коллекции|Список состояния установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
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
  "appAvailability": "String",
  "version": "String"
}
```




