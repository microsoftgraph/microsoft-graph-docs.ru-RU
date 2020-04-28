---
title: Get androidForWorkAppConfigurationSchema
description: Чтение свойств и связей объекта androidForWorkAppConfigurationSchema.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5b92c06c71171338fbe13e1d20f52d1f67f5804e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43418410"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="15a64-103">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="15a64-103">Get androidForWorkAppConfigurationSchema</span></span>

<span data-ttu-id="15a64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15a64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15a64-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15a64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15a64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15a64-107">Чтение свойств и связей объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="15a64-107">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15a64-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="15a64-108">Prerequisites</span></span>
<span data-ttu-id="15a64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15a64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15a64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15a64-111">Permission type</span></span>|<span data-ttu-id="15a64-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15a64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15a64-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15a64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15a64-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a64-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="15a64-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15a64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15a64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a64-116">Not supported.</span></span>|
|<span data-ttu-id="15a64-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15a64-117">Application</span></span>|<span data-ttu-id="15a64-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a64-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15a64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15a64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15a64-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15a64-120">Optional query parameters</span></span>
<span data-ttu-id="15a64-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15a64-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15a64-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15a64-122">Request headers</span></span>
|<span data-ttu-id="15a64-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15a64-123">Header</span></span>|<span data-ttu-id="15a64-124">Значение</span><span class="sxs-lookup"><span data-stu-id="15a64-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15a64-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15a64-125">Authorization</span></span>|<span data-ttu-id="15a64-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15a64-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15a64-127">Accept</span><span class="sxs-lookup"><span data-stu-id="15a64-127">Accept</span></span>|<span data-ttu-id="15a64-128">application/json</span><span class="sxs-lookup"><span data-stu-id="15a64-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15a64-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15a64-129">Request body</span></span>
<span data-ttu-id="15a64-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15a64-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15a64-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="15a64-131">Response</span></span>
<span data-ttu-id="15a64-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="15a64-132">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15a64-133">Пример</span><span class="sxs-lookup"><span data-stu-id="15a64-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="15a64-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a64-134">Request</span></span>
<span data-ttu-id="15a64-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15a64-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="15a64-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a64-136">Response</span></span>
<span data-ttu-id="15a64-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15a64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 913

{
  "value": {
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
}
```



