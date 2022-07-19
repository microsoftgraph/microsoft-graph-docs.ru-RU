---
title: Добавление дополнительных источников
description: Создайте новый дополнительный источник, связанный с поиском обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 99a910cfd87bc58f60ea7a79e64ebae6bb42c6a2
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66840197"
---
# <a name="add-additional-sources"></a>Добавление дополнительных источников
Пространство имен: microsoft.graph.security


Создайте новый [дополнительный источник,](../resources/security-datasource.md) связанный с поиском [обнаружения электронных данных](../resources/security-ediscoverysearch.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [dataSource](../resources/security-datasource.md) в формате JSON.

При создании источника данных можно указать следующие **свойства**.

>**Примечание:** Требуется **либо адрес электронной** **почты** , либо сайт, но не оба. 

|Свойство|Тип|Описание|
|:---|:---|:---|
|email|строка|SMTP-адрес почтового ящика. Чтобы получить адрес электронной почты группы, используйте группы [list или](../api/group-list.md) [Get](../api/group-get.md). Можно выполнить запрос по имени группы, используя `$filter`, например, `https://graph.microsoft.com/v1.0/groups?$filter=displayName eq 'secret group'&$select=mail,id,displayName`.|
|site|Строка|URL-адрес сайта; Например, `https://contoso.sharepoint.com/sites/HumanResources`. |


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает объект `201 Created` [microsoft.graph.security.dataSource](../resources/security-ediscoverysearch.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_datasource_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources

{
    "@odata.type": "microsoft.graph.security.siteSource",
    "site": {
        "webUrl": "https://contoso.sharepoint.com/sites/SecretSite"
    }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.dataSource"
}
-->
``` http
HTTP/1.1 201 Created

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches('c61a5860-d634-4d14-aea7-d82b6f4eb7af')/additionalSources/$entity",
    "@odata.type": "#microsoft.graph.security.siteSource",
    "@odata.id": "https://graph.microsoft.com/v1.0/sites/46303732-3434-4630-3832-363333363441",
    "displayName": "Design - top secret",
    "createdDateTime": "2022-07-15T22:45:36.1096267Z",
    "holdStatus": "0",
    "id": "46303732-3434-4630-3832-363333363441",
    "createdBy": {
        "application": null,
        "user": {
            "id": null,
            "displayName": null
        }
    }
}
```
