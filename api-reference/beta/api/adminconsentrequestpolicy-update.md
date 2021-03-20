---
title: Обновление adminConsentRequestPolicy
description: Обновление свойств объекта adminConsentRequestPolicy.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1c0769262cc17e79448ca856e26334d4c03d92a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952309"
---
# <a name="update-adminconsentrequestpolicy"></a>Обновление adminConsentRequestPolicy
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.ConsentRequest|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|Policy.ReadWrite.ConsentRequest|

При вызове от имени пользователя пользователю необходимо принадлежать к роли [глобального](/azure/active-directory/roles/permissions-reference) администратора.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy 
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)

В следующей таблице показаны свойства, необходимые при обновлении [администрированияConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена или отключена функция запроса на согласие администратора.|
|notifyReviewers|Boolean|Указывает, будут ли рецензенты получать уведомления.|
|remindersEnabled|Boolean|Указывает, будут ли рецензенты получать сообщения напоминания.|
|requestDurationInDays|Int32|Указывает продолжительность действия запроса до его автоматического истечения, если не будет применено решение.|
|рецензенты|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Список рецензентов для согласия администратора.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: text/plain
```
