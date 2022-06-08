---
title: Обновление ediscoverySearch
description: Обновление свойств объекта ediscoverySearch.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 981e9098695789fee2bf60ff8466d2b7c5a411c6
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946188"
---
# <a name="update-ediscoverysearch"></a>Обновление ediscoverySearch
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [ediscoverySearch](../resources/security-ediscoverysearch.md) .

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
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|contentQuery|Строка|Строка запроса в запросе KQL (язык запросов ключевых слов). Дополнительные сведения см. в [запросах по ключевым словам и условиях поиска для поиска контента и обнаружения электронных данных](/microsoft-365/compliance/keyword-queries-and-search-conditions).  Поиск можно уточнить с помощью полей, связанных со значениями; Например, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.|
|dataSourceScopes|dataSourceScopes|Если этот параметр указан, коллекция будет охватывать всю службу для всей рабочей нагрузки. Возможные значения: `none`,`allTenantMailboxes`,,`allTenantSites``allCaseCustodians`,`allCaseNoncustodialDataSources`. **Примечание:** При создании исходной коллекции требуется один хранителя или указание dataSourceScope.|
|description|Строка|Описание поиска **eDiscovery**.|
|displayName|Строка|Отображаемое имя поиска **eDiscovery**.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `204 No Content` код отклика и обновленный [объект ediscoverySearch](../resources/security-ediscoverysearch.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_ediscoverysearch"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}
Content-Type: application/json

{
    "displayName": "Teams search"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```