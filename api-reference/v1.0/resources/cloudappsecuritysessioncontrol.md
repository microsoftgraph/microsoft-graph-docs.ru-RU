---
title: Тип ресурса Клаудаппсекуритисессионконтрол
description: Управление сеансами, используемое для применения проверок безопасности облачных приложений.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6271ae47f94abb0c449dc6bd7a0930468d08d2b5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384726"
---
# <a name="cloudappsecuritysessioncontrol-resource-type"></a>Тип ресурса Клаудаппсекуритисессионконтрол

Пространство имен: microsoft.graph

Управление сеансами, используемое для применения проверок безопасности облачных приложений. Инехритс из [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEnabled     |Boolean      | Указывает, включен ли элемент управления сеансом. |
|клаудаппсекурититипе|String| Возможные значения: `mcasConfigured`, `monitorOnly`, `blockDownloads`, `unknownFutureValue`. Для получения дополнительных сведений обратитесь [к разделу развертывание приложения условного доступа для популярных приложений](https://docs.microsoft.com/cloud-app-security/proxy-deployment-aad). |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecuritySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "cloudAppSecurityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecuritySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
