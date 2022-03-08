---
title: Обновление qna
description: Обновление свойств объекта qna.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: da045a3ed91bdc6ad5441fe9a854d225c144208d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339654"
---
# <a name="update-qna"></a>Обновление qna
Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [qna](../resources/search-qna.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| SearchConfiguration.Read.All, SearchConfiguration.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /search/qna/{qnaId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [qna](../resources/search-qna.md) . Поставляем значения для соответствующих полей, которые должны быть обновлены. Существующие свойства, не включенные в тело запроса, будут поддерживать прежние значения или пересчитываться на основе изменений в других значениях свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.
>**Примечание:** Обновления свойств коллекции обновят всю коллекцию. Любые обновления коллекции, например ключевые слова или категории, полностью заменят коллекцию.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Вопрос, отображаемый в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|description|String|Ответ, отображаемый в результатах поиска. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|webUrl|String|URL-ссылка Qna. Когда пользователи щелкают этот qna в результатах поиска, они перейдут на этот URL-адрес. Наследуется [от searchAnswer](../resources/search-searchAnswer.md).|
|availabilityStartDateTime|DateTimeOffset|Timestamp того, когда qna начнет отображаться в качестве результата поиска. Установите, как `null` всегда доступно.|
|availabilityEndDateTime|DateTimeOffset|Timestamp того, когда qna остановится, чтобы появиться в качестве результата поиска. Установите, как `null` всегда доступно.|
|LanguageTags|Коллекция объектов string|Список стран или регионов, которые могут просматривать этот qna.|
|платформы|коллекция microsoft.graph.devicePlatformType|Список устройств и операционных систем, которые могут просматривать этот qna. Возможные значения: `unknown`, `android`, `androidForWork`, `ios`, `macOS`, `windowsPhone81`, `windowsPhone81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidASOP`.|
|targetedVariations|[коллекция microsoft.graph.search.answerVariant](../resources/search-answerVariant.md)|Варианты QNA для разных стран или устройств. Используйте, когда необходимо показывать пользователям различные контенты на основе их устройства, страны или региона или обоих. Параметры даты и группы будут применяться для всех вариантов.|
|keywords|[microsoft.graph.search.answerKeyword](../resources/search-answerKeyword.md)|Ключевые слова, которые запускают этот qna, отображаются в результатах поиска.|
|state|microsoft.graph.search.answerState|Состояние qna. Возможные значения: `published`, , `draft`, или `excluded``unknownFutureValue`.|
|groupIds|Коллекция String|Список групп безопасности, которые могут просматривать этот qna.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_qna"
}-->
``` http
PATCH https://graph.microsoft.com/beta/search/qna/{qnaId}
Content-Type: application/json

{
    "description": "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend."
}
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}-->
``` http
HTTP/1.1 204 No Content
```

