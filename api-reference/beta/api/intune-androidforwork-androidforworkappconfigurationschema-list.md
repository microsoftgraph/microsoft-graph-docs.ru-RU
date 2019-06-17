---
title: Перечисление объектов androidForWorkAppConfigurationSchema
description: Список свойств и связей объектов androidForWorkAppConfigurationSchema.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6cd8f76142983b42be24632c4ca79371423c322
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966574"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="2e170-103">Перечисление объектов androidForWorkAppConfigurationSchema</span><span class="sxs-lookup"><span data-stu-id="2e170-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="2e170-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e170-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e170-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e170-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e170-106">Список свойств и связей объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="2e170-106">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e170-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e170-107">Prerequisites</span></span>
<span data-ttu-id="2e170-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e170-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e170-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e170-110">Permission type</span></span>|<span data-ttu-id="2e170-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e170-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e170-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e170-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e170-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e170-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e170-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e170-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e170-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e170-115">Not supported.</span></span>|
|<span data-ttu-id="2e170-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e170-116">Application</span></span>|<span data-ttu-id="2e170-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e170-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e170-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e170-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="2e170-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e170-119">Request headers</span></span>
|<span data-ttu-id="2e170-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e170-120">Header</span></span>|<span data-ttu-id="2e170-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2e170-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e170-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e170-122">Authorization</span></span>|<span data-ttu-id="2e170-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e170-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e170-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2e170-124">Accept</span></span>|<span data-ttu-id="2e170-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e170-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e170-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e170-126">Request body</span></span>
<span data-ttu-id="2e170-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e170-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e170-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e170-128">Response</span></span>
<span data-ttu-id="2e170-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e170-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e170-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2e170-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e170-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e170-131">Request</span></span>
<span data-ttu-id="2e170-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e170-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="2e170-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e170-133">Response</span></span>
<span data-ttu-id="2e170-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e170-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





