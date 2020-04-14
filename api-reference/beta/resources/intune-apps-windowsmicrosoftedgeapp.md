---
title: Тип ресурса Виндовсмикрософтеджеапп
description: Содержит свойства и наследуемые свойства для приложения Microsoft EDGE в Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c9f6b487803a26781bc9b9aafeabc16fe29f173
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450761"
---
# <a name="windowsmicrosoftedgeapp-resource-type"></a>Тип ресурса Виндовсмикрософтеджеапп

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства и наследуемые свойства для приложения Microsoft EDGE в Windows.


Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсмикрософтеджеаппс](../api/intune-apps-windowsmicrosoftedgeapp-list.md)|Коллекция [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Список свойств и связей объектов [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|
|[Получение Виндовсмикрософтеджеапп](../api/intune-apps-windowsmicrosoftedgeapp-get.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Чтение свойств и связей объекта [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|
|[Создание Виндовсмикрософтеджеапп](../api/intune-apps-windowsmicrosoftedgeapp-create.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Создание нового объекта [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|
|[Удаление Виндовсмикрософтеджеапп](../api/intune-apps-windowsmicrosoftedgeapp-delete.md)|Нет|Удаляет объект [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md).|
|[Обновление Виндовсмикрософтеджеапп](../api/intune-apps-windowsmicrosoftedgeapp-update.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Обновление свойств объекта [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|

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
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|Состояние отправки. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|оптоволокон|[microsoftEdgeChannel](../resources/intune-apps-microsoftedgechannel.md)|Канал, который необходимо установить на целевые устройства. Возможные значения: `dev`, `beta`, `stable`.|
|дисплайлангуажелокале|String|Языковой стандарт, используемый при отображении текста для пользователя в пограничной приложении.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
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
  "@odata.type": "microsoft.graph.windowsMicrosoftEdgeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "String",
  "displayLanguageLocale": "String"
}
```



