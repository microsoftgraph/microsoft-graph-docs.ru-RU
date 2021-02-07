---
title: Тип ресурса implicitGrantSettings
description: Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ИД и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, по крайней мере одно из следующих свойств должно иметь true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58509ff0f0264a683aaae9c83d60e0f041ef0af7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133282"
---
# <a name="implicitgrantsettings-resource-type"></a>Тип ресурса implicitGrantSettings

Пространство имен: microsoft.graph

Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ИД и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, по крайней мере одно из следующих свойств должно иметь true.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | Указывает, может ли это веб-приложение запрашивать маркер ИД с помощью неявного потока OAuth 2.0.|
|enableAccessTokenIssuance| Boolean | Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2.0.|

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

