---
title: Создание Ситесаурце
description: Создание нового объекта Ситесаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 93cb37a6ff94a52830675f876084fc85a6365a40
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597755"
---
# <a name="create-sitesource"></a>Создание Ситесаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [ситесаурце](../resources/sitesource.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|User.Read|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [ситесаурце](../resources/sitesource.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [ситесаурце](../resources/sitesource.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|site@odata. Bind|String|Идентификатор сайта, который можно получить из ресурса [сайта](../resources/site.md) с помощью метода [получения ресурса сайта по пути](../api/site-getbypath.md) . Использование: {hostname}:/{релативе-Пас}. Для URL-адреса сайта `https://contoso.sharepoint.com/sites/HumanResources` запрос Microsoft Graph будет иметь значение `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources` . Идентификатор является первым идентификатором GUID, указанным в поле ID.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ситесаурце](../resources/sitesource.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_sitesource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
Content-Type: application/json
Content-length: 179

{
    "site@odata.bind": "https://graph.microsoft.com/v1.0/sites/{siteId}"
}
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Human resources site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
