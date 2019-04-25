---
title: Тип ресурса Итемкатегориес
description: Категория элемента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e18319683f6dbceddccc9cf83e48cd3ef89f895d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543058"
---
# <a name="itemcategories-resource-type"></a>Тип ресурса Итемкатегориес
Представляет категорию для ряда элементов в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Итемкатегориес](../api/dynamics-itemcategories-get.md)      |Итемкатегориес|Получение категории элемента.   |
|[POST Итемкатегориес](../api/dynamics-create-itemcategories.md)  |Итемкатегориес|Создайте категорию элемента.|
|[Исправление Итемкатегориес](../api/dynamics-itemcategories-update.md) |Итемкатегориес|Обновление категории элемента.|
|[Удаление Итемкатегориес](../api/dynamics-itemcategories-delete.md)|Нет          |Удаление категории элемента.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |Глобальный уникальный идентификатор (GUID)    |Уникальный идентификатор Итемкатегори. Не редактируемые.|
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

