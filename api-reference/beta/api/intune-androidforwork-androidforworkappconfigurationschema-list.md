---
title: Перечисление объектов androidForWorkAppConfigurationSchema
description: Список свойств и связей объектов androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d68994fd62df5854f02b90b2d5e562928adcc3a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446242"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="ace23-103">Перечисление объектов androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="ace23-103">List androidForWorkAppConfigurationSchemas</span></span>

<span data-ttu-id="ace23-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ace23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ace23-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ace23-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ace23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ace23-107">Список свойств и связей объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="ace23-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ace23-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ace23-108">Prerequisites</span></span>
<span data-ttu-id="ace23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ace23-111">Permission type</span></span>|<span data-ttu-id="ace23-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ace23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ace23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ace23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ace23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ace23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ace23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ace23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace23-116">Not supported.</span></span>|
|<span data-ttu-id="ace23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ace23-117">Application</span></span>|<span data-ttu-id="ace23-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace23-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ace23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ace23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="ace23-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ace23-120">Request headers</span></span>
|<span data-ttu-id="ace23-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ace23-121">Header</span></span>|<span data-ttu-id="ace23-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ace23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ace23-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ace23-123">Authorization</span></span>|<span data-ttu-id="ace23-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ace23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ace23-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ace23-125">Accept</span></span>|<span data-ttu-id="ace23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ace23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace23-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ace23-127">Request body</span></span>
<span data-ttu-id="ace23-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ace23-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ace23-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ace23-129">Response</span></span>
<span data-ttu-id="ace23-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ace23-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ace23-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ace23-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ace23-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ace23-132">Request</span></span>
<span data-ttu-id="ace23-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ace23-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="ace23-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ace23-134">Response</span></span>
<span data-ttu-id="ace23-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ace23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





