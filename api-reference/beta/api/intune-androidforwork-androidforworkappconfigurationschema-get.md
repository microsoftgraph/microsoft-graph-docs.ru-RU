---
title: Get androidForWorkAppConfigurationSchema
description: Чтение свойств и связей объекта androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfed24f2a7f02aeab94e816e724f000938a89d56
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174195"
---
# <a name="get-androidforworkappconfigurationschema"></a><span data-ttu-id="89660-103">Get androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="89660-103">Get androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="89660-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89660-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89660-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89660-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89660-106">Чтение свойств и связей объекта [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="89660-106">Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89660-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="89660-107">Prerequisites</span></span>
<span data-ttu-id="89660-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89660-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89660-110">Permission type</span></span>|<span data-ttu-id="89660-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89660-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89660-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89660-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89660-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89660-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89660-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89660-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89660-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89660-115">Not supported.</span></span>|
|<span data-ttu-id="89660-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89660-116">Application</span></span>|<span data-ttu-id="89660-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89660-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89660-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89660-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89660-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89660-119">Optional query parameters</span></span>
<span data-ttu-id="89660-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="89660-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89660-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89660-121">Request headers</span></span>
|<span data-ttu-id="89660-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89660-122">Header</span></span>|<span data-ttu-id="89660-123">Значение</span><span class="sxs-lookup"><span data-stu-id="89660-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89660-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89660-124">Authorization</span></span>|<span data-ttu-id="89660-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89660-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89660-126">Accept</span><span class="sxs-lookup"><span data-stu-id="89660-126">Accept</span></span>|<span data-ttu-id="89660-127">application/json</span><span class="sxs-lookup"><span data-stu-id="89660-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89660-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89660-128">Request body</span></span>
<span data-ttu-id="89660-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89660-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89660-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="89660-130">Response</span></span>
<span data-ttu-id="89660-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="89660-131">If successful, this method returns a `200 OK` response code and [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89660-132">Пример</span><span class="sxs-lookup"><span data-stu-id="89660-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="89660-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="89660-133">Request</span></span>
<span data-ttu-id="89660-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89660-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

### <a name="response"></a><span data-ttu-id="89660-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="89660-135">Response</span></span>
<span data-ttu-id="89660-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89660-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




