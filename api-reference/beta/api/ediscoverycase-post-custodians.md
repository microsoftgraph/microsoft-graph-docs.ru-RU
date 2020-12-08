---
title: Создание хранитель
description: Создание нового объекта хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7142d00f7fdee7643e5c6c2b755c1c88a1e9f9dc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597802"
---
# <a name="create-custodian"></a>Создание хранитель

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [хранитель](../resources/custodian.md) . После создания объекта хранитель необходимо создать [усерсаурце](../resources/usersource.md) хранитель, чтобы ссылаться на свой почтовый ящик и сайт OneDrive для бизнеса.

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
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [хранитель](../resources/custodian.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [хранитель](../resources/custodian.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|email|String|Основной SMTP-адрес хранитель. Обязательно.|
|апплихолдтосаурцес|Логический|Указывает, применяется ли удержание к источникам хранитель (таким как почтовые ящики, сайты или рабочие группы).|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [хранитель](../resources/custodian.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
