---
title: Тип ресурса mobileLobApp
description: Абстрактный базовый класс, содержащий свойства для всех мобильных бизнес-приложений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce14b34cbf1eff0d0c90b6e086e5668e379ca84c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949817"
---
# <a name="mobilelobapp-resource-type"></a>Тип ресурса mobileLobApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный базовый класс, содержащий свойства для всех мобильных бизнес-приложений.


Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление mobileLobApps](../api/intune-apps-mobilelobapp-list.md)|Коллекция [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|Список свойств и связей объектов [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|[Получение mobileLobApp](../api/intune-apps-mobilelobapp-get.md)|[mobileLobApp](../resources/intune-apps-mobilelobapp.md)|Считывание свойств и связей объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

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
|uploadState|Int32|Состояние отправки. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[Мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|committedContentVersion|Строка|Внутренняя версия подтвержденного содержимого.|
|fileName|String|Имя основного файла бизнес-приложения.|
|size|Int64|Общий размер, включая все отправленные файлы.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Таблица|Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|Список отношений для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|contentVersions|Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список версий содержимого для этого приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```




