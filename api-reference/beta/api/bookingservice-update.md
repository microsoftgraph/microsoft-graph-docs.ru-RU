---
title: Обновление bookingservice
description: Обновите свойства объекта bookingService в указанном bookingbusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 674221dd3195ed136230e64496f1a2af50041397
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160463"
---
# <a name="update-bookingservice"></a>Обновление bookingservice

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойства объекта [bookingService](../resources/bookingservice.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).

Ниже приведены некоторые примеры, которые можно настроить для службы.
- ЦЕНА
- Типичная длина встречи
- Reminders
- Любой буфер времени для настройки до или после завершения службы
- [Параметры политики](../resources/bookingschedulingpolicy.md) планирования, такие как минимальное уведомление для резервирования или отмены, а также возможность выбора клиентами определенных сотрудников для встречи.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Носитель {code}. Обязательно.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|defaultDuration|Длительность|Длина службы по умолчанию, представленная в числах дней, часов, минут и секунд. Например, P11D23H59M59.999999999999S. |
|defaultLocation|[location](../resources/location.md)|Физическое расположение службы по умолчанию.|
|defaultPrice|Двойное с плавающей точкой|Денежное значение по умолчанию для службы.|
|defaultPriceType|bookingPriceType|Способ оплаты службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|defaultReminders|[Коллекция bookingReminder](../resources/bookingreminder.md)|Набор напоминаний по умолчанию для встречи этой службы. Значение этого свойства доступно только при чтении этой **службы bookingService** по его идентификатору.|
|description|Строка|Текстовое описание службы.|
|displayName|Строка|Имя службы.|
|id|String| Только для чтения.|
|languageTag|Строка|Язык страницы самостоятельного резервирования.|
|isHiddenFromCustomers|Boolean|Значение true означает, что эта служба недоступна клиентам для резервирования.|
|isLocationOnline|Boolean|Значение true указывает, что встречи для службы будут храниться в сети. Значение по умолчанию − ложь.|
|notes|String|Дополнительные сведения об этой службе.|
|postBuffer|Длительность|Время буферизации после окончания встречи для этой службы и до того, как можно будет заказать следующую встречу клиента.|
|preBuffer|Длительность|Время буферизации до начала встречи для этой службы.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Набор политик, определяющий способ создания и управления встречами для этого типа службы.|
|smsNotificationsEnabled|Boolean|Значение true SMS, что клиенты могут отправлять уведомления о встрече службы. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|Представляет сотрудников [, предоставляющих](../resources/bookingstaffmember.md) эту службу. |
|customQuestions|[Коллекция bookingQuestionAssignment](../resources/bookingquestionassignment.md)|Он содержит набор пользовательских вопросов, связанных с определенной службой. Необязательно.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных в службе.  |

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере обновляется длительность указанной службы.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingservice-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingservice-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->


