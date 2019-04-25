---
title: Тип ресурса Шипментмесодс
description: Метод отгрузки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 2f7ef9611fc85c13ac24c79b292e06a6bdc5d587
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543037"
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
|id|Глобальный уникальный идентификатор (GUID)|Уникальный идентификатор Шипментмесод. Не редактируемые.|
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


