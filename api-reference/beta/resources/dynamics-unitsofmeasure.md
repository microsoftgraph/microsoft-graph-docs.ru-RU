---
title: Тип ресурса Унитсофмеасуре
description: Объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 97fb9fd7f36042a2ff056570e5e05330ff2e60a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021947"
---
# <a name="unitsofmeasure-resource-type"></a>Тип ресурса Унитсофмеасуре

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет единицу измерения, которая является стандартом измерения количества в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Унитсофмеасуре](../api/dynamics-unitsofmeasure-get.md)|унитсофмеасуре|Возвращает объект единицы измерения.|
|[POST Унитсофмеасуре](../api/dynamics-create-unitsofmeasure.md)|унитсофмеасуре|Создает объект единицы измерения.|
|[Исправление Унитсофмеасуре](../api/dynamics-unitsofmeasure-update.md)|унитсофмеасуре|Обновляет объект единицы измерения.|
|[Удаление Унитсофмеасуре](../api/dynamics-unitsofmeasure-delete.md)|Нет|Удаляет объект единицы измерения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Унитсофмеасуре. Не редактируемые.|
|code|string|Задает код для единицы измерения.|
|displayName|string|Задает отображаемое имя единицы измерения.|
|интернатионалстандардкоде|string|Указывает код единицы измерения, выраженный в соответствии с УНЕЦЕ Rec20 Standard в связи с электронной отправкой документов продажи.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения единицы измерения. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса **унитсофмеасуре** в формате JSON.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```


