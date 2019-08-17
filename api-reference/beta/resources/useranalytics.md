---
title: Тип ресурса Усераналитикс
description: Параметры пользователя и статистика действий.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 51e72d21cfb0e26e46a7d247f4ede59b112893ea
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450801"
---
# <a name="useranalytics-resource-type"></a>Тип ресурса Усераналитикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры пользователя и статистика действий.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
[Получение параметров](../api/useranalytics-get-settings.md) | [settings](settings.md) | Получение параметров пользователя для использования API аналитики.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|settings|[settings](settings.md)|Текущие параметры пользователя для использования API аналитики.|

## <a name="relationships"></a>Отношения

| Отношение | Тип        | Описание |
|:-------------|:------------|:------------|
|активитистатистикс|Коллекция [активитистатистикс](activitystatistics.md)| Коллекция рабочих действий, затраченных пользователем во время и за пределами рабочего времени. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "activityStatistics"
  ],
  "@odata.type": "microsoft.graph.userAnalytics"
}-->

```json
{
  "id": "string",
  "settings": {"@odata.type": "microsoft.graph.settings"},
  "activityStatistics": [{"@odata.type": "microsoft.graph.activityStatistics"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAnalytics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
