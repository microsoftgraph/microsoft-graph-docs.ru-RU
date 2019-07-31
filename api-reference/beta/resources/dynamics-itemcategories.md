---
title: Тип ресурса Итемкатегориес
description: Категория элемента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 18017c580637bb53a70b5f7a331ff7be1dc7a07c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972924"
---
# <a name="itemcategories-resource-type"></a>Тип ресурса Итемкатегориес
Представляет категорию для ряда элементов в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Итемкатегориес](../api/dynamics-itemcategories-get.md)      |Итемкатегориес|Получение категории элемента.   |
|[POST Итемкатегориес](../api/dynamics-create-itemcategories.md)  |Итемкатегориес|Создайте категорию элемента.|
|[Исправление Итемкатегориес](../api/dynamics-itemcategories-update.md) |Итемкатегориес|Обновление категории элемента.|
|[Удаление Итемкатегориес](../api/dynamics-itemcategories-delete.md)|none          |Удаление категории элемента.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |GUID    |Уникальный идентификатор Итемкатегори. Не редактируемые.|
|code                |string  |Код Итемкатегори.                          |
|displayName         |string  |Отображаемое имя Итемкатегориес.                |
|lastModifiedDateTime|отличным|Дата и время последнего изменения Итемкатегори. Только для чтения.|  


## <a name="relationships"></a>Отношения
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

