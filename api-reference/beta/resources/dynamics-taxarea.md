---
title: Тип ресурса Таксареас
description: Налоговая область.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507233"
---
# <a name="taxareas-resource-type"></a>Тип ресурса Таксареас
Представляет тип ресурса "налоговая область" в Dynamics 365 Business Central.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение Таксареас](../api/dynamics-taxarea-get.md)|Таксареас|Получает объект налоговой области.|
|[POST Таксареас](../api/dynamics-create-taxarea.md)|Таксареас|Создает объект налоговой области.|
|[Исправление Таксареас](../api/dynamics-taxarea-update.md)|Таксареас|Обновляет объект налоговой области.|
|[Удаление Таксареас](../api/dynamics-taxarea-delete.md)|Нет|Удаляет объект налоговой области.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|GUID|Уникальный идентификатор налоговой области. Не редактируемые.|
|code|Строка, максимальный размер 20| Код налоговой области.|
|displayName|Строка, максимальный размер 50| Отображаемое имя налоговой области.|
|Такстипе|строка|Тип налога для налоговой области.|
|lastModifiedDateTime|отличным|Дата и время последнего изменения налоговой области. Только для чтения.|

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


