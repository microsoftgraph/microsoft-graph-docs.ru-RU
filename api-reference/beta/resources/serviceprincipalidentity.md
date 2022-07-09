---
title: Тип ресурса servicePrincipalIdentity
description: Модели идентификации субъекта-службы.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bfd53005643633a5f406555eac21d63bec8db8bc
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698424"
---
# <a name="serviceprincipalidentity-resource-type"></a>Тип ресурса servicePrincipalIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Модели идентификации субъекта-службы.

Наследуется от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|appId|String| Идентификатор приложения субъекта-службы. |
|displayName|Строка| Отображаемое имя удостоверения субъекта-службы. Наследуется от [удостоверения](../resources/identity.md). |
|id|String| Идентификатор удостоверения субъекта-службы. Наследуется от [удостоверения](../resources/identity.md). |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
