---
title: Получение networkIPv6ConfigurationManagementCondition
description: Чтение свойств и связей объекта networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b91598657307e72f1a344e30e23b74e0cf648705
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701895"
---
# <a name="get-networkipv6configurationmanagementcondition"></a><span data-ttu-id="81a43-103">Получение networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="81a43-103">Get networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="81a43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81a43-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81a43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a43-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81a43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a43-107">Чтение свойств и связей объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="81a43-107">Read properties and relationships of the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81a43-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="81a43-108">Prerequisites</span></span>
<span data-ttu-id="81a43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81a43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a43-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81a43-111">Permission type</span></span>|<span data-ttu-id="81a43-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81a43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a43-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81a43-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81a43-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a43-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="81a43-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81a43-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81a43-116">Not supported.</span></span>|
|<span data-ttu-id="81a43-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81a43-117">Application</span></span>|<span data-ttu-id="81a43-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a43-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a43-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81a43-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions/{managementConditionId}
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81a43-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81a43-120">Optional query parameters</span></span>
<span data-ttu-id="81a43-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81a43-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81a43-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81a43-122">Request headers</span></span>
|<span data-ttu-id="81a43-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81a43-123">Header</span></span>|<span data-ttu-id="81a43-124">Значение</span><span class="sxs-lookup"><span data-stu-id="81a43-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a43-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81a43-125">Authorization</span></span>|<span data-ttu-id="81a43-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81a43-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a43-127">Accept</span><span class="sxs-lookup"><span data-stu-id="81a43-127">Accept</span></span>|<span data-ttu-id="81a43-128">application/json</span><span class="sxs-lookup"><span data-stu-id="81a43-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a43-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81a43-129">Request body</span></span>
<span data-ttu-id="81a43-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81a43-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81a43-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="81a43-131">Response</span></span>
<span data-ttu-id="81a43-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81a43-132">If successful, this method returns a `200 OK` response code and [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a43-133">Пример</span><span class="sxs-lookup"><span data-stu-id="81a43-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="81a43-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="81a43-134">Request</span></span>
<span data-ttu-id="81a43-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81a43-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
```

### <a name="response"></a><span data-ttu-id="81a43-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="81a43-136">Response</span></span>
<span data-ttu-id="81a43-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81a43-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
    "id": "25811206-1206-2581-0612-812506128125",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "androidForWork"
    ],
    "ipV6Prefix": "Ip V6Prefix value",
    "ipV6Gateway": "Ip V6Gateway value",
    "ipV6DNSServerList": [
      "Ip V6DNSServer List value"
    ],
    "dnsSuffixList": [
      "Dns Suffix List value"
    ]
  }
}
```





