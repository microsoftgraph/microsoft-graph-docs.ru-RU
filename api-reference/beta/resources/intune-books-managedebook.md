---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcec7c8dfaa0461e6b88d67a5a0f73373a1af7b0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797369"
---
# <a name="managedebook-resource-type"></a>Тип ресурса managedEBook

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)|Список категорий для этой электронной книги.|
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



