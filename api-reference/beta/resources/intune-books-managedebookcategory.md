---
title: Тип ресурса Манажедебуккатегори
description: Содержит свойства для одной категории электронной книги Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4bc2662af33af2f42eaeec0e4dae6d6f519549b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694027"
---
# <a name="managedebookcategory-resource-type"></a>Тип ресурса Манажедебуккатегори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Ключ объекта.|
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





