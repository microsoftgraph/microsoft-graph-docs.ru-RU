---
title: Тип ресурса Андроидманажедстореапп
description: Содержит свойства и унаследованные свойства для приложений с управляемым хранилищем Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 069d8c26fe1d9ac4a62ff93fdbee81ee0a5b55de
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727584"
---
# <a name="androidmanagedstoreapp-resource-type"></a>Тип ресурса Андроидманажедстореапп

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для приложений с управляемым хранилищем Android.


Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидманажедстореаппс](../api/intune-apps-androidmanagedstoreapp-list.md)|Коллекция [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|Список свойств и связей объектов [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .|
|[Получение Андроидманажедстореапп](../api/intune-apps-androidmanagedstoreapp-get.md)|[андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|Чтение свойств и связей объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .|
|[Создание Андроидманажедстореапп](../api/intune-apps-androidmanagedstoreapp-create.md)|[андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|Создание нового объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .|
|[Удаление Андроидманажедстореапп](../api/intune-apps-androidmanagedstoreapp-delete.md)|Нет|Удаляет объект [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md).|
|[Обновление Андроидманажедстореапп](../api/intune-apps-androidmanagedstoreapp-update.md)|[андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)|Обновление свойств объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
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
|uploadState|Int32|Состояние отправки. Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` . Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|суперседингаппкаунт|Int32|Общее количество приложений, которые напрямую или косвенно заменяют данное приложение. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|суперседедаппкаунт|Int32|Общее число приложений, для которых это приложение напрямую или косвенно заменяется. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|packageId|String|Идентификатор пакета.|
|appIdentifier|String|Имя удостоверения.|
|usedLicenseCount|Int32|Количество используемых лицензий VPP.|
|totalLicenseCount|Int32|Общее количество лицензий VPP.|
|appStoreUrl|String|URL-адрес приложения для рабочего хранилища.|
|Частный|Логический|Указывает, доступно ли приложение только для указанных пользователей предприятия.|
|иссистемапп|Логический|Указывает, является ли приложение предустановленным системным приложением.|
|апптраккс|Коллекция [андроидманажедстореапптракк](../resources/intune-apps-androidmanagedstoreapptrack.md)|Дорожки, которые видимы для этого предприятия.|
|суппортсоемконфиг|Логический|Поддерживает ли это приложение политику Оемконфиг.|

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
  "@odata.type": "microsoft.graph.androidManagedStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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





