---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bde61142c5d8644ce12911249b17dd61b2c9c131
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201209"
---
# <a name="mobileapp-resource-type"></a>Тип ресурса mobileApp

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileApps](../api/intune-shared-mobileapp-list.md)|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Список свойств и связей объектов [mobileApp](../resources/intune-shared-mobileapp.md).|
|[Получение объекта mobileApp](../api/intune-shared-mobileapp-get.md)|[mobileApp](../resources/intune-shared-mobileapp.md)|Чтение свойств и связей объекта [mobileApp](../resources/intune-shared-mobileapp.md).|
|**Приложения**|
|[Действие assign](../api/intune-shared-mobileapp-assign.md)|Нет|Н/Д|
|[Функция getMobileAppCount](../api/intune-shared-mobileapp-getmobileappcount.md)|Int64|Пока не задокументировано.|
|[Функция getTopMobileApps](../api/intune-shared-mobileapp-gettopmobileapps.md)|Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)|Пока не задокументировано.|
|[действие Упдатерелатионшипс](../api/intune-shared-mobileapp-updaterelationships.md)|Нет|Н/Д|
|[Функция Жетрелатедаппстатес](../api/intune-shared-mobileapp-getrelatedappstates.md)|Коллекция Мобилеаппрелатионшипстате|Пока не задокументировано.|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-mobileapp-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Администратор предоставил или импортировал название приложения.|
|description|Строка|Описание приложения.|
|publisher|String.|Издатель приложения.|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Большой значок, отображается в сведениях о приложении и используется для отправки значка.|
|createdDateTime|DateTimeOffset|Дата и время создания приложения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения.|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором.|
|privacyInformationUrl|String.|URL-адрес заявления о конфиденциальности.|
|informationUrl|String.|URL-адрес с дополнительными сведениями.|
|owner|String|Владелец приложения.|
|developer|String.|Разработчик приложения.|
|notes|String|Заметки для приложения.|
|uploadState|Int32|Состояние отправки.|
|publishingState|мобилеапппублишингстате|Состояние публикации для приложения. Приложение не может быть назначено, если оно не опубликовано. Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе.|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого мобильного приложения.|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|**Приложения**|
|categories|Коллекция mobileAppCategory|Список категорий для этого приложения.|
|assignments|Коллекция mobileAppAssignment|Список назначений группы для этого мобильного приложения.|
|installSummary|mobileAppInstallSummary|Общие сведения по установке мобильного приложения.|
|deviceStatuses|Коллекция mobileAppInstallStatus|Список состояний установки для этого мобильного приложения.|
|userStatuses|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список состояний установки для этого мобильного приложения.|
|Таблица|Коллекция Мобилеаппрелатионшип|Список отношений для этого мобильного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "dependentAppCount": 1024
}
```



