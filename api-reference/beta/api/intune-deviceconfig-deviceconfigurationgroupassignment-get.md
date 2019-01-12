---
title: Получение deviceConfigurationGroupAssignment
description: Чтение свойства и связи объекта deviceConfigurationGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09faec45d80eec6eb65f5101295a72501635abc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967793"
---
# <a name="get-deviceconfigurationgroupassignment"></a><span data-ttu-id="ea2ce-103">Получение deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="ea2ce-103">Get deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="ea2ce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea2ce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea2ce-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea2ce-107">Чтение свойства и связи объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ea2ce-107">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea2ce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea2ce-108">Prerequisites</span></span>
<span data-ttu-id="ea2ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea2ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea2ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea2ce-111">Permission type</span></span>|<span data-ttu-id="ea2ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea2ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea2ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea2ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea2ce-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea2ce-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ea2ce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea2ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea2ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-116">Not supported.</span></span>|
|<span data-ttu-id="ea2ce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea2ce-117">Application</span></span>|<span data-ttu-id="ea2ce-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea2ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea2ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea2ce-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea2ce-120">Optional query parameters</span></span>
<span data-ttu-id="ea2ce-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea2ce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea2ce-122">Request headers</span></span>
|<span data-ttu-id="ea2ce-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea2ce-123">Header</span></span>|<span data-ttu-id="ea2ce-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ea2ce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea2ce-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea2ce-125">Authorization</span></span>|<span data-ttu-id="ea2ce-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ea2ce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea2ce-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ea2ce-127">Accept</span></span>|<span data-ttu-id="ea2ce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ea2ce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea2ce-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea2ce-129">Request body</span></span>
<span data-ttu-id="ea2ce-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea2ce-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea2ce-131">Response</span></span>
<span data-ttu-id="ea2ce-132">Успешно завершена, этот метод возвращает `200 OK` объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea2ce-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ea2ce-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea2ce-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea2ce-134">Request</span></span>
<span data-ttu-id="ea2ce-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ea2ce-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea2ce-136">Response</span></span>
<span data-ttu-id="ea2ce-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ea2ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
    "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
    "targetGroupId": "Target Group Id value",
    "excludeGroup": true
  }
}
```





