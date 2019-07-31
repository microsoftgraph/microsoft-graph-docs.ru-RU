---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e8d25294b219815c8aa569c7a8c7fab7ec68830c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006614"
---
# <a name="shipmentmethods-resource-type"></a>Тип ресурса Шипментмесодс
Представляет способ отгрузки в Dynamics 365 Business Central, таких как UPS, Федекс и DHL.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Шипментмесодс](../api/dynamics-shipmentmethods-get.md)|Шипментмесодс|Получает метод отгрузки.|
|[POST Шипментмесодс](../api/dynamics-create-shipmentmethods.md)|Шипментмесодс|Создает метод отгрузки.|
|[Исправление Шипментмесодс](../api/dynamics-shipmentmethods-update.md)|Шипментмесодс|Обновляет метод отгрузки.|
|[Удаление Шипментмесодс](../api/dynamics-shipmentmethods-delete.md)|none|Удаляет метод отгрузки.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Шипментмесод. Не редактируемые.|
|code|string|Указывает код метода отгрузки.|
|displayName|string|Задает отображаемое имя метода отгрузки.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения метода отгрузки. Только для чтения.|  


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


