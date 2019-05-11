---
title: Тип ресурса Манажедебуккатегори
description: Содержит свойства для одной категории электронной книги Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0baa3dbbecd90483eeb182edf486fcd6bfdd846b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949320"
---
# <a name="managedebookcategory-resource-type"></a>Тип ресурса Манажедебуккатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для одной категории электронной книги Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажедебуккатегориес](../api/intune-books-managedebookcategory-list.md)|Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)|Список свойств и связей объектов [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|
|[Получение Манажедебуккатегори](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Чтение свойств и связей объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|
|[Создание Манажедебуккатегори](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Создание нового объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|
|[Удаление Манажедебуккатегори](../api/intune-books-managedebookcategory-delete.md)|Нет|Удаляет объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).|
|[Обновление Манажедебуккатегори](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|Строка|Имя категории электронной книги.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения Манажедебуккатегори.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




