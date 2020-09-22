---
title: Тип ресурса Таксареас
description: Налоговая область.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 140470f0e293b41770779628280f0117d8bb6a89
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027057"
---
# <a name="taxareas-resource-type"></a>Тип ресурса Таксареас

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип ресурса "налоговая область" в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Таксареас](../api/dynamics-taxarea-get.md)|таксареас|Получает объект налоговой области.|
|[POST Таксареас](../api/dynamics-create-taxarea.md)|таксареас|Создает объект налоговой области.|
|[Исправление Таксареас](../api/dynamics-taxarea-update.md)|таксареас|Обновляет объект налоговой области.|
|[Удаление Таксареас](../api/dynamics-taxarea-delete.md)|Нет|Удаляет объект налоговой области.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор налоговой области. Не редактируемые.|
|code|Строка, максимальный размер 20| Код налоговой области.|
|displayName|Строка, максимальный размер 50| Отображаемое имя налоговой области.|
|такстипе|string|Тип налога для налоговой области.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения налоговой области. Только для чтения.|

## <a name="relationships"></a>Связи

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```




