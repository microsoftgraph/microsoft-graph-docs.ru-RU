---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365502"
---
# <a name="shipmentmethods-resource-type"></a>Тип ресурса Шипментмесодс
Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Шипментмесодс](../api/dynamics-shipmentmethods-get.md)|Шипментмесодс|Получает метод отгрузки.|
|[POST Шипментмесодс](../api/dynamics-create-shipmentmethods.md)|Шипментмесодс|Создает метод отгрузки.|
|[Исправление Шипментмесодс](../api/dynamics-shipmentmethods-update.md)|Шипментмесодс|Обновляет метод отгрузки.|
|[Удаление Шипментмесодс](../api/dynamics-shipmentmethods-delete.md)|Нет|Удаляет метод отгрузки.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Шипментмесод. Не редактируемые.|
|code|строка|Указывает код метода отгрузки.|
|displayName|строка|Задает отображаемое имя метода отгрузки.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения метода отгрузки. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление объекта Шипментмесод в формате JSON.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


