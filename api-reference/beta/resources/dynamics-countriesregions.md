---
title: Тип ресурса Каунтриесрегионс
description: Объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 490fa240cda525b517bf4e8dcec3e89aedbcc201
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049815"
---
# <a name="countriesregions-resource-type"></a>Тип ресурса Каунтриесрегионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет объект Каунтриесрегионс в Dynamics 365 Business Central, который является частью адреса.

## <a name="methods"></a>Методы

| Метод                                                              | Возвращаемый тип    |Описание                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[Получение Каунтриесрегионс](../api/dynamics-countriesregions-get.md)      |каунтриесрегионс|Получение стран и регионов.   |
|[POST Каунтриесрегионс](../api/dynamics-create-countriesregions.md)  |каунтриесрегионс|Создание стран и регионов.|
|[Исправление Каунтриесрегионс](../api/dynamics-countriesregions-update.md) |каунтриесрегионс|Обновление стран и регионов.|
|[Удаление Каунтриесрегионс](../api/dynamics-countriesregions-delete.md)|Нет            |Удаление стран и регионов.|

## <a name="properties"></a>Свойства
| Свойство       | Тип       |Описание                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|id              |GUID        |Уникальный идентификатор страны или региона. Не редактируемые.           |
|code            |string      |Указывает код страны или региона.                    |
|displayName     |string      |Задает отображаемое имя страны или региона.            |
|аддрессформат   |string      |Указывает формат адреса, отображаемого в документах с внешними разворотами. Вы связываете формат адреса с кодом страны или региона, чтобы документы с внешними разворотами на основе карточек или документов с этим кодом страны или региона использовали указанный формат адреса.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения страны или региона. Только для чтения.|  


## <a name="relationships"></a>Связи
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




