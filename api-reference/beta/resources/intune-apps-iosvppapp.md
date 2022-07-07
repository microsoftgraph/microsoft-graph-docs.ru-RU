---
title: Тип ресурса iosVppApp
description: Содержит свойства, в том числе унаследованные, для приложений iOS, на которые распространяется программа VPP (Volume Purchase Program).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39721d6f8f211763a4519c3d36656bf6b5012e08
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666846"
---
# <a name="iosvppapp-resource-type"></a>Тип ресурса iosVppApp

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, в том числе унаследованные, для приложений iOS, на которые распространяется программа VPP (Volume Purchase Program).


Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosVppApps](../api/intune-apps-iosvppapp-list.md)|Коллекция [iosVppApp](../resources/intune-apps-iosvppapp.md)|Список свойств и связей объектов [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Получение iosVppApp](../api/intune-apps-iosvppapp-get.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|Считывание свойств и связей объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Создание iosVppApp](../api/intune-apps-iosvppapp-create.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|Создание нового объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Удаление iosVppApp](../api/intune-apps-iosvppapp-delete.md)|None|Удаление экземпляра [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Обновление iosVppApp](../api/intune-apps-iosvppapp-update.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|Обновление свойств объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Действие revokeAllLicenses](../api/intune-apps-iosvppapp-revokealllicenses.md)|Нет|Отмените все назначенные лицензии IOS VPP для данного приложения.|
|[Действие revokeAllLicenses](../api/intune-apps-iosvppapp-revokeuserlicense.md)|Нет|Отмените назначенную пользователем лицензию IOS VPP для данного приложения.|
|[Действие revokeAllLicenses](../api/intune-apps-iosvppapp-revokedevicelicense.md)|Нет|Отмените назначенную лицензию на устройство IOS VPP для данного приложения.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|String|Описание приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Состояние отправки. Возможные значения: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложению хотя бы одна группа. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Идентификаторы roleScopeTagId|Коллекция объектов string|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|dependentAppCount|Int32|Общее количество зависимостей, которые имеет дочернее приложение. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|supersedingAppCount|Int32|Общее количество приложений, которые это приложение прямо или косвенно заменяет. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|supersededAppCount|Int32|Общее количество приложений, на которые это приложение прямо или косвенно заменяется. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|usedLicenseCount|Int32|Количество используемых лицензий VPP.|
|totalLicenseCount|Int32|Общее количество лицензий VPP.|
|releaseDateTime|DateTimeOffset|Дата и время выпуска приложения, на которое распространяется программа VPP.|
|appStoreUrl|String|URL-адрес магазина.|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|Поддерживаемый тип лицензии.|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|Применимый тип устройства с iOS.|
|vppTokenOrganizationName|String|Организация, связанная с токеном Apple Volume Purchase Program.|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program. Возможные значения: `business`, `education`. Возможные значения: `business`, `education`.|
|vppTokenAppleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|bundleId|String|Имя удостоверения.|
|vppTokenId|String|Идентификатор маркера VPP, связанного с этим приложением.|
|revokeLicenseActionResults|[Коллекция iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)|Результаты действий по отмене лицензии для этого приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Отношения|[Коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignedLicenses|[Коллекция iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Лицензии, назначенные этому приложению.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "releaseDateTime": "String (timestamp)",
  "appStoreUrl": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "String",
  "vppTokenAccountType": "String",
  "vppTokenAppleId": "String",
  "bundleId": "String",
  "vppTokenId": "String",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "String",
      "managedDeviceId": "String",
      "totalLicensesCount": 1024,
      "failedLicensesCount": 1024,
      "actionFailureReason": "String",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ]
}
```




