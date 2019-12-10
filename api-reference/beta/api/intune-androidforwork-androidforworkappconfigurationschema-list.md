---
title: Перечисление объектов androidForWorkAppConfigurationSchema
description: Список свойств и связей объектов androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 345de6ed1f92f54bb4c08297d61b2f5ad4dbde9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39927974"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="26b8b-103">Перечисление объектов androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="26b8b-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="26b8b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26b8b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26b8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26b8b-106">Список свойств и связей объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="26b8b-106">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26b8b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="26b8b-107">Prerequisites</span></span>
<span data-ttu-id="26b8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26b8b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b8b-110">Permission type</span></span>|<span data-ttu-id="26b8b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26b8b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26b8b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b8b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="26b8b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b8b-115">Not supported.</span></span>|
|<span data-ttu-id="26b8b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b8b-116">Application</span></span>|<span data-ttu-id="26b8b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="26b8b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26b8b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="26b8b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26b8b-119">Request headers</span></span>
|<span data-ttu-id="26b8b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26b8b-120">Header</span></span>|<span data-ttu-id="26b8b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="26b8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26b8b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26b8b-122">Authorization</span></span>|<span data-ttu-id="26b8b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26b8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26b8b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="26b8b-124">Accept</span></span>|<span data-ttu-id="26b8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26b8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b8b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26b8b-126">Request body</span></span>
<span data-ttu-id="26b8b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26b8b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b8b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="26b8b-128">Response</span></span>
<span data-ttu-id="26b8b-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26b8b-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26b8b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="26b8b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="26b8b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b8b-131">Request</span></span>
<span data-ttu-id="26b8b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26b8b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="26b8b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b8b-133">Response</span></span>
<span data-ttu-id="26b8b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26b8b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





