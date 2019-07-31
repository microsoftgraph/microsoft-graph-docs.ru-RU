---
title: Тип ресурса Унитсофмеасуре
description: Объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3658c4c510194d3cc950094ec9e46db31589bc03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972868"
---
# <a name="unitsofmeasure-resource-type"></a>Тип ресурса Унитсофмеасуре
Представляет единицу измерения, которая является стандартом измерения количества в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Унитсофмеасуре](../api/dynamics-unitsofmeasure-get.md)|Унитсофмеасуре|Возвращает объект единицы измерения.|
|[POST Унитсофмеасуре](../api/dynamics-create-unitsofmeasure.md)|Унитсофмеасуре|Создает объект единицы измерения.|
|[Исправление Унитсофмеасуре](../api/dynamics-unitsofmeasure-update.md)|Унитсофмеасуре|Обновляет объект единицы измерения.|
|[Удаление Унитсофмеасуре](../api/dynamics-unitsofmeasure-delete.md)|none|Удаляет объект единицы измерения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Унитсофмеасуре. Не редактируемые.|
|code|string|Задает код для единицы измерения.|
|displayName|string|Задает отображаемое имя единицы измерения.|
|Интернатионалстандардкоде|string|Указывает код единицы измерения, выраженный в соответствии с УНЕЦЕ Rec20 Standard в связи с электронной отправкой документов продажи.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения единицы измерения. Только для чтения.|  


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
