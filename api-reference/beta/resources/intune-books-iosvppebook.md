---
title: Тип ресурса iosVppEBook
description: Класс, содержащий свойства электронной книги VPP для iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35a3f6cc1744b869b4dd2dc9e0baf703144ea73b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416778"
---
# <a name="iosvppebook-resource-type"></a>Тип ресурса iosVppEBook

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства электронной книги VPP для iOS.


Наследуется от [managedEBook](../resources/intune-books-managedebook.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosVppEBooks](../api/intune-books-iosvppebook-list.md)|Коллекция [iosVppEBook](../resources/intune-books-iosvppebook.md)|Список свойств и связей объектов [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Получение iosVppEBook](../api/intune-books-iosvppebook-get.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Считывание свойств и связей объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Создание iosVppEBook](../api/intune-books-iosvppebook-create.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Создание объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Удаление iosVppEBook](../api/intune-books-iosvppebook-delete.md)|None|Удаление экземпляра [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Обновление iosVppEBook](../api/intune-books-iosvppebook-update.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|displayName|String|Имя электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|description|String|Описание. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|publisher|String|Издатель. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|publishedDateTime|DateTimeOffset|Дата и время публикации электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Обложка книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|createdDateTime|DateTimeOffset|Дата и время создания электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения электронной книги. Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|vppTokenId|Guid|Идентификатор токена VPP.|
|appleId|String|Идентификатор Apple ID, связанный с токеном VPP.|
|vppOrganizationName|String|Название организации для токена VPP.|
|genres|Коллекция String|Жанры.|
|language|String|Язык.|
|seller|String|Продавец.|
|totalLicenseCount|Int32|Общее число лицензий.|
|usedLicenseCount|Int32|Число используемых лицензий.|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) коллекции|Список категорий для этой книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|assignments|Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|Список назначений для этой электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Сводка по установке мобильного приложения. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|deviceStates|Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Список состояний установки для этой электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|
|userStateSummary|Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Список состояний установки для этой электронной книги. Наследуется от [managedEBook](../resources/intune-books-managedebook.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```




