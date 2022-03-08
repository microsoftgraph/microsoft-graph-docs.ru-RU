---
title: тип ресурса qna
description: Представляет вопрос и ответ (Q&A) в Поиск (Майкрософт).
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b205c31b533affd63b9d38650e1dfe8aa1fb2e3d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339035"
---
# <a name="qna-resource-type"></a>тип ресурса qna

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Q&Как и результаты административного ответа на странице результатов поиска, которые предоставляют ответы на определенные ключевые слова поиска. Q&Как разрешить администраторам отвечать на вопросы пользователя непосредственно в поиске, а не предоставлять ссылку на веб-страницу. Q&A имеет множество свойств, которые позволяют администраторам сделать общие ресурсы более доступными в своей организации.

Наследуется [из searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список qnas](../api/search-searchentity-list-qnas.md)|[коллекция microsoft.graph.search.qna](../resources/search-qna.md)|Получите список объектов [qna](../resources/search-qna.md) и их свойств.|
|[Создание qna](../api/search-searchentity-post-qnas.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Создание нового [объекта qna](../resources/search-qna.md) .|
|[Get qna](../api/search-qna-get.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Ознакомьтесь с свойствами и отношениями [объекта qna](../resources/search-qna.md) .|
|[Обновление qna](../api/search-qna-update.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Обновление свойств объекта [qna](../resources/search-qna.md) .|
|[Удаление qna](../api/search-qna-delete.md)|Нет|Удаляет [объект qna](../resources/search-qna.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор (GUID) для qna. Наследуется [от сущности](../resources/entity.md).|
|displayName|Строка|Вопрос, отображаемый в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|description|String|Ответ, отображаемый в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|URL-ссылка Qna. Когда пользователи щелкают этот qna в результатах поиска, они перейдут на этот URL-адрес. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Сведения о пользователе, который создал или в последний раз изменил qna. Наследуется [от searchAnswer](../resources/search-searchAnswer.md). Только для чтения. |
|lastModifiedDateTime|DateTimeOffset| Время создания или редактирования QNA. Наследуется [от searchAnswer](../resources/search-searchAnswer.md). Только для чтения.|
|availabilityStartDateTime|DateTimeOffset|Timestamp того, когда qna начнет отображаться в качестве результата поиска. Установите, как `null` всегда доступно.|
|availabilityEndDateTime|DateTimeOffset|Timestamp того, когда qna остановится, чтобы появиться в качестве результата поиска. Установите, как `null` всегда доступно.|
|LanguageTags|Коллекция строк|Список языковых имен, которые географически специфичны и которые можно просмотреть в этом QnA. Каждое значение тега языка следует шаблону {language}-{REGION}. В качестве примера можно `en-US` привести английский язык, используемый в США. В [списке](search-api-answers-overview.md#supported-language-tags) возможных значений см. поддерживаемые языковые теги. |
|платформы|коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, которые могут просматривать этот qna. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты QNA для разных стран или устройств. Используйте, когда необходимо показывать пользователям различные контенты на основе их устройства, страны или региона или обоих. Параметры даты и группы будут применяться для всех вариантов.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые запускают этот qna, отображаются в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние qna. Возможные значения: `published`, , `draft`, или `excluded``unknownFutureValue`.|
|isSuggested|Boolean| True, если этот qna был предложен администратору пользователем или был заминирован и предложен Корпорацией Майкрософт. Только для чтения.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать этот qna.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.qna",
  "baseType": "microsoft.graph.search.searchAnswer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.qna",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
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

