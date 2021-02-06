---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского контроля для приложения. Эти параметры контролируют условия получения согласия.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f63f81af9e35183a15ab07b1f8e8fce9e8488bae
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136005"
---
# <a name="parentalcontrolsettings-resource-type"></a>Тип ресурса parentalControlSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает параметры родительского контроля для приложения. Эти параметры контролируют условия получения согласия.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Коллекция объектов string| Указывает [коды стран ISO](https://www.iso.org/iso-3166-country-codes.html)из двух букв. Доступ к приложению будет заблокирован для несовершеннолетних из стран, указанных в этом списке.|
|legalAgeGroupRule| Строка | Указывает правило юридической возрастной группы, которое применяется к пользователям приложения. Может иметь одно из следующих значений: <table><tr><th>Значение</th><th>Описание</th></tr><tr><td>Разрешить</td><td>Значение, используемое по умолчанию. Принудительно применяет минимальный юридический уровень. Это означает, что для несовершеннолетних в Европейском Союзе и Республике Корея требуется родительское согласие.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Принудительно применяет пользователя к указанию даты рождения в соответствии с правилами COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Требуется родительское согласие для детей не ниже 18 лет, независимо от правил для несовершеннолетних в стране.</td></tr><tr><td>RequireConsentForKids</td><td>Требуется родительское согласие для детей до 14 лет, независимо от правил для несовершеннолетних в стране.</td></tr><tr><td>BlockMinors</td><td>Блокирует использование приложения несовершеннолетних.</td></tr></table> |

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


