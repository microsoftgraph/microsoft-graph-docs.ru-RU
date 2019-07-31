---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92ba18488cc2700b565be47bac3874b6d75e1c13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005795"
---
# <a name="implicitgrantsettings-resource-type"></a>Тип ресурса ИмплиЦитгрантсеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|Енаблеидтокениссуанце| Boolean | Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.|
|Енаблеакцесстокениссуанце| Boolean | Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.|

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
