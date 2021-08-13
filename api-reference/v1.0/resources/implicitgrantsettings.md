---
title: неявный тип ресурсовGrantSettings
description: Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ID и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, необходимо установить по крайней мере одно из следующих свойств.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: bfe1e38dfdbdeffb81d34db0f68628c58a37421ee6da260be08e4c6f05c37015
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155136"
---
# <a name="implicitgrantsettings-resource-type"></a>неявный тип ресурсовGrantSettings

Пространство имен: microsoft.graph

Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ID и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, необходимо установить по крайней мере одно из следующих свойств.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Логический | Указывает, может ли это веб-приложение запрашивать маркер ID с помощью неявного потока OAuth 2.0.|
|enableAccessTokenIssuance| Логический | Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2.0.|

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

