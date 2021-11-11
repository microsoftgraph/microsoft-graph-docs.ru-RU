---
title: тип ресурсов компаний
description: Компания в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 8230e7aca8b222c54656845c0e52d4fc60bc7abd
ms.sourcegitcommit: 6b5bee1a1cea92c1f3d6439110c4916eb8b249a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2021
ms.locfileid: "60908577"
---
# <a name="companies-resource-type"></a>тип ресурсов компаний

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тип ресурсов компаний в Dynamics 365 Business Central. 

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип  |Описание|
|:---------------|:-------------|:----------|
|[Получение компаний](../api/dynamics-companies-get.md)|companies|Получите компанию.|

## <a name="properties"></a>Свойства
| Свойство        | Тип |Описание                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |Уникальный ID компании. Только для чтения.|
|name             |string|Указывает компанию.                  |
|displayName      |string|Указывает имя отображения компании.     |
|systemVersion    |string|Указывает внутреннюю версию компании.|
|businessProfileId|string|Указывает ID бизнес-профиля, связанный с компанией.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Вот представление JSON компании.

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}
```




