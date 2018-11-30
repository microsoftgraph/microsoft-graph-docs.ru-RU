---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
ms.openlocfilehash: 51d4ea7c0c5a49b59777d5deaa364a8791a7db8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075876"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="47f49-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="47f49-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="47f49-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47f49-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47f49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47f49-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47f49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47f49-107">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47f49-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47f49-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="47f49-108">Prerequisites</span></span>
<span data-ttu-id="47f49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47f49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47f49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47f49-111">Permission type</span></span>|<span data-ttu-id="47f49-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47f49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47f49-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47f49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47f49-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47f49-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47f49-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47f49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47f49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f49-116">Not supported.</span></span>|
|<span data-ttu-id="47f49-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47f49-117">Application</span></span>|<span data-ttu-id="47f49-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47f49-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47f49-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47f49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="47f49-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47f49-120">Request headers</span></span>
|<span data-ttu-id="47f49-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47f49-121">Header</span></span>|<span data-ttu-id="47f49-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47f49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47f49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47f49-123">Authorization</span></span>|<span data-ttu-id="47f49-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="47f49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47f49-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47f49-125">Accept</span></span>|<span data-ttu-id="47f49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47f49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47f49-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47f49-127">Request body</span></span>
<span data-ttu-id="47f49-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47f49-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47f49-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="47f49-129">Response</span></span>
<span data-ttu-id="47f49-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47f49-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47f49-131">Пример</span><span class="sxs-lookup"><span data-stu-id="47f49-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="47f49-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="47f49-132">Request</span></span>
<span data-ttu-id="47f49-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47f49-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="47f49-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="47f49-134">Response</span></span>
<span data-ttu-id="47f49-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="47f49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





