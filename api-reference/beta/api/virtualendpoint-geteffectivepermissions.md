---
title: 'Виртуалендпоинт: getEffectivePermissions'
description: '**GetEffectivePermissions — это функция, которая ретривес действующие разрешения пользователя, прошедшего проверку подлинности, что позволяет скрыть или отключить контент, к которому у текущего пользователя нет доступа.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b58c5ea00e1b170d831a91f5dc3ff1569bd0d7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378626"
---
# <a name="virtualendpoint-geteffectivepermissions"></a>Виртуалендпоинт: getEffectivePermissions

Пространство имен: microsoft.graph

Просмотр действующих разрешений текущего пользователя, прошедшего проверку подлинности. GetEffectivePermissions — это функция, которая ретривес действующие разрешения пользователя, прошедшего проверку подлинности, что позволяет скрыть или отключить контент, к которому у текущего пользователя нет доступа.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL|
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.|
|Для приложений| Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика. Если у пользователя есть полные разрешения, ответ — `["*"]` .

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    "Microsoft.CloudPC/CloudPCs/Read"
  ]
}
```
