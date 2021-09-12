---
title: Тип ресурса iosVppEBook
description: Класс, содержащий свойства электронной книги VPP для iOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 256fe5ce3648de9e86d68eaa5d24741178fcb76a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007196"
---
# <a name="iosvppebook-resource-type"></a>Тип ресурса iosVppEBook

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Ключ объекта. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|displayName|Строка|Имя электронной книги. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|description|Строка|Описание. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|publisher|String|Издатель. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|publishedDateTime|DateTimeOffset|Дата и время публикации электронной книги. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Обложка книги. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|createdDateTime|DateTimeOffset|Дата и время создания электронной книги. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения электронной книги. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).|
|vppTokenId|Guid|Идентификатор токена VPP.|
|appleId|String|Идентификатор Apple ID, связанный с токеном VPP.|
|vppOrganizationName|String|Название организации для токена VPP.|
|genres|Коллекция String|Жанры.|
|language|String|Язык.|
|seller|String|Продавец.|
|totalLicenseCount|Int32|Общее число лицензий.|
|usedLicenseCount|Int32|Число используемых лицензий.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
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
  "usedLicenseCount": 1024
}
```




