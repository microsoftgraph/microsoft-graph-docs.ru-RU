---
title: Тип ресурса Таксграупс
description: Объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366692"
---
# <a name="taxgroups-resource-type"></a>Тип ресурса Таксграупс
Представляет тип ресурса Таксграупс в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Таксграупс](../api/dynamics-taxgroups-get.md)|Таксграупс|Получает объект налоговой группы.|
|[POST Таксграупс](../api/dynamics-create-taxgroups.md)|Таксграупс|Создает объект налоговой группы.|
|[Исправление Таксграупс](../api/dynamics-taxgroups-update.md)|Таксграупс|Обновляет объект налоговой группы.|
|[Удаление Таксграупс](../api/dynamics-taxgroups-delete.md)|Нет|Удаляет объект налоговой группы.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор Таксграуп. Только для чтения.|
|code|строка|Указывает налоговую группу.|
|displayName|строка|Задает отображаемое имя налоговой группы.|
|Такстипе|строка|Указывает тип налога для группы.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения налоговой группы. Только для чтения.|  


## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Описание в формате JSON

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


