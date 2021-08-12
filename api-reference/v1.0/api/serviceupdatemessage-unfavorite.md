---
title: 'serviceUpdateMessage: неблагоприятный'
description: Удалите любимый статус serviceUpdateMessage для подписанного пользователя.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 00321fdf2b03098c918ce179aeaff581ba740159d2c7cf19b0e9855525d3f4af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134537"
---
# <a name="serviceupdatemessage-unfavorite"></a>serviceUpdateMessage: неблагоприятный
Пространство имен: microsoft.graph

Удалите любимый статус [serviceUpdateMessages](../resources/serviceupdatemessage.md) для подписанного пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ServiceMessageViewpoint.Write|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/serviceAnnouncement/messages/unfavorite
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
|messageIds|Коллекция String|Список ID-сообщений, которые необходимо удалить из избранного.|

## <a name="response"></a>Отклик

В случае успеха это действие возвращает код отклика и значение `200 OK` Boolean `true` в тексте ответа. В противном случае `false` возвращается в тело ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "serviceupdatemessage_unfavorite"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/admin/serviceAnnouncement/messages/unfavorite
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
