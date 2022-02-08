---
title: 'crossTenantAccessPolicyConfigurationDefault: resetToSystemDefault'
description: 'Сброс любых изменений, внесенных в конфигурацию по умолчанию в политике межзаймного доступа к системе по умолчанию.'
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
---

# <a name="crosstenantaccesspolicyconfigurationdefault-resettosystemdefault"></a>crossTenantAccessPolicyConfigurationDefault: resetToSystemDefault

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сброс любых изменений, внесенных в конфигурацию по умолчанию в политике межзаймного доступа к системе по умолчанию.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.CrossTenantAccess|
|Делегированные (личная учетная запись Майкрософт)|Неприменимо|
|Приложение|Policy.ReadWrite.CrossTenantAccess|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /policies/crossTenantAccessPolicy/default/resetToSystemDefault
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного действия возвращается код `200 OK` ответа и пустой ответ. Чтобы подтвердить, что конфигурация по умолчанию восстановлена в системе по умолчанию, запустите [Get crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md) и подтвердите, что **значение isSystemDefault** `true`установлено .

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "crosstenantaccesspolicyconfigurationdefault_resettosystemdefault"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/default/resetToSystemDefault
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.crossTenantAccessPolicyConfigurationDefault"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

}
```
