---
title: Тип ресурса Таксграупс
description: Объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 378d8c1d773eacb3339eba35d5d60cc7ef5f2400
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006607"
---
# <a name="taxgroups-resource-type"></a>Тип ресурса Таксграупс
Представляет тип ресурса Таксграупс в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Таксграупс](../api/dynamics-taxgroups-get.md)|Таксграупс|Получает объект налоговой группы.|
|[POST Таксграупс](../api/dynamics-create-taxgroups.md)|Таксграупс|Создает объект налоговой группы.|
|[Исправление Таксграупс](../api/dynamics-taxgroups-update.md)|Таксграупс|Обновляет объект налоговой группы.|
|[Удаление Таксграупс](../api/dynamics-taxgroups-delete.md)|none|Удаляет объект налоговой группы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Таксграуп. Только для чтения.|
|code|string|Указывает налоговую группу.|
|displayName|string|Задает отображаемое имя налоговой группы.|
|Такстипе|string|Указывает тип налога для группы.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения налоговой группы. Только для чтения.|  


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


