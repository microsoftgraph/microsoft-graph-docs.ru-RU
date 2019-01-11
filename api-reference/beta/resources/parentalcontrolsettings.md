---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского элемента управления для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.
localization_priority: Normal
ms.openlocfilehash: bb6f776d5f206fb0ed35a999effc7bbdc0768512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806519"
---
# <a name="parentalcontrolsettings-resource-type"></a>Тип ресурса parentalControlSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Указывает параметры родительского элемента управления для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Коллекция String| Указывает [двухбуквенный код страны ISO](https://www.iso.org/iso-3166-country-codes.html). Доступ к приложению будут блокироваться для минорам из указанной в этом списке.|
|legalAgeGroupRule| Строка | Правило срок хранения в юридическом группы, которая применяется для пользователей приложения. Может быть установлено одно из следующих значений: <table><tr><th>Значение</th><th>Описание</th></tr><tr><td>Allow (разрешить)</td><td>Значение, используемое по умолчанию. Требуют соблюдения юридических по меньшей мере. Это означает, что является обязательным для минорам в Европейском союзе и Корея, родительское согласие.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Обеспечивает пользователю для указания Дата рождения в соответствии с правилами COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Требуется родительское согласие для возраста ниже 18, вне зависимости от страны дополнительный номер правила.</td></tr><tr><td>RequireConsentForKids</td><td>Требуется родительское согласие для возраста ниже 14, вне зависимости от страны дополнительный номер правила.</td></tr><tr><td>BlockMinors</td><td>Блоки минорам с помощью приложения.</td></tr></table> |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
