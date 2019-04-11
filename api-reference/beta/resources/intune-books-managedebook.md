---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 888df51e17ab45dcada3d69fad95315b26b4b20e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800401"
---
# <a name="managedebook-resource-type"></a>Тип ресурса managedEBook

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, содержащий базовые свойства управляемой электронной книги.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedEBook](../api/intune-books-managedebook-list.md)|Коллекция [managedEBook](../resources/intune-books-managedebook.md)|Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).|
|[Get managedEBook](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).|
|[Действие назначения](../api/intune-books-managedebook-assign.md)|Нет|Н/Д|

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
|Отношение|Тип|Описание|
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





