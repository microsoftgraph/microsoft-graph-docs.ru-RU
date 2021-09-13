---
title: неявный тип ресурсовGrantSettings
description: Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ID и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, необходимо установить по крайней мере одно из следующих свойств.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 2ccf78ded6c9fa482f5054e2734d369acf041b18
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118609"
---
# <a name="implicitgrantsettings-resource-type"></a>неявный тип ресурсовGrantSettings

Пространство имен: microsoft.graph

Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. Отдельные свойства доступны для запроса ID и маркеров доступа в рамках неявного потока. Чтобы включить неявный поток, необходимо установить по крайней мере одно из следующих свойств.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | Указывает, может ли это веб-приложение запрашивать маркер ID с помощью неявного потока OAuth 2.0.|
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

