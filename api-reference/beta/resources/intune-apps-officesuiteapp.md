---
title: Тип ресурса officeSuiteApp
description: Содержит свойства и наследуемые свойства для приложения набора приложений Office 365.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2be565af88961ebafe4ed978524763797a3fe475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395533"
---
# <a name="officesuiteapp-resource-type"></a>Тип ресурса officeSuiteApp

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и наследуемые свойства для приложения набора приложений Office 365.


Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md) коллекции|Свойства списка и связей объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Получение officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Чтение свойства и связи объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Создание officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Создание нового объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Удаление officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|Нет|Удаляет [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[Обновление officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Обновление свойства объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|

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
|autoAcceptEula|Логический|Значение, чтобы принять условия лицензионного соглашения автоматически на устройстве enduser.|
|productIds|[officeProductId](../resources/intune-apps-officeproductid.md) коллекции|Коды продуктов, представляющих SKU набора приложений Office 365.|
|excludedApps;|[excludedApps](../resources/intune-apps-excludedapps.md);|Свойство для представления приложения, исключенных из выбранного продукта Office 365 идентификатор.|
|useSharedComputerActivation|Логический|Свойство для представления, является ли активация совместно используемый компьютер используется не для набора приложений Office 365.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|Свойство для представления канала обновления Office 365. Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Свойство для представления версию пакета приложения Office 365. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|localesToInstall|Коллекция String|Свойство для представления языковых стандартов, которые устанавливаются при установке приложения из Office 365. Используется стандартный 6033 RFC. Параметры REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Чтобы задать уровень отображения для пользовательского интерфейса программы установки ход выполнения установки на устройстве. Возможные значения: `none`, `full`.|
|shouldUninstallOlderVersionsOfOffice|Логический|Свойство, позволяющее определить, нужно ли удалить существующий MSI Office, если пакет приложений Office 365 развертывается на устройство или нет.|
|targetVersion|String|Свойство для представления конкретной версия набора приложений Office 365, должны оставаться развернутое на устройствах.|
|updateVersion|String|Свойство для представления версии обновления, в котором версия целевой доступна для набора приложений Office 365.|
|officeConfigurationXml|Binary|Свойство для представления XML-файл конфигурации, который может использоваться для приложений Office профессиональный плюс. Приоритет над другие свойства. Если этот параметр указан, XML-файл конфигурации будет использоваться для создания приложения.|

## <a name="relationships"></a>Отношения
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
  "@odata.type": "microsoft.graph.officeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "String"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "String",
  "officePlatformArchitecture": "String",
  "localesToInstall": [
    "String"
  ],
  "installProgressDisplayLevel": "String",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "String",
  "updateVersion": "String",
  "officeConfigurationXml": "binary"
}
```




