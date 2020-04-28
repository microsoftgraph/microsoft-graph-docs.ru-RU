---
title: Тип ресурса Таксграупс
description: Объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3c8f244b9c3601aaeb315b09bb51d21275a63f6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503259"
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


## <a name="relationships"></a>Связи
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


