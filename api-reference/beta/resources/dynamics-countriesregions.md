---
title: Тип ресурса Каунтриесрегионс
description: Объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 73f60a48e1b7b3564851271209e195ecbbf171e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012634"
---
# <a name="countriesregions-resource-type"></a>Тип ресурса Каунтриесрегионс
Представляет объект Каунтриесрегионс в Dynamics 365 Business Central, который является частью адреса.

## <a name="methods"></a>Методы

| Метод                                                              | Возвращаемый тип    |Описание                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[Получение Каунтриесрегионс](../api/dynamics-countriesregions-get.md)      |Каунтриесрегионс|Получение стран и регионов.   |
|[POST Каунтриесрегионс](../api/dynamics-create-countriesregions.md)  |Каунтриесрегионс|Создание стран и регионов.|
|[Исправление Каунтриесрегионс](../api/dynamics-countriesregions-update.md) |Каунтриесрегионс|Обновление стран и регионов.|
|[Удаление Каунтриесрегионс](../api/dynamics-countriesregions-delete.md)|none            |Удаление стран и регионов.|

## <a name="properties"></a>Свойства
| Свойство       | Тип       |Описание                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|id              |GUID        |Уникальный идентификатор страны или региона. Не редактируемые.           |
|code            |string      |Указывает код страны или региона.                    |
|displayName     |string      |Задает отображаемое имя страны или региона.            |
|Аддрессформат   |string      |Указывает формат адреса, отображаемого в документах с внешними разворотами. Вы связываете формат адреса с кодом страны или региона, чтобы документы с внешними разворотами на основе карточек или документов с этим кодом страны или региона использовали указанный формат адреса.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения страны или региона. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление объекта Каунтриесрегионс в формате JSON.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


