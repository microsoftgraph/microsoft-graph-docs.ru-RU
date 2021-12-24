---
title: тип ресурса signInActivity
description: Предоставляет последний интерактивный или неинактивный вход для определенного пользователя.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c67966902315f4b8ef4ab75f7f0c8d3cb5988f98
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604184"
---
# <a name="signinactivity-resource-type"></a>тип ресурса signInActivity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет последний интерактивный или неинактивный вход для конкретного [пользователя.](user.md) Так как signInActivity описывает свойство объекта пользователя, Azure AD сохраняет signinactivity для пользователей до тех пор, пока существуют объекты пользователя. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|lastSignInDateTime|DateTimeOffset|Последняя интерактивная дата и время регистрации для конкретного пользователя. Это поле можно использовать для вычисления последнего времени, когда пользователь вписался в каталог с помощью интерактивного метода проверки подлинности. Это поле можно использовать для создания отчетов, например неактивных пользователей. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2014 г. : `'2014-01-01T00:00:00Z'` . Azure AD поддерживает интерактивные входы с апреля 2020 г. Дополнительные сведения об использовании значения этого свойства см. в рубке Управление неактивными учетными записями пользователей [в Azure AD.](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
|lastSignInRequestId|Строка|Запрос идентификатора последней интерактивной входной записи, выполненной этим пользователем.|
|lastNonInteractiveSignInDateTime|DateTimeOffset|Последняя неакактивная дата регистрации для конкретного пользователя. Это поле можно использовать для вычисления последнего времени, когда клиент вписался в каталог от имени пользователя. Поскольку некоторые пользователи могут использовать клиентов для доступа к ресурсам клиента, а не непосредственного входного доступа к клиенту, для идентификации неактивных пользователей можно использовать дату неинактивную регистрацию вместе с lastSignInDateTime. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, полночь UTC 1 января 2014 г. : `'2014-01-01T00:00:00Z'` . Azure AD поддерживает неинактивную регистрацию с мая 2020 г. Дополнительные сведения об использовании значения этого свойства см. в рубке Управление неактивными учетными записями пользователей [в Azure AD.](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)|
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
