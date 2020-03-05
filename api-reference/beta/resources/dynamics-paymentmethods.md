---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d72ac6ec655e15ad6f3c824dc2d5e9c3e09db0c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503651"
---
# <a name="paymentmethods-resource-type"></a>Тип ресурса Пайментмесодс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Пайментмесодс](../api/dynamics-paymentmethods-get.md)      |пайментмесодс|Возвращает объект метода платежа.   |
|[POST Пайментмесодс](../api/dynamics-create-paymentmethods.md)  |пайментмесодс|Создает объект метода оплаты.|
|[Исправление Пайментмесодс](../api/dynamics-paymentmethods-update.md) |пайментмесодс|Обновляет объект метода оплаты.|
|[Удаление Пайментмесодс](../api/dynamics-paymentmethods-delete.md)|нет          |Удаляет объект метода оплаты.|

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
