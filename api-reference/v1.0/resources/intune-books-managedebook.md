---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 42d14dbd1c2afa6eb316bcb46cf3fe76bd0669e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028814"
---
# <a name="managedebook-resource-type"></a>Тип ресурса managedEBook

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, содержащий базовые свойства управляемой электронной книги.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedEBooks](../api/intune-books-managedebook-list.md)|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).|
|[Получение объекта managedEBook](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).|
|[действие назначения](../api/intune-books-managedebook-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Имя электронной книги.|
|description|String|Описание.|
|publisher|String|Издатель.|
|publishedDateTime|DateTimeOffset|Дата и время публикации электронной книги.|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Обложка книги.|
|createdDateTime|DateTimeOffset|Дата и время создания электронной книги.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения электронной книги.|
|informationUrl|String|URL-адрес с дополнительными сведениями.|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Список назначений для этой электронной книги.|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Общие сведения по установке мобильного приложения.|
|deviceStates|Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Список состояний установки для этой электронной книги.|
|userStateSummary|Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Список состояний установки для этой электронной книги.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



