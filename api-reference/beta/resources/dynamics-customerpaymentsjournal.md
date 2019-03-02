---
title: Тип ресурса Кустомерпайментжаурналс
description: Журнал платежей клиентов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365740"
---
# <a name="customerpaymentsjournals-resource-type"></a>Тип ресурса Кустомерпайментсжаурналс
Представляет журнал платежей клиента в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод               | Возвращаемый тип             |Описание                      |
|:---------------------|:------------------------|:--------------------------------|
|[Получение Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-get.md)      |Кустомерпайментжаурналс|Возвращает журнал платежей клиента.   |
|[POST Кустомерпайментжаурналс](../api/dynamics-create-customerpaymentsjournal.md)  |Кустомерпайментжаурналс|Создает журнал платежей клиента.|
|[Исправление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-update.md) |Кустомерпайментжаурналс|Обновляет журнал платежей клиента.|
|[Удаление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-delete.md)|Нет                     |Удаляет журнал платежей клиента.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор журнала платежей клиента. Не редактируемые.           |
|code                |Строка, максимальный размер 10| Код журнала платежей клиента.                             |
|displayName         |Строка, максимальный размер 50| Отображаемое имя журнала платежей клиента.                     |
|lastModifiedDateTime|отличным               |Дата и время последнего изменения журнала платежей клиента. Только для чтения.|

## <a name="relationships"></a>Отношения

## <a name="json-representation"></a>Описание в формате JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

