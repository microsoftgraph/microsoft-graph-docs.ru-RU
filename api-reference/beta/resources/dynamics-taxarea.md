---
title: Тип ресурса Таксареас
description: Налоговая область.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d2c4f007c23ae32fb79255a0a8f1509589740a70
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503434"
---
# <a name="taxareas-resource-type"></a>Тип ресурса Таксареас

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип ресурса "налоговая область" в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Таксареас](../api/dynamics-taxarea-get.md)|таксареас|Получает объект налоговой области.|
|[POST Таксареас](../api/dynamics-create-taxarea.md)|таксареас|Создает объект налоговой области.|
|[Исправление Таксареас](../api/dynamics-taxarea-update.md)|таксареас|Обновляет объект налоговой области.|
|[Удаление Таксареас](../api/dynamics-taxarea-delete.md)|нет|Удаляет объект налоговой области.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор налоговой области. Не редактируемые.|
|code|Строка, максимальный размер 20| Код налоговой области.|
|displayName|Строка, максимальный размер 50| Отображаемое имя налоговой области.|
|такстипе|строка|Тип налога для налоговой области.|
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


