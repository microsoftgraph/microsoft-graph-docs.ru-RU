---
title: 'ediscoveryCustodian: removeHold'
description: '**ЗАДАЧА: добавить описание**'
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 4069641d0079d450b6370d47167e6e49872f0f66
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839866"
---
# <a name="ediscoverycustodian-removehold"></a>ediscoveryCustodian: removeHold
Пространство имен: microsoft.graph.security

Запустите процесс удаления удержания у хранителей [обнаружения электронных данных](../resources/security-ediscoverycustodian.md). После создания операции можно получить `Location` состояние, извлекая параметр из заголовков ответа. Расположение содержит URL-адрес, возвращающий объект [eDiscoveryHoldOperation](../resources/security-ediscoveryholdoperation.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/removeHold
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{eDiscoveryCustodianId}/removeHold
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|ids|Коллекция String|Идентификаторы хранителей для применения удержания. Необязательный параметр.|


## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры
### <a name="example-1-remove-hold-from-multiple-custodians"></a>Пример 1. Удаление удержания нескольких хранителей
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/removeHold
Content-Type: application/json

{
  "ids": [
    "7f697316-43ed-48e1-977f-261be050db93", "b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8"
  ]
}
```


#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

### <a name="example-2-remove-hold-from-a-single-custodian"></a>Пример 2. Удаление удержания одного хранителя
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/c25c3914f9f743ee9cbaa25377e0cec6/removeHold
```


#### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```