---
title: Создание Клаудпкпровисионингполици
description: Создайте новую политику подготовки облачных ПК.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 45410405c88d7bb8a3e8de544e40279af490386a
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563879"
---
# <a name="create-cloudpcprovisioningpolicy"></a>Создание Клаудпкпровисионингполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Клаудпк. ReadWrite. ALL|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                |
| :------------ | :------------------------  |
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики подготовки.|
|description|String|Описание политики подготовки.|
|онпремисесконнектионид|String|Идентификатор Клаудпконпремисесконнектион. Чтобы обеспечить сетевое подключение к облачным компьютерам и присоединение к домену, выберите подключение с виртуальной сетью, проверенной службой Cloud PC.|
|имажеид|String|Идентификатор образа ОС, который вы хотите подготовить к работе на облачных компьютерах. Формат изображения для типа галереи: {publisher_offer_sku}.|
|имажедисплайнаме|String|Отображаемое имя для образа ОС, который вы собираетесь заготовить.|
|имажетипе|клаудпкпровисионингполициимажетипе|Тип образа ОС (настраиваемого или галереи), который необходимо подготовить к работе на облачных компьютерах. Возможные значения: `gallery`, `custom`.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "gallery"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
  }
```
