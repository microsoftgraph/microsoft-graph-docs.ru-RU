---
title: Тип ресурса закладок
description: Закладки — это административный ответ в Поиск (Майкрософт) результатов для общих поисковых запросов в организации. Закладки имеют множество свойств, которые позволяют администраторам сделать общие ресурсы более доступными в своей организации.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 24582a18ae2ad332a59bc3d8b2db28b3e3189b6a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339038"
---
# <a name="bookmark-resource-type"></a>Тип ресурса закладок

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Закладки — это административный ответ в Поиск (Майкрософт) результатов для общих поисковых запросов в организации. Закладки имеют множество свойств, которые позволяют администраторам сделать общие ресурсы более доступными в своей организации.

Наследуется [из searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Закладки списка](../api/search-searchentity-list-bookmarks.md)|[коллекция microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Получите список объектов [закладок](../resources/search-bookmark.md) и их свойств.|
|[Создание закладки](../api/search-searchentity-post-bookmarks.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Создайте новый [объект закладки](../resources/search-bookmark.md) .|
|[Получить закладки](../api/search-bookmark-get.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Ознакомьтесь с свойствами и отношениями объекта [закладки](../resources/search-bookmark.md) .|
|[Обновление закладки](../api/search-bookmark-update.md)|[microsoft.graph.search.bookmark](../resources/search-bookmark.md)|Обновление свойств объекта [закладки](../resources/search-bookmark.md) .|
|[Удаление закладки](../api/search-bookmark-delete.md)|Нет|Удаляет объект [закладки](../resources/search-bookmark.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор (GUID) для закладки. Наследуется [от сущности](../resources/entity.md).|
|displayName|Строка|Имя закладки, отображаемая в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|description|String|Описание закладки, показанное на странице результатов поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|ССЫЛКА URL-адреса закладок. Когда пользователи щелкают эту закладки в результатах поиска, они перейдут на этот URL-адрес. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Сведения о пользователе, который создал или в последний раз изменил закладки. Наследуется [от searchAnswer](../resources/search-searchAnswer.md). Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время создания или редактирования закладки. Наследуется [от searchAnswer](../resources/search-searchAnswer.md). Только для чтения. |
|categories|Коллекция String|Категории, обычно используемые для описания этой закладки. Например, ИТ и HR.|
|availabilityStartDateTime|DateTimeOffset|Время начала появления закладки в результате поиска. Установите, как `null` всегда доступно.|
|availabilityEndDateTime|DateTimeOffset|Время, когда закладки перестанут отображаться в результате поиска. Установите, как `null` всегда доступно.|
|LanguageTags|Коллекция строк|Список языковых имен, географически определенных и в которых можно просмотреть эту закладку. Каждое значение тега языка следует шаблону {language}-{REGION}. В качестве примера можно `en-US` привести английский язык, используемый в США. В [списке](search-api-answers-overview.md#supported-language-tags) возможных значений см. поддерживаемые языковые теги.|
|платформы|коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, способных просматривать эту закладку. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты закладки для разных стран или устройств. Используйте, когда необходимо показывать пользователям различные контенты на основе их устройства, страны или региона или обоих. Параметры даты и группы будут применяться для всех вариантов.|
|powerAppIds|Коллекция String|Список Power Apps, связанных с этой закладкой. Если пользователи добавляют существующие Power Apps в закладки, они могут выполнять задачи, например вводить время отпуска или сообщать о расходах на странице результатов поиска.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые запускают эту закладку, отображаются в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние закладки. Возможные значения: `published`, , `draft`, или `excluded``unknownFutureValue`.|
|isSuggested|Boolean|True, если эта закладка была предложена администратору пользователем или была заминирована и предложена Корпорацией Майкрософт. Только для чтения.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать эту закладку.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.bookmark",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.bookmark",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "categories": [
    "String"
  ],
  "availabilityStartDateTime": "String (timestamp)",
  "availabilityEndDateTime": "String (timestamp)",
  "languageTags": [
    "String"
  ],
  "platforms": [
    "String"
  ],
  "targetedVariations": [
    {
      "@odata.type": "microsoft.graph.search.answerVariant"
    }
  ],
  "powerAppIds": [
    "String"
  ],
  "keywords": {
    "@odata.type": "microsoft.graph.search.answerKeyword"
  },
  "state": "String",
  "isSuggested": "Boolean",
  "groupIds": [
    "String"
  ]
}
```

