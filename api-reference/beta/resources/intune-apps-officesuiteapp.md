---
title: Тип ресурса officeSuiteApp
description: Содержит свойства и унаследованные свойства для приложения Office365 Suite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efee048d20eeb006057381203d23d1ecfcb22668
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669282"
---
# <a name="officesuiteapp-resource-type"></a>Тип ресурса officeSuiteApp

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и унаследованные свойства для приложения Office365 Suite.


Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[Коллекция officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Список свойств и связей объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Получение officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Чтение свойств и связей объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Создание officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Создайте объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Удаление officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|Нет|Удаляет [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[Обновление officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Обновление свойств объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|

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
|Идентификаторы roleScopeTagId|Коллекция String|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|dependentAppCount|Int32|Общее количество зависимостей, которые имеет дочернее приложение. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|supersedingAppCount|Int32|Общее количество приложений, которые это приложение прямо или косвенно заменяет. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|supersededAppCount|Int32|Общее количество приложений, на которые это приложение прямо или косвенно заменяется. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|autoAcceptEula|Логическое|Значение для автоматического принятия лицензионного соглашения на устройстве конечного пользователя.|
|идентификаторы продуктов|[Коллекция officeProductId](../resources/intune-apps-officeproductid.md)|Идентификаторы продуктов, которые представляют номер SKU Office365 Suite.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md);|Свойство, представляющее приложения, исключенные из выбранного идентификатора продукта Office365.|
|useSharedComputerActivation|Логическое|Свойство, указывающее, используется ли активация общего компьютера не для набора приложений Office 365.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|Свойство, представляющее канал обновления Office365. Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md);|Свойство, представляющее версию набора приложений Office 365. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|localesToInstall|Коллекция объектов string|Свойство, представляющее языковые стандарты, установленные при установке приложений из Office365. В нем используется стандарт RFC 6033. Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Чтобы указать уровень отображения пользовательского интерфейса установки хода установки на устройстве. Возможные значения: `none`, `full`.|
|shouldUninstallOlderVersionsOfOffice|Логический|Свойство, определяющее, следует ли удалять существующие MSI Office, если набор приложений Office365 развернут на устройстве или нет.|
|targetVersion|String|Свойство, представляющее конкретную целевую версию для набора приложений Office 365, который должен быть развернут на устройствах.|
|updateVersion|String|Свойство, представляющее версию обновления, в которой конкретная целевая версия доступна для набора приложений Office365.|
|officeConfigurationXml|Binary|Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс. Имеет приоритет над всеми другими свойствами. При наличии XML-файла конфигурации будет использоваться для создания приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|Отношения|[Коллекция mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Набор прямых связей для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|

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
  "dependentAppCount": 1024,
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
  "autoAcceptEula": true,
  "productIds": [
    "String"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
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
    "teams": true,
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




