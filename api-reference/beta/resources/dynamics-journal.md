---
title: Тип ресурса "журнал"
description: Журнал в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7cfc723a4370c2b30440dcd4e33b50ed066ac89b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006594"
---
# <a name="journal-resource-type"></a>Тип ресурса "журнал"
Представляет журнал в Dynamics 365 Business Central.

## <a name="methods"></a>Методы

| Метод                                            |Возвращаемый тип|Описание    |
|:--------------------------------------------------|:----------|:--------------|
|[Получение журнала](../api/dynamics-journal-get.md)      |Фин    |Получает журнал.   |
|[Разноска журнала](../api/dynamics-create-journal.md)  |Фин    |Создает журнал.|
|[Журнал исправлений](../api/dynamics-journal-update.md) |Фин    |Обновляет журнал.|
|[Удаление журнала](../api/dynamics-journal-delete.md)|none       |Удаляет журнал.|

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

