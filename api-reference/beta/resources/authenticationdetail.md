---
title: Тип ресурса authenticationDetail
description: Предоставляет сведения о проверке подлинности для входного пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и сведения о PTA/PHS.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0f7042b8b2be369c97e19cb038d7cf82fe07e96d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964568"
---
# <a name="authenticationdetail-resource-type"></a>Тип ресурса authenticationDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о проверке подлинности для входного пользователя, такие как сведения о многофакторной проверке подлинности (MFA) и сведения о PTA/PHS.

## <a name="properties"></a>Свойства

| Свойство                       | Тип           | Описание                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | Строка         | Тип метода проверки подлинности, используемого для выполнения этого шага проверки подлинности. Возможные значения: `Password` , , , , , `SMS` `Voice` `Authenticator App` `Software OATH token` `Satisfied by token` `Previously satisfied` .                            |
| authenticationMethodDetail     | Строка         | Сведения о методе проверки подлинности, используемом для выполнения этого шага проверки подлинности. Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения Authenticator) и источник паролей (например, облако, AD FS, PTA, PHS). |
| authenticationStepDateTime     | DateTimeOffset | Представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.                                           |
| authenticationStepRequirement  | Строка         | Шаг проверки подлинности, который это удовлетворит. Например, первичная проверка подлинности или многофакторная проверка подлинности.                                                                                                     |
| authenticationStepResultDetail | Строка         | Сведения о том, почему этот шаг был успешным или неудачным. Например, пользователь заблокирован, введен код мошенничества, нет ввода телефона - приурочиваемый, телефон недоступен, или утверждение в маркере.                                                     |
| успешно                      | Boolean        | Указывает состояние шага проверки подлинности. Возможные значения: `succeeded` , `failed` .                                                                                                                                 |

## <a name="json-representation"></a>Представление JSON

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

