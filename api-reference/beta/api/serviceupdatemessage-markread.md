---
title: 'serviceUpdateMessage: markRead'
description: Пометить список сообщений об обновлении службы в качестве чтения для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 87cddaecbab5dc361f9a2601c7dd38806840406f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107828"
---
# <a name="serviceupdatemessage-markread"></a>serviceUpdateMessage: markRead
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пометить список [serviceUpdateMessages](../resources/serviceupdatemessage.md) в качестве чтения для подписанного пользователя. 

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|ServiceMessageViewpoint.Write|
|Делегированное (личная учетная запись Майкрософт)|ServiceMessageViewpoint.Write|
|Для приложений|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/markRead
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|messageIds|Набор строк|Список ID-сообщений, которые необходимо отметить как чтение.|


## <a name="response"></a>Отклик

В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа. В противном случае `false` возвращается в тело ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_markread"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/markRead
Content-Type: application/json

{
  "messageIds": ["MC172851", "MC167983"]
}
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": true
}
```