---
title: Получение networkIPv4ConfigurationManagementCondition
description: Чтение свойств и связей объекта networkIPv4ConfigurationManagementCondition.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6da3c71bba4babfac20e7227ac92fb83bd66939
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179917"
---
# <a name="get-networkipv4configurationmanagementcondition"></a><span data-ttu-id="71085-103">Получение networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="71085-103">Get networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="71085-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71085-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71085-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71085-106">Чтение свойств и связей объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="71085-106">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71085-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71085-107">Prerequisites</span></span>
<span data-ttu-id="71085-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71085-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71085-110">Permission type</span></span>|<span data-ttu-id="71085-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71085-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71085-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71085-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71085-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71085-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71085-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71085-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71085-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71085-115">Not supported.</span></span>|
|<span data-ttu-id="71085-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71085-116">Application</span></span>|<span data-ttu-id="71085-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71085-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71085-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71085-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71085-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71085-119">Optional query parameters</span></span>
<span data-ttu-id="71085-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71085-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71085-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71085-121">Request headers</span></span>
|<span data-ttu-id="71085-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71085-122">Header</span></span>|<span data-ttu-id="71085-123">Значение</span><span class="sxs-lookup"><span data-stu-id="71085-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71085-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71085-124">Authorization</span></span>|<span data-ttu-id="71085-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71085-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71085-126">Accept</span><span class="sxs-lookup"><span data-stu-id="71085-126">Accept</span></span>|<span data-ttu-id="71085-127">application/json</span><span class="sxs-lookup"><span data-stu-id="71085-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71085-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71085-128">Request body</span></span>
<span data-ttu-id="71085-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71085-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71085-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="71085-130">Response</span></span>
<span data-ttu-id="71085-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71085-131">If successful, this method returns a `200 OK` response code and [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71085-132">Пример</span><span class="sxs-lookup"><span data-stu-id="71085-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="71085-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="71085-133">Request</span></span>
<span data-ttu-id="71085-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71085-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="71085-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="71085-135">Response</span></span>
<span data-ttu-id="71085-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71085-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
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
}
```




