---
title: Тип ресурса Регионаландлангуажесеттингс
description: Ресурс, представляющий региональные и языковые параметры пользователей
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 0e6178b7d2a461365c759432d62efcffc44cfe6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073518"
---
# <a name="regionalandlanguagesettings-resource-type"></a>Тип ресурса Регионаландлангуажесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Открытый тип, который представляет предпочтения пользователя для языков в различных контекстах, а также для региональных языковых стандартов и форматирования, которые заменяют календарь по умолчанию и форматирование даты и времени.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                   | Описание                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [получение](../api/regionalAndLanguageSettings-get.md);       | [регионаландлангуажесеттингс](regionalAndLanguageSettings.md) | Чтение свойств объекта **регионаландлангуажесеттингс** .                                       |
| [Обновление](../api/regionalandlanguagesettings-update.md) | [регионаландлангуажесеттингс](regionalAndLanguageSettings.md) | Обновление всех или подмножества свойств объекта **регионаландлангуажесеттингс** для пользователя. |

## <a name="properties"></a>Свойства
| Свойство                   | Тип                                                  | Описание                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| дефаултдисплайлангуаже     | [localeInfo](localeinfo.md)                           | Предпочтительный язык пользовательского интерфейса пользователя (меню, кнопки, ленты, предупреждающие сообщения) для веб-приложений Майкрософт.<br><br>Возвращается по умолчанию. Значение null не допускается. |
| аусоринглангуажес         | Коллекция объектов localeInfo                                 | Приоритетный список языков, в которых пользователь читает и авторы.<br><br>Возвращается по умолчанию. Значение null не допускается.                                                              |
| дефаулттранслатионлангуаже | localeInfo                                            | Язык, на который пользователь ожидает документы, сообщения электронной почты и сообщения, преобразованные в.<br><br>Возвращается по умолчанию.                                                    |
| дефаултспичинпутлангуаже | localeInfo                                            | Язык, который пользователь должен использовать в качестве входных данных для сценариев преобразования текста в речь.<br><br>Возвращается по умолчанию.                                                              |
| дефаултрегионалформат      | localeInfo                                            | Языковой стандарт, который управляет форматированием даты, времени и календаря по умолчанию.<br><br>Возвращается по умолчанию.                                                                 |
| регионалформатоверридес    | [регионалформатоверридес](regionalformatoverrides.md) | Позволяет пользователю переопределять свои Дефаултрегионалформат с использованием определенных форматов полей.<br><br>Возвращается по умолчанию.                                                      |

## <a name="json-representation"></a>Представление JSON

Ниже приведено определение ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages":[{"@odata.type":"microsoft.graph.localeInfo"}] ,
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat":{"@odata.type":"microsoft.graph.localeInfo"} ,
    "regionalFormatOverrides":{"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


