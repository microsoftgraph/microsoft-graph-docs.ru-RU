---
title: Тип ресурса Усераккаунтинформатион
description: Тип ресурса Усераккаунтинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b2993348b19cd0f55cbb7d26369276ea97006960
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846083"
---
# <a name="useraccountinformation-resource-type"></a>Тип ресурса Усераккаунтинформатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения, специально связанные с учетной записью пользователя, будь то учетная запись Azure AD или учетная запись Майкрософт. Идентификатор сущности задается соответствующим идентификаторам Azure AD AD или CID учетной записи Майкрософт соответственно. Эти поля доступны только для чтения через Microsoft Graph и должны редактироваться с помощью профиля пользователя или администратора клиента для соответствующего интерфейса.

Наследуется от [итемфацет](itemfacet.md).

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                                         | Описание                                                                   |
|:-------------------------------------------------------------------|:----------------------------------------------------|:------------------------------------------------------------------------------|
| [Получение Усераккаунтинформатион](../api/useraccountinformation-get.md) | [усераккаунтинформатион](useraccountinformation.md) | Чтение свойств и связей объекта **усераккаунтинформатион** . |

## <a name="properties"></a>Свойства

| Свойство             | Тип                        | Описание                                                                                                                               |
|:---------------------|:----------------------------|:------------------------------------------------------------------------------------------------------------------------------------------|
| ageGroup             | String                      | Показывает группу возрастных пользователей. Допустимые `null` значения `minor` , `notAdult` и `adult` они создаются каталогом и не могут быть изменены. |
| countryCode          | String                      | Содержит двухбуквенный код страны, связанный с учетной записью пользователя.                                                                |
| преферредлангуажетаг | [localeInfo](localeinfo.md) | Содержит язык, который пользователь связал с учетной записью как предпочитаемый.                                                               |
| userPrincipalName    | String                      | Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.                                                                    |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": ""
}-->

```json
{
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {"@odata.type": "microsoft.graph.localeInfo"},
  "userPrincipalName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAccountInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
