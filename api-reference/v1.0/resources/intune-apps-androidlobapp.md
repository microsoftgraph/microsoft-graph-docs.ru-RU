---
title: Тип ресурса androidLobApp
description: Содержит свойства, в том числе унаследованные, для бизнес-приложений Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2611cc93f046e2d95d1d6df5287430c65d170bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532860"
---
# <a name="androidlobapp-resource-type"></a>Тип ресурса androidLobApp

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, в том числе унаследованные, для бизнес-приложений Android.


Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление androidLobApps](../api/intune-apps-androidlobapp-list.md)|Коллекция [androidLobApp](../resources/intune-apps-androidlobapp.md)|Список свойств и связей объектов [androidLobApp](../resources/intune-apps-androidlobapp.md).|
|[Получение androidLobApp](../api/intune-apps-androidlobapp-get.md)|[androidLobApp](../resources/intune-apps-androidlobapp.md);|Считывание свойств и связей объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).|
|[Создание androidLobApp](../api/intune-apps-androidlobapp-create.md)|[androidLobApp](../resources/intune-apps-androidlobapp.md);|Создание нового объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).|
|[Удаление androidLobApp](../api/intune-apps-androidlobapp-delete.md)|None|Удаление экземпляра [androidLobApp](../resources/intune-apps-androidlobapp.md).|
|[Обновление androidLobApp](../api/intune-apps-androidlobapp-update.md)|[androidLobApp](../resources/intune-apps-androidlobapp.md)|Обновление свойств объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|Строка|Издатель приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|Строка|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|Строка|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|Строка|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|Строка|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|committedContentVersion|Строка|Внутренняя версия подтвержденного содержимого. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|Строка|Имя основного файла бизнес-приложения. Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|packageId|Строка|Идентификатор пакета.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|
|versionName|Строка|Имя версии бизнес-приложения для Android.|
|versionCode|String|Код версии бизнес-приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "String",
  "versionCode": "String"
}
```




