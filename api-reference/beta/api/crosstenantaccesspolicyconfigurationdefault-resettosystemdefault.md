---
title: 'crossTenantAccessPolicyConfigurationDefault: resetToSystemDefault'
description: Сброс любых изменений, внесенных в конфигурацию по умолчанию в политике межзаймного доступа к системе по умолчанию.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 22a2b3914d4a526c57146cf395d8255435199f5f
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804425"
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

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `204 No Content`. Чтобы подтвердить, что конфигурация по умолчанию восстановлена в системе по умолчанию, запустите [Get crossTenantAccessPolicyConfigurationDefault](../api/crosstenantaccesspolicyconfigurationdefault-get.md) и подтвердите, что **значение isSystemDefault** `true`установлено .

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
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
