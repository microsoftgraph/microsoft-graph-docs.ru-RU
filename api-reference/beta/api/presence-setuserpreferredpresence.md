---
title: 'присутствие: setUserPreferredPresence'
description: Настройка предпочитаемого пользователем присутствия для пользователя
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: f2edf4fd85c9bad4d2ee8b7a703a19340328c086
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391182"
---
# <a name="presence-setuserpreferredpresence"></a>присутствие: setUserPreferredPresence

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Установите предпочтительное состояние доступности и активности для пользователя. Если установлено предпочтительное присутствие пользователя, его присутствие является предпочтительным.

Предпочтительное присутствие вступает в силу только при наличии хотя бы [одного](presence-setpresence.md#presence-sessions) сеанса присутствия пользователя. В противном случае присутствие пользователя остается в автономном режиме.

Сеанс присутствия может быть создан в результате успешной операции [setPresence](presence-setpresence.md) или если пользователь подписан на Teams клиента. 

Дополнительные новости о [сеансах присутствия](presence-setpresence.md#presence-sessions) и [их времени ожидания и истечения срока действия.](presence-setpresence.md#timeout-expiration-and-keep-alive) 

## <a name="permissions"></a>Разрешения
Для вызова API требуется следующее разрешение. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Presence.ReadWrite                          |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setUserPreferredPresence
```
## <a name="request-headers"></a>Заголовки запроса
| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр          | Тип     | Описание                                                                                                                                                                                                                                    |
| :----------------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| availability       | String   | Сведения о базовом присутствии.                                                                                                                                                                                                                 |
| действие           | String   | Дополнительные сведения о доступности.                                                                                                                                                                                                  |
| expirationDuration | duration | Срок действия сеанса присутствия приложения. Значение представлено в формате ISO 8601 для длительности.<br/>В случае невыполнения условий по умолчанию будет применено:<br/>DoNotDisturb или Busy: срок действия истекает через 1 день<br/>Все остальные: срок действия истекает через 7 дней |

Поддерживаемые сочетания **доступности** и **активности:**

| availability | действие     | Описание                                         |
| :----------- | :----------- | :-------------------------------------------------- |
| Доступно    | Доступно    | Установите предпочтительное присутствие пользователя как доступное.       |
| Занята         | Занята         | Установите предпочтительное для пользователя присутствие как Busy.            |
| DoNotDisturb | DoNotDisturb | Установите предпочтительное присутствие пользователя как DoNotDisturb.    |
| BeRightBack  | BeRightBack  | Установите предпочтительное присутствие пользователя как BeRightBack.     |
| Away         | Away         | Установите предпочтительное для пользователя присутствие как Away.            |
| Автономный режим      | OffWork      | Установите предпочтительное для пользователя присутствие в автономном режиме. |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры

Следующий запрос задает пользователю предпочтительное присутствие в качестве DoNotDisturb для пользователя `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` с истечением 8 часов.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "setUserPreferredPresence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setUserPreferredPresence
Content-Type: application/json

{
  "availability": "DoNotDisturb",
  "activity": "DoNotDisturb",
  "expirationDuration": "PT8H"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
