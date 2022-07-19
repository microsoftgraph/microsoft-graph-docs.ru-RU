---
title: 'ediscoveryCustodian: activate'
description: Повторно активируйте хранителя из дела.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 8208d98c9047966c8331f5f7f9212f46a426ee6d
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839963"
---
# <a name="ediscoverycustodian-activate"></a>ediscoveryCustodian: activate
Пространство имен: microsoft.graph.security



Активируйте хранителя, освобожденного из дела, чтобы снова сделать его частью дела. Дополнительные сведения см. в [разделе "Управление хранителями" дела об обнаружении электронных данных (premium](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian)).


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{ediscoveryCustodianId}/activate
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.activate"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{ediscoveryCustodianId}/activate
```
### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```