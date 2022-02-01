---
title: тип ресурса broadcastMeetingCaptionSettings
description: Представляет параметры подписи события Microsoft Teams в прямом эфире.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c0f1ef0288627561c17bac5fa4c0a0c9f4af74e7
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290961"
---
# <a name="broadcastmeetingcaptionsettings-resource-type"></a>тип ресурса broadcastMeetingCaptionSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры подписи события Microsoft Teams [в прямом эфире](/microsoftteams/teams-live-events/what-are-teams-live-events). Подробные сведения об использовании подписей в Teams клиенте см. в материале [Use live captions in a live event](https://support.microsoft.com/office/use-live-captions-in-a-live-event-1d6778d4-6c65-4189-ab13-e2d77beb9e2a).

## <a name="properties"></a>Свойства

| Свойство             | Тип              | Описание                                                     |
|:---------------------|:------------------|:----------------------------------------------------------------|
| isCaptionEnabled     | Логическое           | Указывает, включена ли подпись для этого Teams в прямом эфире. |
| spokenLanguage       | String            | Разговорный язык.                                            |
| translationLanguages | Коллекция строк | Языки перевода (выберите до 6).                     |

> [!TIP]
>
> Языки перевода не могут содержать тот же языковой код, что и разговорный язык.

### <a name="spokenlanguage-values"></a>значения spokenLanguage

В следующей таблице показаны поддерживаемые языковые коды для разговорных языков.

| Разговорный язык           | Значение   |
|:--------------------------|:--------|
| Китайский (упрощенный, PRC) | zh-Hans |
| Нидерландский (Нидерланды)       | nl      |
| Английский (США)   | ru      |
| Французский (Канада)           | fr-ca   |
| Французский (Франция)           | fr      |
| Немецкий (Германия)          | de      |
| Хинди (Индия)             | hi      |
| Итальянский (Италия)           | оно      |
| Японский (Япония)          | ja      |
| Корейский (Корея)            | ko      |
| португальский (Бразилия);       | pt      |
| Русский (Россия)          | ru      |
| Испанский (Испания)           | es      |
| Испанский (Мексика)          | es-mx   |
| Шведский (Швеция)          | sv      |

### <a name="translationlanguaes-values"></a>значения translationLanguaes

В следующей таблице показаны поддерживаемые языковые коды для языков перевода.

| Язык перевода                     | Значение   |
|------------------------------------------|---------|
| Afrikaans (Южная Африка)                 | af      |
| Арабский (Египет)                           | ar      |
| Боснийский (латиница)                          | bs      |
| Болгария (Болгария)                     | bg      |
| Каталанский                                  | ca      |
| Китайский (упрощенный, PRC)                | zh-Hans |
| Китайский (Tranditional, Гонконг S.A.R.) | yue     |
| Китайский (Tranditional)                   | zh-Hant |
| Креоль (Гаити)                           | ht      |
| Хорватский (Хорватия)                       | hr      |
| Чешский (Чешская Республика)                   | cs      |
| Датский (Дания)                         | da      |
| Нидерландский (Нидерланды)                      | nl      |
| Английский (США)                  | ru      |
| Эстонский (Эстония)                       | et      |
| Филиппинский (Филиппины)                   | fil     |
| Финский (Финляндия)                        | fi      |
| Французский (Канада)                          | fr-ca   |
| Французский (Франция)                          | fr      |
| Немецкий (Германия)                         | de      |
| Греческий (Греция)                           | el      |
| Иврит (Израиль)                          | он      |
| Хинди (Индия)                            | hi      |
| Hmong                                    | mww     |
| Венгерский (Венгрия)                      | hu      |
| Индонезийский                               | id      |
| Итальянский (Италия)                          | оно      |
| Японский (Япония)                         | ja      |
| Клингон                                  | tlh     |
| Корейский (Корея)                           | ko      |
| Латышский (Латвия)                         | lv      |
| Литовский (Литва)                   | lt      |
| Малагасий (Мадагаскар)                    | mg      |
| Малайский (Малайзия)                         | ms      |
| Мальтийский (Мальта)                          | mt      |
| Персидский (Иран)                           | fa      |
| Польский (Польша)                          | pl      |
| Португальский (Бразилия)                      | pt      |
| Querétaro Otomi                          | otq     |
| Румынский (Румыния)                       | ro      |
| Русский (Россия)                         | ru      |
| Самоан                                   | sm      |
| Сербский (латиница)                          | sr-latn |
| Serbian Cyrillic                         | sr-cyrl |
| Словак (Словакия)                        | sk      |
| Словенский                                | sl      |
| Испанский (Испания)                          | es      |
| Суахили (Кения)                          | sw      |
| Шведский (Швеция)                         | sv      |
| Tahitian                                 | ty      |
| Тайский (Таиланд)                          | th      |
| Tongan                                   | на      |
| Турецкий (Турция)                         | tr      |
| Украинский (Украина)                      | uk      |
| Урду (Исламская Республика Пакистан)      | ur      |
| Вьетнам (Вьетнам)                     | vi      |
| Валлийский (Великобритания)                   | cy      |
| Yucatec Maya                             | yua     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.broadcastMeetingCaptionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.broadcastMeetingCaptionSettings",
  "isCaptionEnabled": "Boolean",
  "spokenLanguage": "String",
  "translationLanguages": [
    "String"
  ]
}
```
