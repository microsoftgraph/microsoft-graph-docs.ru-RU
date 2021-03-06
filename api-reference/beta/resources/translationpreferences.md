---
title: тип ресурса translationPreferences
description: Ресурс, представляющий параметры параметров перевода пользователя.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: b2e45f797709067e52f142c3de3f2be566b55201
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518169"
---
# <a name="translationpreferences-resource-type"></a>тип ресурса translationPreferences

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запись в переопределяемом списке языка перевода пользователя.

## <a name="properties"></a>Свойства

|Свойство             |Тип                                         |Описание                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|translationBehavior  |[translationBehavior](#translationbehavior-values)       |Предпочтительное поведение пользователя для перевода.<br><br>Возвращается по умолчанию. Значение null не допускается. |                   
|LanguageOverrides    |[коллекция translationLanguageOverride](translationLanguageOverride.md)                | Переопределять поведение для языков, если таково.<br><br>Возвращается по умолчанию.|
|untranslatedLanguages|Коллекция String| Список языков, которые пользователю не нужно переводить. Это вычисляется из коллекции **authoringLanguages** в [regionalAndLanguageSettings](regionalandlanguagesettings.md)и **коллекции languageOverrides** в **translationPreferences.** В списке указаны нейтральные культурные значения, которые включают языковый код без какой-либо страны или региона. Например, он указывает "fr" для нейтральной французской культуры, но не "fr-FR" для французской культуры во Франции. <br><br>Возвращается по умолчанию. Только для чтения.| 

### <a name="translationbehavior-values"></a>значения translationBehavior

|Member |Описание                                                                  |
|-------|-----------------------------------------------------------------------------|
|Спросите    |Запрос пользователя перед переводом сообщений/чатов/веб-страниц для пользователя.|
|Да    |Автоматически перевод сообщений/чатов/веб-страниц для пользователя.           |
|Нет     |Не предлагай пользователю подсказок или автоматический перевод.                 |



## <a name="json-representation"></a>Представление JSON

Ниже приводится определение ресурса JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationPreferences"
}-->

```json
{
    "translationBehavior": "string",
    "languageOverrides": [{"@odata.type":"microsoft.graph.translationLanguageOverride"}],
    "untranslatedLanguages": ["string"]
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


