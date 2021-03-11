---
title: тип ресурса signInActivity
description: Предоставляет последнюю дату записи для определенного пользователя.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e48d2e64c71e67c623582552224a11636c7c6c7c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721861"
---
# <a name="signinactivity-resource-type"></a>тип ресурса signInActivity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет дату последней записи для определенного [пользователя.](user.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|Последняя интерактивная дата регистрации для конкретного пользователя. Это поле можно использовать для вычисления последнего времени, когда пользователь вписался в каталог с помощью интерактивного метода проверки подлинности. Это поле можно использовать для создания отчетов, например неактивных пользователей. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2014 г. : `'2014-01-01T00:00:00Z'` . Дополнительные сведения об использовании значения этого свойства см. в рубке Управление неактивными учетными записями пользователей [в Azure AD.](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
|lastSignInRequestId|String|Запрос ID последнего входного знака, выполненного этим пользователем.|

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
  "lastSignInRequestId": "String"
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
