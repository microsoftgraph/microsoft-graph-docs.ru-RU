---
title: authenticationMethodConfigurations
description: объект authenticationMethodConfigurations.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 083ace96234a724fc4c9f6e1cdda0cbd8a99e22a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964952"
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
