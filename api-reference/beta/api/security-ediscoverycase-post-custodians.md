---
title: Создание объекта ediscoveryCustodian
description: Создайте объект ediscoveryCustodian.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8732969c2ed71b6eb1e043a56ce254bdbb7a0af9
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946224"
---
# <a name="create-ediscoverycustodian"></a>Создание объекта ediscoveryCustodian
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .
После создания объекта хранителя необходимо создать [userSource](../resources/security-usersource.md) хранителя для ссылки на его почтовый ящик и сайт OneDrive для бизнеса.

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

При создании **ediscoveryCustodian** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|Основной SMTP-адрес хранителя. Обязательный.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и [объект ediscoveryCustodian](../resources/security-ediscoverycustodian.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_ediscoverycustodian_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians
Content-Type: application/json

{
    "email":"AdeleV@contoso.com",
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
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