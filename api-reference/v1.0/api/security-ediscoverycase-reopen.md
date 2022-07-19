---
title: Повторное открытие eDiscoveryCase
description: Повторно откройте закрытый eDiscoveryCase.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2888d36b46d367dcdb79ecf8372e9138170daba7
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839710"
---
# <a name="ediscoverycase-reopen"></a>eDiscoveryCase: повторное открытие

Пространство имен: microsoft.graph.security



Повторно откройте дело обнаружения электронных данных, которое было закрыто. Дополнительные сведения см. в [разделе "Повторное открытие закрытого дела"](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/reopen
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "reopen_ediscoverycase"
}
-->
``` http
POST https://graph.microsoft.com/security/cases/eDiscoveryCases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
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
