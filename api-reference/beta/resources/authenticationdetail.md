---
title: Тип ресурса authenticationDetail
description: Предоставляет сведения о проверке подлинности для пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b888ec232a95c821ab00f6baa16e787cfbc7dd7f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136628"
---
# <a name="authenticationdetail-resource-type"></a>Тип ресурса authenticationDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о проверке подлинности для пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и PTA/PHS.

## <a name="properties"></a>Свойства

| Свойство                       | Тип           | Описание                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | Строка         | Тип метода проверки подлинности, используемого для выполнения этого шага проверки подлинности. Возможные значения: `Password` , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` .                            |
| authenticationMethodDetail     | Строка         | Сведения о методе проверки подлинности, используемом для выполнения этого шага проверки подлинности. Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения Authenticator) и источник пароля (например, облако, AD FS, PTA, PHS). |
| authenticationStepDateTime     | DateTimeOffset | Представляет сведения о дате и времени в формате ISO 8601 и всегда используется в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.                                           |
| authenticationStepRequirement  | Строка         | Шаг проверки подлинности, который это удовлетворит. Например, основная или многофакторная проверка подлинности.                                                                                                     |
| authenticationStepResultDetail | Строка         | Сведения о том, почему шаг был успешным или неудачным. Например, пользователь заблокирован, введен код мошенничества, не ввод данных с телефона : время и время действия, недостижимый телефон или утверждение в маркере.                                                     |
| succeeded                      | Boolean        | Указывает состояние шага проверки подлинности. Возможные значения: `succeeded` , `failed` .                                                                                                                                 |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

