---
title: Создание политики
description: Создание нового объекта политики, указав отображаемое имя, тип политики и описание политики.
localization_priority: Normal
ms.openlocfilehash: 4850b2899bfd9add703af912f16602960b2657f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831236"
---
# <a name="create-policy"></a>Создание политики

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Создание нового объекта [политики](../resources/policy.md) , указав отображаемое имя, тип политики и описание политики.

>Примечание: Сведения о политике проверяются перед сохранением. Если он не пройдет проверку, 400 Неверный запрос будут возвращены.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

```http
POST /policies
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type | application/json  | Характер данных в теле объекта. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса для представления JSON объекта [политики](../resources/policy.md) .

В следующей таблице приведены свойства, необходимых при создании политики.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|definition|Строка|Строковая версия объекта [политики](../resources/policy.md) .|
|displayName|Строка|Пользовательское имя для политики.|
|type|Строка|Указывает тип политики. В настоящее время должен быть «TokenLifetimePolicy»|

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `201 Created` ответа кода и [политики](../resources/policy.md) объекта в теле ответа. В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.  

## <a name="example"></a>Пример
В следующем примере создается новый срока жизни маркера политики. Обратите внимание на то, что параметр определения строки escape-двойные кавычки.

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
