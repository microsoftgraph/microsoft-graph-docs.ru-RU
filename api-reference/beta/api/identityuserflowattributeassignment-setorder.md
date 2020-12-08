---
title: 'Идентитюсерфловаттрибутеассигнмент: Сетордер'
description: Задайте порядок Идентитюсерфловаттрибутеассигнментс, собираемых в рамках пользовательского процесса.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 705acf8e65d7d01c40d98860c6f5066121d23a81
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581428"
---
# <a name="identityuserflowattributeassignment-setorder"></a>Идентитюсерфловаттрибутеассигнмент: Сетордер

Пространство имен: microsoft.graph

Задайте порядок Идентитюсерфловаттрибутеассигнментс, собираемых в рамках пользовательского процесса.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|Идентитюсерфлов. ReadWrite. ALL|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Идентитюсерфлов. ReadWrite. ALL|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/setOrder
POST /identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/setOrder
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|невассигнментордер|[ассигнментордер](../resources/assignmentorder.md)|Используется для определения порядка атрибутов, собранных в пользовательском движении.|

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "identityuserflowattributeassignment_setorder"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder

Content-Type: application/json
Content-length: 90

{
  "newAssignmentOrder": {
    "order": [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
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
```
