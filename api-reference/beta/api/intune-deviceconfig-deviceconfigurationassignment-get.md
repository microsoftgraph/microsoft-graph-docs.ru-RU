---
title: Get deviceConfigurationAssignment
description: Чтение свойств и связей объекта deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 54a1086e7d6d6cfc266cb73f75e3a775a788b700
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847975"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="a3928-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a3928-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="a3928-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a3928-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3928-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3928-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3928-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3928-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3928-107">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a3928-107">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3928-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a3928-108">Prerequisites</span></span>
<span data-ttu-id="a3928-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3928-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3928-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3928-111">Permission type</span></span>|<span data-ttu-id="a3928-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3928-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3928-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3928-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3928-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3928-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3928-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3928-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3928-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3928-116">Not supported.</span></span>|
|<span data-ttu-id="a3928-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3928-117">Application</span></span>|<span data-ttu-id="a3928-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3928-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3928-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3928-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3928-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3928-120">Optional query parameters</span></span>
<span data-ttu-id="a3928-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3928-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a3928-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3928-122">Request headers</span></span>
|<span data-ttu-id="a3928-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3928-123">Header</span></span>|<span data-ttu-id="a3928-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a3928-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3928-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3928-125">Authorization</span></span>|<span data-ttu-id="a3928-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3928-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3928-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a3928-127">Accept</span></span>|<span data-ttu-id="a3928-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a3928-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3928-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3928-129">Request body</span></span>
<span data-ttu-id="a3928-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3928-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3928-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3928-131">Response</span></span>
<span data-ttu-id="a3928-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a3928-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3928-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a3928-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3928-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3928-134">Request</span></span>
<span data-ttu-id="a3928-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3928-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a3928-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3928-136">Response</span></span>
<span data-ttu-id="a3928-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3928-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





