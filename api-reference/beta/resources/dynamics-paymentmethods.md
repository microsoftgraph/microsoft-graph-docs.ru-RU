---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b30f97166625d45eba1a78342c219cbb74f42a8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013754"
---
# <a name="paymentmethods-resource-type"></a>Тип ресурса Пайментмесодс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Пайментмесодс](../api/dynamics-paymentmethods-get.md)      |пайментмесодс|Возвращает объект метода платежа.   |
|[POST Пайментмесодс](../api/dynamics-create-paymentmethods.md)  |пайментмесодс|Создает объект метода оплаты.|
|[Исправление Пайментмесодс](../api/dynamics-paymentmethods-update.md) |пайментмесодс|Обновляет объект метода оплаты.|
|[Удаление Пайментмесодс](../api/dynamics-paymentmethods-delete.md)|Нет          |Удаляет объект метода оплаты.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |Уникальный идентификатор Пайментмесодс. Не редактируемые.           |
|code                |string  |Указывает код метода оплаты.                           |
|displayName         |string  |Задает отображаемое имя метода оплаты.                   |
|lastModifiedDateTime|datetime|Дата и время последнего изменения метода оплаты. Только для чтения.|  


## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление объекта Пайментмесодс в формате JSON.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


