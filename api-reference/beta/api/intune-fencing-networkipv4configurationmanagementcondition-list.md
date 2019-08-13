---
title: Список networkIPv4ConfigurationManagementConditions
description: Список свойств и связей объектов networkIPv4ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef1d3c48e086e16051e7db1d40dd11409a6053ca
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355467"
---
# <a name="list-networkipv4configurationmanagementconditions"></a><span data-ttu-id="9a41b-103">Список networkIPv4ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="9a41b-103">List networkIPv4ConfigurationManagementConditions</span></span>

> <span data-ttu-id="9a41b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a41b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a41b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a41b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a41b-106">Список свойств и связей объектов [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="9a41b-106">List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a41b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9a41b-107">Prerequisites</span></span>
<span data-ttu-id="9a41b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a41b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a41b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a41b-110">Permission type</span></span>|<span data-ttu-id="9a41b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a41b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a41b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a41b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a41b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a41b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9a41b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a41b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a41b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a41b-115">Not supported.</span></span>|
|<span data-ttu-id="9a41b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a41b-116">Application</span></span>|<span data-ttu-id="9a41b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a41b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a41b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a41b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="9a41b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a41b-119">Request headers</span></span>
|<span data-ttu-id="9a41b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a41b-120">Header</span></span>|<span data-ttu-id="9a41b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9a41b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a41b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a41b-122">Authorization</span></span>|<span data-ttu-id="9a41b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a41b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a41b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9a41b-124">Accept</span></span>|<span data-ttu-id="9a41b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a41b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a41b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a41b-126">Request body</span></span>
<span data-ttu-id="9a41b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a41b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a41b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a41b-128">Response</span></span>
<span data-ttu-id="9a41b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a41b-129">If successful, this method returns a `200 OK` response code and a collection of [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a41b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9a41b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a41b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a41b-131">Request</span></span>
<span data-ttu-id="9a41b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a41b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="9a41b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a41b-133">Response</span></span>
<span data-ttu-id="9a41b-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a41b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
      "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "ipV4Prefix": "Ip V4Prefix value",
      "ipV4Gateway": "Ip V4Gateway value",
      "ipV4DHCPServer": "Ip V4DHCPServer value",
      "ipV4DNSServerList": [
        "Ip V4DNSServer List value"
      ],
      "dnsSuffixList": [
        "Dns Suffix List value"
      ]
    }
  ]
}
```






