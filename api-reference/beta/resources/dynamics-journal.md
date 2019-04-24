---
title: Тип ресурса "журнал"
description: Журнал в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bef5008bbacb1729f48758b228e55a3f6adc2af0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507303"
---
# <a name="journal-resource-type"></a>Тип ресурса "журнал"
Представляет журнал в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                            |Возвращаемый тип|Описание    |
|:--------------------------------------------------|:----------|:--------------|
|[Получение журнала](../api/dynamics-journal-get.md)      |Фин    |Получает журнал.   |
|[Разноска журнала](../api/dynamics-create-journal.md)  |Фин    |Создает журнал.|
|[Журнал исправлений](../api/dynamics-journal-update.md) |Фин    |Обновляет журнал.|
|[Удаление журнала](../api/dynamics-journal-delete.md)|Нет       |Удаляет журнал.|

## <a name="properties"></a>Свойства
| Свойство           | Тип                  |Описание                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|id                  |GUID                   |Уникальный идентификатор журнала. Не редактируемые.           |
|code                |Строка, максимальный размер 10| Код журнала.                             |
|displayName         |Строка, максимальный размер 50| Отображаемое имя журнала.                     |
|lastModifiedDateTime|отличным               |Дата и время последнего изменения, внесенные в журнал. Только для чтения.|

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

