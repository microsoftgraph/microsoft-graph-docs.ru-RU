---
title: Тип ресурса microsoftStoreForBusinessApp
description: Приложения из Microsoft Store для бизнеса. Этот класс не поддерживает операции создания, удаления и обновления.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ed75d27035011245757a750e9bddf971d9bf435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094486"
---
# <a name="microsoftstoreforbusinessapp-resource-type"></a>Тип ресурса microsoftStoreForBusinessApp

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Приложения из Microsoft Store для бизнеса. Этот класс не поддерживает операции создания, удаления и обновления.


Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление microsoftStoreForBusinessApps](../api/intune-apps-microsoftstoreforbusinessapp-list.md)|Коллекция [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|Список свойств и связей объектов [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Получение microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-get.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|Считывание свойств и связей объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Создание microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-create.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Удаление microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-delete.md)|None|Удаление экземпляра [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|
|[Обновление microsoftStoreForBusinessApp](../api/intune-apps-microsoftstoreforbusinessapp-update.md)|[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)|Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
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
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|usedLicenseCount|Int32|Количество используемых лицензий на Microsoft Store для бизнеса.|
|totalLicenseCount|Int32|Общее количество лицензий на Microsoft Store для бизнеса.|
|productKey|String|Ключ продукта для приложения.|
|licenseType|[микрософтсторефорбусинесслиценсетипе](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|Тип лицензии приложения. Возможные значения: `offline`, `online`.|
|packageIdentityName|String|Идентификатор пакета приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "publishingState": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String"
}
```









