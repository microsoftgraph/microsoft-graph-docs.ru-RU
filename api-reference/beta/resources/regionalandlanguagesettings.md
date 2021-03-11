---
title: тип ресурса regionalAndLanguageSettings
description: Ресурс, представляющий региональные и языковые предпочтения пользователей
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 25af8de5a93bc67ed774b161ec63c1698434efb2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721315"
---
# <a name="regionalandlanguagesettings-resource-type"></a>тип ресурса regionalAndLanguageSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Открытый тип, который представляет предпочтения пользователя для языков в различных контекстах, а также для регионального языка и форматирования, который диски календаря по умолчанию, и форматирование для даты и времени.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                   | Описание                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [получение](../api/regionalAndLanguageSettings-get.md);       | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | Чтение свойств объекта **regionalAndLanguageSettings.**                                       |
| [Обновление](../api/regionalandlanguagesettings-update.md) | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | Обновление всех или подмножества свойств объекта **regionalAndLanguageSettings** для пользователя. |

## <a name="properties"></a>Свойства
| Свойство                   | Тип                                                  | Описание                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| defaultDisplayLanguage     | [localeInfo](localeinfo.md)                           | Предпочтительный язык пользовательского интерфейса пользователя (меню, кнопки, ленты, предупреждающие сообщения) для веб-приложений Майкрософт.<br><br>Возвращается по умолчанию. Значение null не допускается. |
| authoringLanguages         | Коллекция объектов [localeInfo](localeinfo.md)                                 | Приоритизированный список языков, на которые пользователь читает и авторов.<br><br>Возвращается по умолчанию. Значение null не допускается.                                                              |
| defaultTranslationLanguage | [localeInfo](localeinfo.md)                 | Язык, на который пользователь ожидает перевода документов, электронной почты и сообщений.<br><br>Возвращается по умолчанию.                                                    |
| defaultSpeechInputLanguage | [localeInfo](localeinfo.md)                 | Язык, который пользователь должен использовать в качестве ввода для текстовых сценариев речи.<br><br>Возвращается по умолчанию.                                                              |
| defaultRegionalFormat      | [localeInfo](localeinfo.md)            | Локализ, который диски по умолчанию даты, времени и форматирования календаря.<br><br>Возвращается по умолчанию.                                                                 |
| regionalFormatOverrides    | [regionalFormatOverrides](regionalformatoverrides.md) | Позволяет пользователю переопределять значение defaultRegionalFormat с помощью определенных форматов поля.<br><br>Возвращается по умолчанию.                                                      |
| translationPreferences     | [translationPreferences](translationPreferences.md)   | Предпочтительные параметры пользователя при потреблении переведенных документов, электронной почты, сообщений и веб-сайтов.<br><br>Возвращается по умолчанию. Значение null не допускается.                                       |

## <a name="json-representation"></a>Представление JSON

Ниже приводится определение ресурса JSON.

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages": [{"@odata.type":"microsoft.graph.localeInfo"}],
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat": {"@odata.type":"microsoft.graph.localeInfo"},
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"},
    "translationPreferences":{"@odata.type":"microsoft.graph.translationPreferences"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


