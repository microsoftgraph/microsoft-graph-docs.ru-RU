---
title: 'ediscoveryExportOperation: getDownloadUrl'
description: возвращает downloadUrl, откуда экспортированное содержимое доставляется в виде потока.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7a990c67b5b444bc1d6b7db04c6e2035763e6363
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838096"
---
# <a name="ediscoveryexportoperation-getdownloadurl"></a>ediscoveryExportOperation: getDownloadUrl
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Если URL-адрес большого двоичного объекта Azure не указан в действии экспорта, операция экспорта экспортирует файлы во внутреннее хранилище. Содержимое этого хранилища можно получить, вызвав эту функцию. Это возвратит downloadUrl, куда zippped-содержимое доставляется в виде потока.


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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/operations/{eDiscoveryCaseOperationId}/microsoft.graph.security.ediscoveryExportOperation/getDownloadUrl
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения эта функция возвращает код `200 OK` отклика и строку в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoveryexportoperationthis.getdownloadurl"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/ediscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/operations/c5ae226f457547a582ef0eb6dbfaee25/microsoft.graph.security.ediscoveryExportOperation/getDownloadUrl
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.String"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: text/plain

{
    "https://sdfpkgg0021.blob.edproxy.aed01.ediscovery.outlook.com/packaging120g37c10016472cb0abf28fac5800b0/6dec1a1c-0577-424f-819c-9542edc47f5a.zip?{SASToken}"
}
```

