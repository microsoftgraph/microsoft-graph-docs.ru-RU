---
title: тип ресурса authenticationMethodsRoot
description: Контейнер для свойств навигации для ресурсов методов проверки подлинности Azure AD.
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e01fe33d73d67058bf765d3562c77ea657630ea6
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2021
ms.locfileid: "61403204"
---
# <a name="authenticationmethodsroot-resource-type"></a>тип ресурса authenticationMethodsRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для свойств навигации для ресурсов методов проверки подлинности Azure AD.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| Уникальный идентификатор. Наследуется от [сущности](../resources/entity.md).|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRoot",
  "id": "String (identifier)"
}
```