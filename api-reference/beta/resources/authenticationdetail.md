---
title: Тип ресурса Аусентикатиондетаил
description: Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97375635d86b1be8149035c94d183026a3d49a25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508089"
---
# <a name="authenticationdetail-resource-type"></a>Тип ресурса Аусентикатиондетаил

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о проверке подлинности для входа пользователя, например сведения о многофакторной проверке подлинности (MFA) и сведения о ПТА/ФС.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Параметр authenticationmethod|String||Тип метода проверки подлинности, используемый для выполнения этого этапа проверки подлинности. Возможные значения: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.|
|аусентикатионмесоддетаил|String|Сведения о методе проверки подлинности, используемом для выполнения этой процедуры проверки подлинности. Например, номер телефона (для SMS и голосовой связи), имя устройства (для приложения проверки подлинности) и источник пароля (Cloud, AD FS, ПТА, ФС). |
|аусентикатионстепдатетиме|DateTimeOffset|Представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
|аусентикатионстепрекуиремент|String|Шаг проверки подлинности, который удовлетворен. Например, Первичная проверка подлинности или многофакторная проверка подлинности.|
|аусентикатионстепресултдетаил|String|Сведения о причине успешного или неудачного завершения этапа. Например, пользователь блокируется, заменяется мошеннический код, не используется ввод с истекшим сроком ожидания, Телефон недоступен или утвержден в маркере.|
|закончил|Логический|Указывает состояние этапа проверки подлинности.|Возможные значения: `succeeded`, `failed`.|

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