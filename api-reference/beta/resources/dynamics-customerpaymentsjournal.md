---
title: Тип ресурса Кустомерпайментжаурналс
description: Журнал платежей клиентов в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9b909676a3cce34ac15481e9ce05746e972d7f8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504582"
---
# <a name="customerpaymentsjournals-resource-type"></a>Тип ресурса Кустомерпайментсжаурналс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет журнал платежей клиента в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод               | Возвращаемый тип             |Описание                      |
|:---------------------|:------------------------|:--------------------------------|
|[Получение Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-get.md)      |кустомерпайментжаурналс|Возвращает журнал платежей клиента.   |
|[POST Кустомерпайментжаурналс](../api/dynamics-create-customerpaymentsjournal.md)  |кустомерпайментжаурналс|Создает журнал платежей клиента.|
|[Исправление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-update.md) |кустомерпайментжаурналс|Обновляет журнал платежей клиента.|
|[Удаление Кустомерпайментжаурналс](../api/dynamics-customerpaymentsjournal-delete.md)|нет                     |Удаляет журнал платежей клиента.|

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

