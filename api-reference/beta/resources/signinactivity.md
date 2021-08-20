---
title: тип ресурса signInActivity
description: Предоставляет последний интерактивный или неинактивный вход для определенного пользователя.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1ba087ba9a351fc2aba30c1c11be7e2ef0765b26
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384417"
---
# <a name="signinactivity-resource-type"></a>тип ресурса signInActivity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет последний интерактивный или неинактивный вход для конкретного [пользователя.](user.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|Последняя интерактивная дата регистрации для конкретного пользователя. Это поле можно использовать для вычисления последнего времени, когда пользователь вписался в каталог с помощью интерактивного метода проверки подлинности. Это поле можно использовать для создания отчетов, например неактивных пользователей. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2014 г. : `'2014-01-01T00:00:00Z'` . Дополнительные сведения об использовании значения этого свойства см. в рубке Управление неактивными учетными записями пользователей [в Azure AD.](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
|lastSignInRequestId|String|Запрос идентификатора последней интерактивной входной записи, выполненной этим пользователем.|
|lastNonInteractiveSignInDateTime|DateTimeOffset|Последняя неакактивная дата регистрации для конкретного пользователя. Это поле можно использовать для вычисления последнего времени, когда клиент вписался в каталог от имени пользователя. Поскольку некоторые пользователи могут использовать клиентов для доступа к ресурсам клиента, а не непосредственного входного доступа к клиенту, для идентификации неактивных пользователей можно использовать дату неинактивную регистрацию вместе с lastSignInDateTime. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2014 г. : `'2014-01-01T00:00:00Z'` . Дополнительные сведения об использовании значения этого свойства см. в рубке Управление неактивными учетными записями пользователей [в Azure AD.](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
|lastNonInteractiveSignInRequestId|Строка|Запрос идентификатора последнего неинактивного входного номера, выполненного этим пользователем.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String",
  "lastNonInteractiveSignInDateTime": "String (timestamp)",
  "lastNonInteractiveSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
