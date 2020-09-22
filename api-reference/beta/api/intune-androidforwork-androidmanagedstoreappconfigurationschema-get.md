---
title: Получение Андроидманажедстореаппконфигуратионсчема
description: Чтение свойств и связей объекта Андроидманажедстореаппконфигуратионсчема.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15d8082a6c9418f01e0673bbbd2d349fbf272862
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012497"
---
# <a name="get-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="d313b-103">Получение Андроидманажедстореаппконфигуратионсчема</span><span class="sxs-lookup"><span data-stu-id="d313b-103">Get androidManagedStoreAppConfigurationSchema</span></span>

<span data-ttu-id="d313b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d313b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d313b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d313b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d313b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d313b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d313b-107">Чтение свойств и связей объекта [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="d313b-107">Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d313b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d313b-108">Prerequisites</span></span>
<span data-ttu-id="d313b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d313b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d313b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d313b-111">Permission type</span></span>|<span data-ttu-id="d313b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d313b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d313b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d313b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d313b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d313b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d313b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d313b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d313b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d313b-116">Not supported.</span></span>|
|<span data-ttu-id="d313b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d313b-117">Application</span></span>|<span data-ttu-id="d313b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d313b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d313b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d313b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d313b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d313b-120">Optional query parameters</span></span>
<span data-ttu-id="d313b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d313b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d313b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d313b-122">Request headers</span></span>
|<span data-ttu-id="d313b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d313b-123">Header</span></span>|<span data-ttu-id="d313b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d313b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d313b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d313b-125">Authorization</span></span>|<span data-ttu-id="d313b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d313b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d313b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d313b-127">Accept</span></span>|<span data-ttu-id="d313b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d313b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d313b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d313b-129">Request body</span></span>
<span data-ttu-id="d313b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d313b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d313b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d313b-131">Response</span></span>
<span data-ttu-id="d313b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d313b-132">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d313b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d313b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d313b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d313b-134">Request</span></span>
<span data-ttu-id="d313b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d313b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="d313b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d313b-136">Response</span></span>
<span data-ttu-id="d313b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d313b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1755

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
    "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
    "exampleJson": "ZXhhbXBsZUpzb24=",
    "schemaItems": [
      {
        "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
        "index": 5,
        "parentIndex": 11,
        "schemaItemKey": "Schema Item Key value",
        "displayName": "Display Name value",
        "description": "Description value",
        "defaultBoolValue": true,
        "defaultIntValue": 15,
        "defaultStringValue": "Default String Value value",
        "defaultStringArrayValue": [
          "Default String Array Value value"
        ],
        "dataType": "integer",
        "selections": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ]
      }
    ],
    "nestedSchemaItems": [
      {
        "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
        "index": 5,
        "parentIndex": 11,
        "schemaItemKey": "Schema Item Key value",
        "displayName": "Display Name value",
        "description": "Description value",
        "defaultBoolValue": true,
        "defaultIntValue": 15,
        "defaultStringValue": "Default String Value value",
        "defaultStringArrayValue": [
          "Default String Array Value value"
        ],
        "dataType": "integer",
        "selections": [
          {
            "@odata.type": "microsoft.graph.keyValuePair",
            "name": "Name value",
            "value": "Value value"
          }
        ]
      }
    ]
  }
}
```






