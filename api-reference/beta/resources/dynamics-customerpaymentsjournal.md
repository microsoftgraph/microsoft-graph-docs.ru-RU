---
title: Тип ресурса Кустомерпайментжаурналс
description: Журнал платежей клиентов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0791fe2b8c36bdff535f7fc56dea54abe1632647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973634"
---
# <a name="customerpaymentsjournals-resource-type"></a>Тип ресурса Кустомерпайментсжаурналс
Представляет журнал платежей клиента в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод               | Возвращаемый тип             |Описание                      |
|:---------------------|:------------------------|:--------------------------------|
|[Получение Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-get.md)      |Кустомерпайментжаурналс|Возвращает журнал платежей клиента.   |
|[POST Кустомерпайментжаурналс](../api/dynamics-create-customerpaymentsjournal.md)  |Кустомерпайментжаурналс|Создает журнал платежей клиента.|
|[Исправление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-update.md) |Кустомерпайментжаурналс|Обновляет журнал платежей клиента.|
|[Удаление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-delete.md)|none                     |Удаляет журнал платежей клиента.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор журнала платежей клиента. Не редактируемые.           |
|code                |Строка, максимальный размер 10| Код журнала платежей клиента.                             |
|displayName         |Строка, максимальный размер 50| Отображаемое имя журнала платежей клиента.                     |
|lastModifiedDateTime|отличным               |Дата и время последнего изменения журнала платежей клиента. Только для чтения.|

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

