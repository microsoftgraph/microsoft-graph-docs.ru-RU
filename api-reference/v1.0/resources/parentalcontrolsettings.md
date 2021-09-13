---
title: тип ресурса parentalControlSettings
description: Указывает параметры родительского контроля для приложения. Эти параметры контролируют опыт согласия.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c3b484c9c47f4d238c7e9e7c96e7316426fcaf5d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044465"
---
# <a name="parentalcontrolsettings-resource-type"></a>тип ресурса parentalControlSettings

Пространство имен: microsoft.graph

Указывает параметры родительского контроля для приложения. Эти параметры контролируют опыт согласия.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Коллекция String| Указывает [коды страны ISO](https://www.iso.org/iso-3166-country-codes.html)с двумя буквами. Доступ к приложению будет заблокирован для несовершеннолетних из стран, указанных в этом списке.|
|legalAgeGroupRule| Строка | Указывает правило юридической возрастной группы, которое применяется к пользователям приложения. Может иметь одно из следующих значений: <table><tr><th>Значение</th><th>Описание</th></tr><tr><td>Разрешить</td><td>Значение, используемое по умолчанию. Обеспечивает соблюдение юридического минимума. Это означает, что для несовершеннолетних в Европейском союзе и Корее требуется родительское согласие.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>В соответствии с правилами COPPA пользователь должен указать дату рождения. </td></tr><tr><td>RequireConsentForMinors</td><td>Требуется родительское согласие для детей в возрасте до 18 лет, независимо от правил страны.</td></tr><tr><td>RequireConsentForKids</td><td>Требуется родительское согласие для детей в возрасте до 14 лет, независимо от правил страны.</td></tr><tr><td>BlockMinors</td><td>Блокирует использование приложения для несовершеннолетних.</td></tr></table> |

## <a name="json-representation"></a>Представление в формате JSON
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

