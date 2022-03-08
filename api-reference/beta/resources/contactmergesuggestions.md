---
title: тип ресурса contactMergeSuggestions
description: Представляет функцию, чтобы предложить объединение контактных элементов, Outlook обнаруживает дубликаты в списке контактов пользователя
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 56237901cca14d075dfa7f03729a9261d8d281a0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339332"
---
# <a name="contactmergesuggestions-resource-type"></a>тип ресурса contactMergeSuggestions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет функцию, чтобы предложить слияние контактных элементов, Outlook обнаруживает дубликаты в списке контактов пользователя.

Этот ресурс предоставляет средства, позволяющие включить или отключить функцию на уровне пользователя. По умолчанию предложение включено. Дубликаты контактных элементов остаются дубликатами в папке контактов, если пользователь не выберет их слияние.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/contactmergesuggestions-get.md);|[contactMergeSuggestions](contactmergesuggestions.md)|Ознакомьтесь с свойствами **объекта contactMergeSuggestions** .|
|[Обновление](../api/contactmergesuggestions-update.md)|Нет |Обновление свойств объекта **contactMergeSuggestions** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|`true` если функция слияния дублирующих контактов включена для пользователя; `false` если функция отключена. Значение по умолчанию — `true`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactMergeSuggestions",
  "openType": false
}
-->
``` json
{
  "isEnabled": "Boolean"
}
```

