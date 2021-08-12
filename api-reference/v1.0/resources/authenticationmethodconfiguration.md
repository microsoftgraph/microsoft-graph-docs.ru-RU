---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b94a80f212f7bbf4fe3f23b34828c8afec5cd3f72d7cc460ffe9455b1e2b3ae0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160102"
---
# <a name="authenticationmethodconfiguration-resource-type"></a>тип ресурса authenticationMethodConfiguration
Пространство имен: microsoft.graph

Представляет политику метода проверки подлинности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Имя политики.|
|state|authenticationMethodState|Состояние политики. Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
