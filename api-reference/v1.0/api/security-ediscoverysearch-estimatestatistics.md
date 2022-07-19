---
title: 'ediscoverySearch: estimateStatistics'
description: Выполняет оценку поиска обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0809dbad83052bdd6a8de830df8cb522c61ba693
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839789"
---
# <a name="ediscoverysearch-estimatestatistics"></a>ediscoverySearch: estimateStatistics
Пространство имен: microsoft.graph.security

Выполните оценку количества сообщений электронной почты и документов в поиске электронных данных. Дополнительные сведения об поисковых запросах в службе обнаружения электронных данных см. в статье "Сбор данных для дела [в службе обнаружения электронных данных (премиум)"](/microsoft-365/compliance/collecting-data-for-ediscovery).


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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/estimateStatistics
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

Если оценка успешно запущена, это действие возвращает код `202 Accepted` отклика.
Ответ также будет содержать `Location` заголовок, содержащий расположение [объекта microsoft.graph.security.estimateStatisticsOperation](../resources/security-ediscoveryestimateoperation.md) , созданного для обработки оценки. Проверьте состояние операции оценки, выполнив запрос GET к расположению.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.estimatestatistics"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/estimatestatistics
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```