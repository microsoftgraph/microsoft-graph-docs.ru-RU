---
title: Создание cloudPcProvisioningPolicy
description: Создайте новую политику предоставления облачных компьютеров.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a83b156808fd0c9634fc8c7fedf62a6c9b8a2996
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874076"
---
# <a name="create-cloudpcprovisioningpolicy"></a>Создание cloudPcProvisioningPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
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

## <a name="request-body"></a>Основной текст запроса

В теле запроса укажу представление объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в JSON.

В следующей таблице показаны свойства, необходимые при создании [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемого имени для политики предоставления.|
|description|String|Описание политики предоставления.|
|onPremisesConnectionId|String|ИД cloudPcOnPremisesConnection. Чтобы убедиться, что облачные компьютеры имеют сетевое подключение и присоединяются к домену, выберите подключение к виртуальной сети, проверяемой службой облачных КОМПЬЮТЕРов.|
|imageId|String|ИД образа ОС, который вы хотите получить на облачных ПК. Формат изображения типа коллекции: {publisher_offer_sku}.|
|imageDisplayName|String|Отображаемая имя для образа ОПЕРАЦИОННОй системы, который вы хотите демонстрировать.|
|imageType|cloudPcProvisioningPolicyImageType|Тип образа ОС (настраиваемого или галереи), который необходимо настроить на облачных ПК. Возможные значения: `gallery`, `custom`.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и объект `201 Created` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте отклика.

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
