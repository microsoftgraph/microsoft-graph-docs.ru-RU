---
title: Тип ресурса Андроидманажедсторевебапп
description: Содержит свойства и наследуемые свойства для веб-приложений, настроенных для распространения с помощью управляемого хранилища приложений Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68deabf6301673a7cf10bcb2b96fb01b93dcb921
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281987"
---
# <a name="androidmanagedstorewebapp-resource-type"></a>Тип ресурса Андроидманажедсторевебапп

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и наследуемые свойства для веб-приложений, настроенных для распространения с помощью управляемого хранилища приложений Android.


Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидманажедсторевебаппс](../api/intune-apps-androidmanagedstorewebapp-list.md)|Коллекция [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md)|Список свойств и связей объектов [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Получение Андроидманажедсторевебапп](../api/intune-apps-androidmanagedstorewebapp-get.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Чтение свойств и связей объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Создание Андроидманажедсторевебапп](../api/intune-apps-androidmanagedstorewebapp-create.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Создание нового объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Удаление Андроидманажедсторевебапп](../api/intune-apps-androidmanagedstorewebapp-delete.md)|Нет|Удаляет объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md).|
|[Обновление Андроидманажедсторевебапп](../api/intune-apps-androidmanagedstorewebapp-update.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Обновление свойств объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|description|String|Описание приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
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
|uploadState|Int32|Состояние отправки. Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` . Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|суперседингаппкаунт|Int32|Общее количество приложений, которые напрямую или косвенно заменяют данное приложение. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|суперседедаппкаунт|Int32|Общее число приложений, для которых это приложение напрямую или косвенно заменяется. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|packageId|String|Идентификатор пакета. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|appIdentifier|String|Имя удостоверения. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|usedLicenseCount|Int32|Количество используемых лицензий VPP. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|totalLicenseCount|Int32|Общее количество лицензий VPP. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|appStoreUrl|String|URL-адрес приложения для рабочего хранилища. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|Частный|Boolean|Указывает, доступно ли приложение только для указанных пользователей предприятия. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|иссистемапп|Boolean|Указывает, является ли приложение предустановленным системным приложением. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|апптраккс|Коллекция [андроидманажедстореапптракк](../resources/intune-apps-androidmanagedstoreapptrack.md)|Дорожки, которые видимы для этого предприятия. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|
|суппортсоемконфиг|Boolean|Поддерживает ли это приложение политику Оемконфиг. Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|Таблица|Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|Набор прямых отношений для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreWebApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "String",
  "appIdentifier": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "appStoreUrl": "String",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "String",
      "trackAlias": "String"
    }
  ],
  "supportsOemConfig": true
}
```




