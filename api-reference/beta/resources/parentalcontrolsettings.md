---
title: Тип ресурса parentalControlSettings
description: Указывает параметры родительского элемента управления для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.
ms.openlocfilehash: 96f0fa96f9257187e404b61eaca877302d50ccee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075723"
---
# <a name="parentalcontrolsettings-resource-type"></a>Тип ресурса parentalControlSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Указывает параметры родительского элемента управления для приложения. Эти параметры определяют на взаимодействие с согласия пользователя.

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
:---------------|:--------|:----------|
|countriesBlockedForMinors|Коллекция String| Указывает [двухбуквенный код страны ISO](https://www.iso.org/iso-3166-country-codes.html). Доступ к приложению будут блокироваться для минорам из указанной в этом списке.|
|legalAgeGroupRule| String | Правило срок хранения в юридическом группы, которая применяется для пользователей приложения. Может быть установлено одно из следующих значений: <table><tr><th>Значение</th><th>Description</th></tr><tr><td>Allow (разрешить)</td><td>Значение, используемое по умолчанию. Требуют соблюдения юридических по меньшей мере. Это означает, что является обязательным для минорам в Европейском союзе и Корея, родительское согласие.</td></tr><tr><td>RequireConsentForPrivacyServices</td><td>Обеспечивает пользователю для указания Дата рождения в соответствии с правилами COPPA. </td></tr><tr><td>RequireConsentForMinors</td><td>Требуется родительское согласие для возраста ниже 18, вне зависимости от страны дополнительный номер правила.</td></tr><tr><td>RequireConsentForKids</td><td>Требуется родительское согласие для возраста ниже 14, вне зависимости от страны дополнительный номер правила.</td></tr><tr><td>BlockMinors</td><td>Блоки минорам с помощью приложения.</td></tr></table> |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
