---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 52c2929d36ceaa250bd3843556073190da9d4152
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939490"
---
# <a name="implicitgrantsettings-resource-type"></a>Тип ресурса ИмплиЦитгрантсеттингс

Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|енаблеидтокениссуанце| Логический | Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.|
|енаблеакцесстокениссуанце| Логический | Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
