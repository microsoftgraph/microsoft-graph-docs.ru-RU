---
title: Создание cloudPcOnPremisesConnection
description: Создание сетевого подключения Azure для создания облачных компьютеров.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: f541ae5a05ae79507cb042ad6685bbe25754eef8
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589368"
---
# <a name="create-cloudpconpremisesconnection"></a>Создание cloudPcOnPremisesConnection

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) для создания облачных компьютеров.

[!INCLUDE [on-premise-rename-note](../../includes/on-premise-rename-note.md)]

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
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                |
| :------------ | :------------------------  |
| Авторизация | Bearer {token}. Обязательный.  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) .

В следующей таблице показаны свойства, необходимые при создании [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения для сетевого подключения Azure.|
|type|cloudPcOnPremisesConnectionType|Указывает, как будет присоединяться к Azure Active Directory. Значение по умолчанию — `hybridAzureADJoin`. Возможные значения: `azureADJoin`, `hybridAzureADJoin`, `unknownFutureValue`.|
|subscriptionId|Строка|ID целевой подписки Azure, связанной с клиентом.|
|adDomainName|Строка|Полное доменное имя домена (FQDN) домена Active Directory, к нему необходимо присоединиться.|
|adDomainUsername|String|Имя пользователя учетной записи Active Directory (учетная запись пользователя или службы), которая имеет разрешения на создание компьютерных объектов в Active Directory. Необходимый формат: admin@contoso.com.|
|adDomainPassword|String|Пароль, связанный с adDomainUsername.|
|resourceGroupId|Строка|ID целевой группы ресурсов. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".|
|virtualNetworkId|Строка|ID целевой виртуальной сети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".|
|subnetId|Строка|ID целевой подсети. Необходимый формат: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `201 Created` ответа и [объект cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpconpremisesconnection_from_cloudpconpremisesconnection"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "displayName": "test-canary-02",
  "type": "hybridAzureADJoin",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "CPC customer 001 test subscription",
  "adDomainName": "contoso001.com",
  "adDomainUsername": "dcadmin",
  "organizationalUnit": "OU=Domain Controllers, DC=contoso001, DC=com",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "ac2ad805-167e-49ee-9bef-196c4ce7ffff",
  "managedBy": "windows365",
  "displayName": "test-canary-02",
  "type": "hybridAzureADJoin",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "CPC customer 001 test subscription",
  "adDomainName": "contoso001.com",
  "adDomainUsername": "dcadmin",
  "organizationalUnit": "OU=Domain Controllers, DC=contoso001, DC=com",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet",
  "healthCheckStatus": "pending"
}
```
