---
title: Обновление букингсервице
description: Обновление свойств объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 607949e8c4b00230815fa8b29eba751494efb8b3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636011"
---
# <a name="update-bookingservice"></a>Обновление букингсервице

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).

Ниже приведено несколько примеров, которые можно настроить для службы.
- ЦЕНА
- Типичная длительность встречи
- Reminders
- Любой буфер, который должен быть настроен до или окончание срока выполнения службы
- [Планирование](../resources/bookingschedulingpolicy.md) таких параметров политики, как минимальное уведомление о книге или Отмена, а также возможность выбора определенных сотрудников для встречи пользователями.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Резервирования. ReadWrite. ALL, Books. Manage. ALL   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Дефаултдуратион|Duration (Длительность)|Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд. Например, P11D23H59M 59.999999999999 S. |
|defaultLocation|[location](../resources/location.md)|Физическое расположение службы по умолчанию.|
|Дефаултприце|Двойное|Денежная Цена по умолчанию для службы.|
|Дефаултприцетипе|string|Способ оплаты службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|Дефаултреминдерс|Коллекция [букингреминдер](../resources/bookingreminder.md)|Набор напоминаний по умолчанию для встречи этой службы. Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.|
|description|String|Текстовое описание службы.|
|displayName|Строка|Имя службы.|
|emailAddress|String|Адрес электронной почты|
|id|String| Только для чтения.|
|Ишидденфромкустомерс|Логический|Значение true означает, что эта служба недоступна клиентам для резервирования.|
|notes|String|Дополнительные сведения об этой службе.|
|Буфер буфера|Duration (Длительность)|Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.|
|пребуфер|Duration (Длительность)|Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.|
|Счедулингполици|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.|
|Стаффмемберидс|Коллекция String|Представляет [сотрудников](../resources/bookingstaffmember.md) , которые предоставляют эту службу. |

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере обновляется длительность указанной службы.
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingservice-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingservice-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
