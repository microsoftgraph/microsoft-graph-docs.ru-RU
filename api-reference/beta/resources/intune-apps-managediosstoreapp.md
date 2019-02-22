---
title: Тип ресурса managedIOSStoreApp
description: Содержит свойства, в том числе унаследованные, для приложения из магазина iOS, которым вы можете управлять с помощью политики защиты приложений Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 002748469ffd22dade862556191f3c2d1aafa31e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165697"
---
# <a name="managediosstoreapp-resource-type"></a>Тип ресурса managedIOSStoreApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, в том числе унаследованные, для приложения из магазина iOS, которым вы можете управлять с помощью политики защиты приложений Intune.


Наследуется от [managedApp](../resources/intune-apps-managedapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedIOSStoreApps](../api/intune-apps-managediosstoreapp-list.md)|Коллекция [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)|Список свойств и связей объектов [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Получение managedIOSStoreApp](../api/intune-apps-managediosstoreapp-get.md)|[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md);|Считывание свойств и связей объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Создание managedIOSStoreApp](../api/intune-apps-managediosstoreapp-create.md)|[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md);|Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Удаление managedIOSStoreApp](../api/intune-apps-managediosstoreapp-delete.md)|None|Удаление экземпляра [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Обновление managedIOSStoreApp](../api/intune-apps-managediosstoreapp-update.md)|[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)|Обновление свойств объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
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
|uploadState|Int32|Состояние отправки. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[Мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Логический|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|appAvailability|[Манажедаппаваилабилити](../resources/intune-apps-managedappavailability.md)|Доступность приложения. НаСледуется от [managedApp](../resources/intune-apps-managedapp.md). Возможные значения: `global`, `lineOfBusiness`.|
|version|Строка|Версия приложения. Наследуется от [managedApp](../resources/intune-apps-managedapp.md)|
|bundleId|String|Идентификатор пакета приложения.|
|appStoreUrl|String|AppStoreUrl для Apple.|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|Архитектура iOS, поддерживаемая этим приложением.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosminimumoperatingsystem.md)|Значение, которое представляет минимальную поддерживаемую версию операционной системы.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Сводка по установке мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "version": "String",
  "bundleId": "String",
  "appStoreUrl": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```




