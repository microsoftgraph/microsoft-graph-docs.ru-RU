---
title: Создание cloudPcProvisioningPolicy
description: Создайте новую политику продюсинга облачных КОМПЬЮТЕРов.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c8ceafcd70592f4f0b10e1818200021cfb7ae061
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722806"
---
# <a name="create-cloudpcprovisioningpolicy"></a>Создание cloudPcProvisioningPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|CloudPC.ReadWrite.All|

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
| Авторизация | Bearer {token}. Обязательный.  |
| Content-Type  | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) .

В следующей таблице показаны свойства, необходимые при создании [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя отображения политики обеспечения.|
|description|String|Описание политики обеспечения.|
|onPremisesConnectionId|String|ID cloudPcOnPremisesConnection. Чтобы обеспечить подключение к облачным компьютерам и подключение к домену, выберите подключение к виртуальной сети, проверенной службой облачных ПК.|
|imageId|String|ID изображения ОС, которое необходимо уладить на облачных ПК. Формат изображения типа галереи: {publisher_offer_sku}. Поддерживаемые значения для каждого из параметров:<ul><li>издатель: Microsoftwindowsdesktop.</li> <li>предложение: windows-ent-cpc.</li> <li>sku: 21h1-ent-cpc-m365, 21h1-ent-cpc-os, 20h2-ent-cpc-m365, 20h2-ent-cpc-os, 20h1-ent-cpc-m365, 20h1-ent-cpc-os, 19h2-ent-cpc-os.</li></ul>|
|imageDisplayName|String|Имя отображения образа ОС, которое вы закаповыватель.|
|imageType|cloudPcProvisioningPolicyImageType|Тип изображения ОС (настраиваемый или галерейный) для предоставления на облачных ПК. Возможные значения: `gallery`, `custom`.|
|WindowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Определенные Windows настройки при создании облачных компьютеров для этой политики обеспечения.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код `201 Created` отклика и [объект cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) в тексте ответа.

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

{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "description": "Description value",
    "displayName": "Display Name value",
    "domainJoinConfiguration": {
        "domainJoinType": "hybridAzureADJoin",
        "onPremisesConnectionId": "16ee6c71-fc10-438b-88ac-daa1ccafffff"
    },
    "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
    "imageDisplayName": "Windows-10 19h1-evd",
    "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
    "imageType":"gallery",
    "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
    "windowsSettings": {
        "language": "en-US"
    }
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-powershell-snippets.md)]
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

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "domainJoinConfiguration": {
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "type": "hybridAzureADJoin"
  },
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "imageDisplayName": "Windows-10 19h1-evd",
  "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
  "imageType":"gallery",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "windowsSettings": {
    "language": "en-US"
  }
}
```
