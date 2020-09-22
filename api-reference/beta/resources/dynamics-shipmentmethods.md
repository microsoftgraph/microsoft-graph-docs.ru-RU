---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d45153a08572f32f29128fd4d3f51638d71c951b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027071"
---
# <a name="shipmentmethods-resource-type"></a>Тип ресурса Шипментмесодс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Шипментмесодс](../api/dynamics-shipmentmethods-get.md)|шипментмесодс|Получает метод отгрузки.|
|[POST Шипментмесодс](../api/dynamics-create-shipmentmethods.md)|шипментмесодс|Создает метод отгрузки.|
|[Исправление Шипментмесодс](../api/dynamics-shipmentmethods-update.md)|шипментмесодс|Обновляет метод отгрузки.|
|[Удаление Шипментмесодс](../api/dynamics-shipmentmethods-delete.md)|Нет|Удаляет метод отгрузки.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Шипментмесод. Не редактируемые.|
|code|string|Указывает код метода отгрузки.|
|displayName|string|Задает отображаемое имя метода отгрузки.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения метода отгрузки. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление объекта Шипментмесод в формате JSON.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```




