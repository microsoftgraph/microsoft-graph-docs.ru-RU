---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366650"
---
# <a name="paymentmethods-resource-type"></a>Тип ресурса Пайментмесодс
Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Пайментмесодс](../api/dynamics-paymentmethods-get.md)      |Пайментмесодс|Возвращает объект метода платежа.   |
|[POST Пайментмесодс](../api/dynamics-create-paymentmethods.md)  |Пайментмесодс|Создает объект метода оплаты.|
|[Исправление Пайментмесодс](../api/dynamics-paymentmethods-update.md) |Пайментмесодс|Обновляет объект метода оплаты.|
|[Удаление Пайментмесодс](../api/dynamics-paymentmethods-delete.md)|Нет          |Удаляет объект метода оплаты.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |Уникальный идентификатор Пайментмесодс. Не редактируемые.           |
|code                |строка  |Указывает код метода оплаты.                           |
|displayName         |строка  |Задает отображаемое имя метода оплаты.                   |
|lastModifiedDateTime|отличным|Дата и время последнего изменения метода оплаты. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление объекта Пайментмесодс в формате JSON.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
