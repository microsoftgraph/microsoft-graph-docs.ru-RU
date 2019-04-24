---
title: Тип ресурса Каунтриесрегионс
description: Объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b6f50ba3046a402f2b8729529675653286808459
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507268"
---
# <a name="countriesregions-resource-type"></a>Тип ресурса Каунтриесрегионс
Представляет объект Каунтриесрегионс в Dynamics 365 Business Central, который является частью адреса.

## <a name="methods"></a>Методы

| Метод                                                              | Возвращаемый тип    |Описание                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[Получение Каунтриесрегионс](../api/dynamics-countriesregions-get.md)      |Каунтриесрегионс|Получение стран и регионов.   |
|[POST Каунтриесрегионс](../api/dynamics-create-countriesregions.md)  |Каунтриесрегионс|Создание стран и регионов.|
|[Исправление Каунтриесрегионс](../api/dynamics-countriesregions-update.md) |Каунтриесрегионс|Обновление стран и регионов.|
|[Удаление Каунтриесрегионс](../api/dynamics-countriesregions-delete.md)|Нет            |Удаление стран и регионов.|

## <a name="properties"></a>Свойства
| Свойство       | Тип       |Описание                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|id              |GUID        |Уникальный идентификатор страны или региона. Не редактируемые.           |
|code            |string      |Указывает код страны или региона.                    |
|displayName     |string      |Задает отображаемое имя страны или региона.            |
|Аддрессформат   |строка      |Указывает формат адреса, отображаемого в документах с внешними разворотами. Вы связываете формат адреса с кодом страны или региона, чтобы документы с внешними разворотами на основе карточек или документов с этим кодом страны или региона использовали указанный формат адреса.|
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


