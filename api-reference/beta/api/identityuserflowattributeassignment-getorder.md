---
title: 'Идентитюсерфловаттрибутеассигнмент: упорядочение'
description: Получение порядка Идентитюсерфловаттрибутеассигнментс, собранных в пользовательском движении.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 653a1e83ee96418dc70129790f62ea764e6326f9
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581427"
---
# <a name="identityuserflowattributeassignment-getorder"></a>Идентитюсерфловаттрибутеассигнмент: упорядочение

Пространство имен: microsoft.graph

Получение порядка Идентитюсерфловаттрибутеассигнментс, собранных в пользовательском движении.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/getOrder
GET /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/getOrder
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="function-parameters"></a>Параметры функции

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха эта функция возвращает `200 OK` код отклика и объект [ассигнментордер](../resources/assignmentorder.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_getorder"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta$metadata#microsoft.graph.assignmentOrder",
    "order": [
        "extension_GUID_ShoeSize",
        "City"
    ]
}
```
