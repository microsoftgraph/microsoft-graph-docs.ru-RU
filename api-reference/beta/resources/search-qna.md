---
title: Тип ресурса qna
description: Представляет вопрос и ответ (Q&A) в Поиск (Майкрософт).
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d17f10b3613bb4e88791c90fd81e0440ece8eb2d
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602786"
---
# <a name="qna-resource-type"></a>Тип ресурса qna

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Q&Как результаты административного ответа на странице результатов поиска, которые предоставляют ответы на определенные ключевые слова поиска. Вопрос&Как разрешить администраторам отвечать на вопросы пользователя непосредственно в поиске, а не предоставлять ссылку на веб-страницу. Q&A имеет множество свойств, которые позволяют администраторам сделать общие ресурсы более доступными в своей организации.

Наследуется от [searchAnswer](../resources/search-searchAnswer.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление qnas](../api/search-searchentity-list-qnas.md)|[Коллекция microsoft.graph.search.qna](../resources/search-qna.md)|Получение списка объектов [qna](../resources/search-qna.md) и их свойств.|
|[Создание QNA](../api/search-searchentity-post-qnas.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Создайте новый [объект qna](../resources/search-qna.md) .|
|[Получение QNA](../api/search-qna-get.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Чтение свойств и связей объекта [qna](../resources/search-qna.md) .|
|[Обновление QNA](../api/search-qna-update.md)|[microsoft.graph.search.qna](../resources/search-qna.md)|Обновление свойств объекта [qna](../resources/search-qna.md) .|
|[Удаление QNA](../api/search-qna-delete.md)|Нет|Удаляет объект [qna](../resources/search-qna.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор (GUID) для qna. Наследуется от [сущности](../resources/entity.md).|
|displayName|String|Вопрос, отображаемый в результатах поиска. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|description|Строка|Ответ, отображаемый в результатах поиска. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|Ссылка на URL-адрес Qna. Когда пользователи щелкают этот QNA в результатах поиска, они будут переходить по этому URL-адресу. Наследуется от [searchAnswer](../resources/search-searchAnswer.md).|
|lastModifiedBy|[Microsoft.graph.identitySet](../resources/identityset.md)|Сведения о пользователе, который создал или в последний раз изменил QNA. Наследуется от [searchAnswer](../resources/search-searchAnswer.md). Только для чтения. |
|lastModifiedDateTime|DateTimeOffset| Метка времени создания или изменения QNA. Наследуется от [searchAnswer](../resources/search-searchAnswer.md). Только для чтения.|
|availabilityStartDateTime|DateTimeOffset|Метка времени, когда qna начнет отображаться в качестве результата поиска. Задайте значение `null` "Всегда доступно".|
|availabilityEndDateTime|DateTimeOffset|Метка времени остановки qna в качестве результата поиска. Задайте значение `null` "Всегда доступно".|
|languageTags|Коллекция строк|Список географически определенных языков, в которых можно просмотреть это QnA. Каждое значение тега языка соответствует шаблону {language}-{region}. Например, английский язык, `en-us` используемый в США. Список [возможных значений см](search-api-answers-overview.md#supported-language-tags) . в поддерживаемых языковых тегах. |
|Платформ|Коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, которые могут просматривать этот QNA. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[Коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты QNA для разных стран или устройств. Используйте, если необходимо показывать пользователям разные материалы в зависимости от их устройства, страны или региона или и того, и другого. Параметры даты и группы будут применяться ко всем вариантам.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые инициирует отображение этого QNA в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние qna. Возможные значения: `published`, `draft`, или `excluded``unknownFutureValue`.|
|isSuggested|Boolean| Значение true, если этот вопрос был предложен администратору пользователем или был минифицирован и предложен корпорацией Майкрософт. Только для чтения.|
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

