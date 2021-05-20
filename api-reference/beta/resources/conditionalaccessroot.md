---
title: тип ресурса conditionalAccess
description: Ресурс **conditionalaccess** является точкой входа для объектной модели Conditinal Access. Он не содержит никаких полезных свойств.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3683965cda79f003cb5e548101272d869be902b8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547529"
---
# <a name="conditionalaccess-resource-type"></a>тип ресурса conditionalaccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **conditionalAccess —** это точка входа для объектной модели условного доступа. Он не содержит никаких полезных свойств.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) |[conditionalAccessPolicy](conditionalaccesspolicy.md)| Создайте **новое условноеaccessPolicy,** разместив в коллекции conditionalAccessPolicy.|
|[Создание namedLocations](../api/conditionalaccessroot-post-namedlocations.md) |[namedLocation](namedlocation.md)| Создайте новые **именаLocations,** разместив их в коллекции namedLocations.|
|[Создание проверки подлинностиContextClassReferences](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md)|[authenticationContextClassReferences](authenticationcontextclassreference.md)|Создайте новую **проверку подлинностиContextClassReferences,** разместив их в коллекции authenticationContextClassReferences.|


## <a name="properties"></a>Свойства

Ресурс conditionalAccess является точкой входа для объектной модели условного доступа и не содержит никаких свойств.

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|conditionalAccessPolicy|Коллекция [conditionalAccessPolicy](conditionalaccesspolicy.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных политик условного доступа.|
|namedLocations|[коллекция namedLocations](namedlocation.md)| Только для чтения. Допускается значение null. Возвращает коллекцию указанных именных местоположений.|
|authenticationContextClassReferences|[коллекция authenticationContextClassReferences](authenticationcontextclassreference.md)|Только для чтения. Допускается значение null. Возвращает коллекцию ссылок на определенный класс проверки подлинности.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditional access resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

