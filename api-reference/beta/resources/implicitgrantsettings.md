---
title: неявный тип ресурсовGrantSettings
description: 'Указывает, может ли это веб-приложение запрашивать маркеры с помощью неявного потока OAuth 2.0. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: fe471eefe817e48468258195dae4c93331dd6e04
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547017"
---
# <a name="implicitgrantsettings-resource-type"></a>неявный тип ресурсовGrantSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


