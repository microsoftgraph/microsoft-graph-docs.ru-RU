---
title: Тип ресурса regionalAndLanguageSettings
description: Ресурс, представляющий региональные и языковые параметры пользователей
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 66734cba4c5d0e2997a4bfd5b70c54156821f5da
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934914"
---
# <a name="regionalandlanguagesettings-resource-type"></a>Тип ресурса regionalAndLanguageSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Открытый тип, который представляет предпочтения пользователя для языков в различных контекстах, а также региональных стандартов и форматирования, на котором задается календарь по умолчанию, и форматирования для даты и времени.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                   | Описание                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [получение](../api/regionalAndLanguageSettings-get.md);       | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | Чтение свойств объекта **regionalAndLanguageSettings.**                                       |
| [обновление](../api/regionalandlanguagesettings-update.md). | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | Обновление всех или подмножества свойств объекта **regionalAndLanguageSettings** для пользователя. |

## <a name="properties"></a>Свойства
| Свойство                   | Тип                                                  | Описание                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| defaultDisplayLanguage     | [localeInfo](localeinfo.md)                           | Предпочитаемый пользователем язык пользовательского интерфейса (меню, кнопки, ленты, предупреждения) для веб-приложений Майкрософт.<br><br>Возвращается по умолчанию. Значение null не допускается. |
| authoringLanguages         | Коллекция объектов localeInfo                                 | Приоритетный список языков, на которые пользователь читает и авторов.<br><br>Возвращается по умолчанию. Значение null не допускается.                                                              |
| defaultTranslationLanguage | localeInfo                                            | Язык, на который пользователь ожидает перевода документов, сообщений электронной почты и сообщений.<br><br>Возвращается по умолчанию.                                                    |
| defaultSpeechInputLanguage | localeInfo                                            | Язык, который пользователь должен использовать в качестве входных данных для текста в речевой сценарий.<br><br>Возвращается по умолчанию.                                                              |
| defaultRegionalFormat      | localeInfo                                            | Региональные стандарты, которые будут управлять форматированием даты, времени и календаря по умолчанию.<br><br>Возвращается по умолчанию.                                                                 |
| regionalFormatOverrides    | [regionalFormatOverrides](regionalformatoverrides.md) | Позволяет пользователю переопределять свой defaultRegionalFormat с помощью форматов, определенных для поля.<br><br>Возвращается по умолчанию.                                                      |

## <a name="json-representation"></a>Представление JSON

Ниже приводится определение ресурса в JSON.

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
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


