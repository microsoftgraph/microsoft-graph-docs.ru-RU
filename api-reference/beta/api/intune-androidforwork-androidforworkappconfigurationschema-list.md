---
title: Перечисление объектов androidForWorkAppConfigurationSchema
description: Список свойств и связей объектов androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdc9aeb2ba6a17b1c58908383e2a4da18fa9c82b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001402"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="81a40-103">Перечисление объектов androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="81a40-103">List androidForWorkAppConfigurationSchemas</span></span>

<span data-ttu-id="81a40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81a40-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a40-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a40-107">Список свойств и связей объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="81a40-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81a40-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="81a40-108">Prerequisites</span></span>
<span data-ttu-id="81a40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81a40-111">Permission type</span></span>|<span data-ttu-id="81a40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81a40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81a40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81a40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81a40-116">Not supported.</span></span>|
|<span data-ttu-id="81a40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81a40-117">Application</span></span>|<span data-ttu-id="81a40-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a40-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="81a40-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="81a40-120">Request headers</span></span>
|<span data-ttu-id="81a40-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81a40-121">Header</span></span>|<span data-ttu-id="81a40-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81a40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81a40-123">Authorization</span></span>|<span data-ttu-id="81a40-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81a40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81a40-125">Accept</span></span>|<span data-ttu-id="81a40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81a40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a40-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81a40-127">Request body</span></span>
<span data-ttu-id="81a40-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81a40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81a40-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="81a40-129">Response</span></span>
<span data-ttu-id="81a40-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81a40-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a40-131">Пример</span><span class="sxs-lookup"><span data-stu-id="81a40-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="81a40-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="81a40-132">Request</span></span>
<span data-ttu-id="81a40-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81a40-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="81a40-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="81a40-134">Response</span></span>
<span data-ttu-id="81a40-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81a40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
      "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
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
  ]
}
```






