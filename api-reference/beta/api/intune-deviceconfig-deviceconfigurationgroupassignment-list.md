---
title: Список deviceConfigurationGroupAssignments
description: Свойства списка и связей объектов deviceConfigurationGroupAssignment.
author: tfitzmac
ms.openlocfilehash: a1dce979ab078d22c755b77724abfd274a1872cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361434"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="7e882-103">Список deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="7e882-103">List deviceConfigurationGroupAssignments</span></span>

> <span data-ttu-id="7e882-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7e882-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e882-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e882-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e882-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7e882-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e882-107">Свойства списка и связей объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7e882-107">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e882-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7e882-108">Prerequisites</span></span>
<span data-ttu-id="7e882-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e882-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e882-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e882-111">Permission type</span></span>|<span data-ttu-id="7e882-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e882-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e882-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e882-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e882-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e882-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7e882-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e882-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e882-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e882-116">Not supported.</span></span>|
|<span data-ttu-id="7e882-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e882-117">Application</span></span>|<span data-ttu-id="7e882-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e882-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e882-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e882-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="7e882-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e882-120">Request headers</span></span>
|<span data-ttu-id="7e882-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e882-121">Header</span></span>|<span data-ttu-id="7e882-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7e882-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e882-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e882-123">Authorization</span></span>|<span data-ttu-id="7e882-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7e882-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e882-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e882-125">Accept</span></span>|<span data-ttu-id="7e882-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e882-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e882-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e882-127">Request body</span></span>
<span data-ttu-id="7e882-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e882-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e882-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e882-129">Response</span></span>
<span data-ttu-id="7e882-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7e882-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e882-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7e882-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e882-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e882-132">Request</span></span>
<span data-ttu-id="7e882-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e882-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="7e882-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e882-134">Response</span></span>
<span data-ttu-id="7e882-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7e882-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```





