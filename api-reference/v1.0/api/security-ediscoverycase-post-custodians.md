---
title: Создание хранителей
description: Создайте объект ediscoveryCustodian.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: db69f0db35ad1e5b6910d15f73984d32be73e7cc
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839728"
---
# <a name="create-custodians"></a>Создание хранителей
Пространство имен: microsoft.graph.security



Создайте объект [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .
После создания объекта хранителя необходимо создать [userSource](../resources/security-usersource.md) хранителя, чтобы ссылаться на его почтовый ящик и OneDrive для бизнеса сайте.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) в формате JSON.

При создании объекта **ediscoveryCustodian можно указать следующие свойства**.

|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|Основной SMTP-адрес хранителя. Обязательный.|

## <a name="response"></a>Отклик

В случае успешного выполнения `201 Created` этот метод возвращает код отклика и объект [microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_ediscoverycustodian_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians
Content-Type: application/json

{
    "email":"AdeleV@contoso.com",
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryCustodian"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
     "status": "active",
     "holdStatus": "applied",
     "createdDateTime": "2022-05-23T00:58:19.0702426Z",
     "lastModifiedDateTime": "2022-05-23T00:58:19.0702436Z",
     "releasedDateTime": null,
     "id": "0053a61a3b6c42738f7606791716a22a",
     "displayName": "Adele Vance",
     "email": "AdeleV@contoso.com",
     "acknowledgedDateTime": "0001-01-01T00:00:00Z"
}
```