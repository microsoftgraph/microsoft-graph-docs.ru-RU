---
title: Тип ресурса Унитсофмеасуре
description: Объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 870e188939646594b62e6eebf3e234eb0211f140
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365754"
---
# <a name="unitsofmeasure-resource-type"></a>Тип ресурса Унитсофмеасуре
Представляет единицу измерения, которая является стандартом измерения количества в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Унитсофмеасуре](../api/dynamics-unitsofmeasure-get.md)|Унитсофмеасуре|Возвращает объект единицы измерения.|
|[POST Унитсофмеасуре](../api/dynamics-create-unitsofmeasure.md)|Унитсофмеасуре|Создает объект единицы измерения.|
|[Исправление Унитсофмеасуре](../api/dynamics-unitsofmeasure-update.md)|Унитсофмеасуре|Обновляет объект единицы измерения.|
|[Удаление Унитсофмеасуре](../api/dynamics-unitsofmeasure-delete.md)|Нет|Удаляет объект единицы измерения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Унитсофмеасуре. Не редактируемые.|
|code|строка|Задает код для единицы измерения.|
|displayName|строка|Задает отображаемое имя единицы измерения.|
|Интернатионалстандардкоде|строка|Указывает код единицы измерения, выраженный в соответствии с УНЕЦЕ Rec20 Standard в связи с электронной отправкой документов продажи.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения единицы измерения. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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
