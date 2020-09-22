---
title: Тип ресурса Таксграупс
description: Объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 373e4785d19a7983f890ee3c3574533323829954
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027043"
---
# <a name="taxgroups-resource-type"></a>Тип ресурса Таксграупс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип ресурса Таксграупс в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Таксграупс](../api/dynamics-taxgroups-get.md)|таксграупс|Получает объект налоговой группы.|
|[POST Таксграупс](../api/dynamics-create-taxgroups.md)|таксграупс|Создает объект налоговой группы.|
|[Исправление Таксграупс](../api/dynamics-taxgroups-update.md)|таксграупс|Обновляет объект налоговой группы.|
|[Удаление Таксграупс](../api/dynamics-taxgroups-delete.md)|Нет|Удаляет объект налоговой группы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Таксграуп. Только для чтения.|
|code|string|Указывает налоговую группу.|
|displayName|string|Задает отображаемое имя налоговой группы.|
|такстипе|string|Указывает тип налога для группы.|
|lastModifiedDateTime|datetime|Дата и время последнего изменения налоговой группы. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже показано представление объекта Таксграуп в формате JSON.

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```




