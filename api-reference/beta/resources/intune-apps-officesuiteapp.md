---
title: Тип ресурса officeSuiteApp
description: Содержит свойства и наследуемые свойства для приложения набора Office365.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c866a4589505af9721d0fc97d16056e90939b19b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199113"
---
# <a name="officesuiteapp-resource-type"></a>Тип ресурса officeSuiteApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и наследуемые свойства для приложения набора Office365.


Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Оффицесуитеаппс](../api/intune-apps-officesuiteapp-list.md)|Коллекция [officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Список свойств и связей объектов [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Получение officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Чтение свойств и связей объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Создание officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Создание нового объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Удаление officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|Нет|Удаляет объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[Обновление officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md);|Обновление свойств объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publisher|String.|Издатель приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).|
|privacyInformationUrl|String.|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|informationUrl|String.|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|developer|String.|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|uploadState|Int32|Состояние отправки. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|аутоакцептеула|Boolean.|Значение, которое будет автоматически принимать условия лицензионного соглашения на устройстве ендусер.|
|productIds|Коллекция [оффицепродуктид](../resources/intune-apps-officeproductid.md)|Идентификаторы продуктов, представляющие SKU набора Office365.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md);|Свойство для представления приложений, исключаемых из выбранного идентификатора продукта Office365.|
|Свойства usesharedcomputeractivation|Boolean.|Свойство для представления того, используется ли активация на общем компьютере не для приложений Office365.|
|updateChannel|[оффицеупдатечаннел](../resources/intune-apps-officeupdatechannel.md)|Свойство для представления канала обновления Office365. Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Свойство для представления версии набора приложений Office365. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|localesToInstall|Коллекция строк|Свойство для представления языковых стандартов, устанавливаемых при установке приложений из Office365. В нем используется стандартная спецификация RFC 6033. Словомhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|инсталлпрогрессдисплайлевел|[оффицесуитеинсталлпрогрессдисплайлевел](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Для указания уровня отображения пользовательского интерфейса установки хода установки на устройстве. Возможные значения: `none`, `full`.|
|шаулдунинсталлолдерверсионсофоффице|Boolean.|Свойство, определяющее, следует ли удалить существующий MSI Office, если на устройстве развернут набор приложений Office365.|
|Атрибута targetversion|String.|Свойство, представляющее определенную целевую версию для набора приложений Office365, который должен быть развернут на устройствах.|
|упдатеверсион|String.|Свойство для представления версии обновления, в которой определенная Целевая версия доступна для набора приложений Office365.|
|оффицеконфигуратионксмл|Binary|Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс. Имеет приоритет над всеми другими свойствами. Если этот параметр указан, для создания приложения будет использоваться XML-файл конфигурации.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Общие сведения по установке мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|Таблица|Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)|Список отношений для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|

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



