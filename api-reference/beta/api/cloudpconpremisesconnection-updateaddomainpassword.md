---
title: 'cloudPcOnPremisesConnection: updateAdDomainPassword'
description: Обновление пароля домена Active Directory для успешного локального подключения. Этот API поддерживается, когда тип onPremisesConnection является hybridAzureADJoin.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3a2f518821eb7825146450dc6aaf2da00e39dd36
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266315"
---
# <a name="cloudpconpremisesconnection-updateaddomainpassword"></a>cloudPcOnPremisesConnection: updateAdDomainPassword
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление пароля домена Active Directory для [onPremisesConnection](../resources/cloudpconpremisesconnection.md). Этот API поддерживается при типе **onPremisesConnection** `hybridAzureADJoin` .


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|adDomainPassword|Строка|Пароль, связанный с **adDomainUsername**.|



## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpconpremisesconnection_updateaddomainpassword"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{Id}/UpdateAdDomainPassword
Content-Type: application/json

{
  "adDomainPassword": "AdDomainPassword value"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpconpremisesconnection-updateaddomainpassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpconpremisesconnection-updateaddomainpassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/cloudpconpremisesconnection-updateaddomainpassword-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
