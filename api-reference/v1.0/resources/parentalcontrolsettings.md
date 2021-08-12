---
title: тип ресурса parentalControlSettings
description: Указывает параметры родительского контроля для приложения. Эти параметры контролируют опыт согласия.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e5e232972cf86ded43e74a57257986dddb61098e2451b7639e7de9e93291618d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180490"
---
# <a name="parentalcontrolsettings-resource-type"></a>тип ресурса parentalControlSettings

Пространство имен: microsoft.graph

Указывает параметры родительского контроля для приложения. Эти параметры контролируют опыт согласия.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Коллекция String| Указывает [коды страны ISO](https://www.iso.org/iso-3166-country-codes.html)с двумя буквами. Доступ к приложению будет заблокирован для несовершеннолетних из стран, указанных в этом списке.|
|legalAgeGroupRule| String | Указывает правило юридической возрастной группы, которое применяется к пользователям приложения. Может иметь одно из следующих значений: <table><tr><th>Значение</th><th>Описание</th></tr><tr><td>Разрешить</td><td>Значение, используемое по умолчанию. Обеспечивает соблюдение юридического минимума. Это означает, что для несовершеннолетних в Европейском союзе и Корее требуется родительское согласие.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>В соответствии с правилами COPPA пользователь должен указать дату рождения. </td></tr><tr><td>RequireConsentForMinors</td><td>Требуется родительское согласие для детей в возрасте до 18 лет, независимо от правил страны.</td></tr><tr><td>RequireConsentForKids</td><td>Требуется родительское согласие для детей в возрасте до 14 лет, независимо от правил страны.</td></tr><tr><td>BlockMinors</td><td>Блокирует использование приложения для несовершеннолетних.</td></tr></table> |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```

