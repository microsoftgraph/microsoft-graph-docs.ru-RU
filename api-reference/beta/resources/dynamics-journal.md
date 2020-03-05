---
title: Тип ресурса "журнал"
description: Журнал в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 041de72a3372fd80063b96ba73d10272247c4fdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503749"
---
# <a name="journal-resource-type"></a>Тип ресурса "журнал"

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет журнал в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                            |Возвращаемый тип|Описание    |
|:--------------------------------------------------|:----------|:--------------|
|[Получение журнала](../api/dynamics-journal-get.md)      |Фин    |Получает журнал.   |
|[Разноска журнала](../api/dynamics-create-journal.md)  |Фин    |Создает журнал.|
|[Журнал исправлений](../api/dynamics-journal-update.md) |Фин    |Обновляет журнал.|
|[Удаление журнала](../api/dynamics-journal-delete.md)|нет       |Удаляет журнал.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор журнала. Не редактируемые.           |
|code                |Строка, максимальный размер 10| Код журнала.                             |
|displayName         |Строка, максимальный размер 50| Отображаемое имя журнала.                     |
|lastModifiedDateTime|datetime               |Дата и время последнего изменения, внесенные в журнал. Только для чтения.|

## <a name="bound-actions"></a>Связанные действия
Тип ресурса журнал предоставляет связанное действие `post` , которое отправляет соответствующий раздел общего журнала.

Учет раздела общего журнала показано в следующем примере:  
`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.

Ответ не имеет контента; код ответа — 204.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

