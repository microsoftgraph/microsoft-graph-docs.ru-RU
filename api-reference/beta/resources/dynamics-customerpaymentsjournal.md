---
title: Тип ресурса Кустомерпайментжаурналс
description: Журнал платежей клиентов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a6fc1cf1541ebfbcf514de3005c7a89961531568
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071362"
---
# <a name="customerpaymentsjournals-resource-type"></a>Тип ресурса Кустомерпайментсжаурналс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет журнал платежей клиента в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод               | Возвращаемый тип             |Описание                      |
|:---------------------|:------------------------|:--------------------------------|
|[Получение Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-get.md)      |кустомерпайментжаурналс|Возвращает журнал платежей клиента.   |
|[POST Кустомерпайментжаурналс](../api/dynamics-create-customerpaymentsjournal.md)  |кустомерпайментжаурналс|Создает журнал платежей клиента.|
|[Исправление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-update.md) |кустомерпайментжаурналс|Обновляет журнал платежей клиента.|
|[Удаление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-delete.md)|Нет                     |Удаляет журнал платежей клиента.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор журнала платежей клиента. Не редактируемые.           |
|code                |Строка, максимальный размер 10| Код журнала платежей клиента.                             |
|displayName         |Строка, максимальный размер 50| Отображаемое имя журнала платежей клиента.                     |
|lastModifiedDateTime|datetime               |Дата и время последнего изменения журнала платежей клиента. Только для чтения.|

## <a name="relationships"></a>Связи

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```



