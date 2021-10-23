---
title: Обновление externalConnection
description: Обновление свойств объекта externalConnection.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c418efb3794cb30040b59211be741bd14ad7d306
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559269"
---
# <a name="update-externalconnection"></a>Обновление externalConnection

Пространство имен: microsoft.graph.externalConnectors

Обновление свойств объекта [externalConnection.](../resources/externalconnectors-externalconnection.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Application                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /external/connections/{connectionsId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. Могут быть обновлены перечисленные ниже свойства.

| Свойство      | Тип                                           | Описание |
|:--------------|:-----------------------------------------------|:------------|
| configuration | [microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md) | Указывает дополнительные ID-адреса приложений, которые разрешены для управления подключением и индексации контента в подключении. |
| description   | Строка                                         | Описание подключения, отображаемого в Центр администрирования Microsoft 365. |
| name          | String                                         | Отображает имя подключения, отображаемого в Центр администрирования Microsoft 365. Максимальная длина 128 символов. |


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


<!-- {
  "blockType": "request",
  "name": "update_externalconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/external/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
