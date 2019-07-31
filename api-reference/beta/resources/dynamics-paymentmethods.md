---
title: Тип ресурса Пайментмесодс
description: Объект метода оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 08cfc864ee670a799a5f1672fa96cf8167ef1423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006586"
---
# <a name="paymentmethods-resource-type"></a>Тип ресурса Пайментмесодс
Представляет способ оплаты в Dynamics 365 Business Central, например PayPal, кредитную карту и банковский счет.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип  |Описание             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Получение Пайментмесодс](../api/dynamics-paymentmethods-get.md)      |Пайментмесодс|Возвращает объект метода платежа.   |
|[POST Пайментмесодс](../api/dynamics-create-paymentmethods.md)  |Пайментмесодс|Создает объект метода оплаты.|
|[Исправление Пайментмесодс](../api/dynamics-paymentmethods-update.md) |Пайментмесодс|Обновляет объект метода оплаты.|
|[Удаление Пайментмесодс](../api/dynamics-paymentmethods-delete.md)|none          |Удаляет объект метода оплаты.|

## <a name="properties"></a>Свойства
| Свойство           | Тип   |Описание                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |Уникальный идентификатор Пайментмесодс. Не редактируемые.           |
|code                |string  |Указывает код метода оплаты.                           |
|displayName         |string  |Задает отображаемое имя метода оплаты.                   |
|lastModifiedDateTime|отличным|Дата и время последнего изменения метода оплаты. Только для чтения.|  


## <a name="relationships"></a>Отношения
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
