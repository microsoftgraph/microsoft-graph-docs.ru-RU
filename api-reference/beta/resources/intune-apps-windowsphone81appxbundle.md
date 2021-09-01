---
title: тип ресурса windowsPhone81AppXBundle
description: Содержит свойства и унаследованные свойства для Windows Phone 8.1 Линейка пакетов AppX для бизнес-приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 985fed8214f31651b3daa592adee7ec5945a129c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783976"
---
# <a name="windowsphone81appxbundle-resource-type"></a>тип ресурса windowsPhone81AppXBundle

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для Windows Phone 8.1 Линейка пакетов AppX для бизнес-приложений.


Наследует [от windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsPhone81AppXBundles](../api/intune-apps-windowsphone81appxbundle-list.md)|[коллекция windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Список свойств и связей [объектов WindowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)|
|[Получить windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-get.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Чтение свойств и связей [объекта WindowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)|
|[Создание windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-create.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Создайте [новый объект WindowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)|
|[Удаление windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-delete.md)|Нет|Удаляет [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).|
|[Обновление windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-update.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Обновление свойств объекта [WindowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)|

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
|uploadState|Int32|Состояние загрузки. Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` . Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению по крайней мере одна группа. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция String|Список ids тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|dependentAppCount|Int32|Общее число зависимостей, которые имеет детское приложение. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersedingAppCount|Int32|Общее число приложений, которые это приложение прямо или косвенно перемежает. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|supersededAppCount|Int32|Общее число приложений, которые это приложение прямо или косвенно вымежает. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Архитектура Windows, которая поддерживается этим приложением. Унаследовано от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md). Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|identityName|String|Имя удостоверения. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityPublisherHash|String|Хэш издателей удостоверений. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityResourceIdentifier|String|Идентификатор ресурса Identity. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|phoneProductIdentifier|Строка|Идентификатор Телефон продукта. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|phonePublisherId|Строка|The Телефон Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityVersion|String|Версия удостоверения. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|appXPackageInformationList|[коллекция windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)|Список сведений о пакете AppX.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|deviceStatuses|[коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояния установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|userStatuses|[коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояния установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|отношения|[коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|contentVersions|Коллекция [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81AppXBundle"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "applicableArchitectures": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true,
    "v10_2H20": true,
    "v10_21H1": true
  },
  "phoneProductIdentifier": "String",
  "phonePublisherId": "String",
  "identityVersion": "String",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "String",
      "displayName": "String",
      "identityName": "String",
      "identityPublisher": "String",
      "identityResourceIdentifier": "String",
      "identityVersion": "String",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true,
        "v10_1909": true,
        "v10_2004": true,
        "v10_2H20": true,
        "v10_21H1": true
      }
    }
  ]
}
```



