---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea4fc7a46c111f01751a232e7475ce3bc055eb21
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123218"
---
# <a name="mobileapp-resource-type"></a>Тип ресурса mobileApp

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileApps](../api/intune-apps-mobileapp-list.md)|Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)|Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).|
|[Получение объекта mobileApp](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).|
|[assign action](../api/intune-apps-mobileapp-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Администратор предоставил или импортировал название приложения.|
|description|String|Описание приложения.|
|publisher|String|Издатель приложения.|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Большой значок, отображается в сведениях о приложении и используется для отправки значка.|
|createdDateTime|DateTimeOffset|Дата и время создания приложения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения.|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором.|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности.|
|informationUrl|String|URL-адрес с дополнительными сведениями.|
|owner|String|Владелец приложения.|
|developer|String|Разработчик приложения.|
|notes|String|Заметки для приложения.|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение не может быть назначено, если оно не опубликовано. Возможные значения: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения.|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения.|

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
  "publishingState": "String"
}
```




