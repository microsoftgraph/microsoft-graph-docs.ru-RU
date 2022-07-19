---
title: 'ediscoveryNoncustodialDataSource: removeHold'
description: Запустите процесс удаления удержания из источников данных, не охраняемых при обнаружении электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 46a7e70f79be000907b59d9858a28b150e9a1158
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839818"
---
# <a name="ediscoverynoncustodialdatasource-removehold"></a>ediscoveryNoncustodialDataSource: removeHold
Пространство имен: microsoft.graph.security



Запустите процесс удаления удержания из источников данных [, не охраняемых при обнаружении электронных данных](../resources/security-ediscoverynoncustodialdatasource.md). После создания операции можно получить `Location` состояние, извлекая параметр из заголовков ответа. Расположение содержит URL-адрес, возвращающий объект [eDiscoveryHoldOperation](../resources/security-ediscoveryholdoperation.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/removeHold
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/{ediscoverynoncustodialDatasourceId}/removeHold
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
|ids|Коллекция String|Идентификаторы источников данных, не хранимых для удаления удержания. Необязательный параметр.|



## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

## <a name="examples"></a>Примеры

### <a name="example-1-remove-hold-from-multiple-non-custodial-data-sources"></a>Пример 1. Удаление удержания из нескольких источников данных, которые не являются хранителями
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/removeHold
Content-Type: application/json

{
    "ids": [
        "39333641443238353535383731453339",
        "46333131344239353834433430454335"
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

### <a name="example-2-remove-hold-from-a-single-non-custodial-data-source"></a>Пример 2. Удаление удержания из одного источника данных, не являемой хранителями
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/39333641443238353535383731453339/removeHold
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
