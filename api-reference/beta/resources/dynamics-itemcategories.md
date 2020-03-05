---
title: Тип ресурса Итемкатегориес
description: Категория элемента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d0a751fe076c76fcb703c4d910ac35d3d0593b15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503847"
---
# <a name="itemcategories-resource-type"></a>Тип ресурса Итемкатегориес

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет категорию для ряда элементов в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Итемкатегориес](../api/dynamics-itemcategories-get.md)      |итемкатегориес|Получение категории элемента.   |
|[POST Итемкатегориес](../api/dynamics-create-itemcategories.md)  |итемкатегориес|Создайте категорию элемента.|
|[Исправление Итемкатегориес](../api/dynamics-itemcategories-update.md) |итемкатегориес|Обновление категории элемента.|
|[Удаление Итемкатегориес](../api/dynamics-itemcategories-delete.md)|нет          |Удаление категории элемента.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |GUID    |Уникальный идентификатор Итемкатегори. Не редактируемые.|
|code                |string  |Код Итемкатегори.                          |
|displayName         |string  |Отображаемое имя Итемкатегориес.                |
|lastModifiedDateTime|datetime|Дата и время последнего изменения Итемкатегори. Только для чтения.|  


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление объекта Итемкатегориес в формате JSON.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

