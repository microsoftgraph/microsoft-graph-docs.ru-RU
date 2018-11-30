---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
ms.openlocfilehash: 2933f66f648a00f4fd66dd4ec20cbcbba395acd2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077500"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="fda20-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="fda20-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="fda20-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fda20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fda20-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fda20-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fda20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fda20-107">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fda20-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fda20-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fda20-108">Prerequisites</span></span>
<span data-ttu-id="fda20-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fda20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fda20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fda20-111">Permission type</span></span>|<span data-ttu-id="fda20-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fda20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fda20-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fda20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fda20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fda20-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fda20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fda20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda20-116">Not supported.</span></span>|
|<span data-ttu-id="fda20-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fda20-117">Application</span></span>|<span data-ttu-id="fda20-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fda20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fda20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fda20-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fda20-120">Request headers</span></span>
|<span data-ttu-id="fda20-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fda20-121">Header</span></span>|<span data-ttu-id="fda20-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fda20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fda20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda20-123">Authorization</span></span>|<span data-ttu-id="fda20-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fda20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fda20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fda20-125">Accept</span></span>|<span data-ttu-id="fda20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fda20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fda20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fda20-127">Request body</span></span>
<span data-ttu-id="fda20-128">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fda20-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="fda20-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fda20-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="fda20-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fda20-130">Property</span></span>|<span data-ttu-id="fda20-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fda20-131">Type</span></span>|<span data-ttu-id="fda20-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fda20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fda20-133">id</span><span class="sxs-lookup"><span data-stu-id="fda20-133">id</span></span>|<span data-ttu-id="fda20-134">String</span><span class="sxs-lookup"><span data-stu-id="fda20-134">String</span></span>|<span data-ttu-id="fda20-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="fda20-135">The key of the assignment.</span></span>|
|<span data-ttu-id="fda20-136">target</span><span class="sxs-lookup"><span data-stu-id="fda20-136">target</span></span>|[<span data-ttu-id="fda20-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fda20-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fda20-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="fda20-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fda20-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fda20-139">Response</span></span>
<span data-ttu-id="fda20-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fda20-140">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda20-141">Пример</span><span class="sxs-lookup"><span data-stu-id="fda20-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="fda20-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fda20-142">Request</span></span>
<span data-ttu-id="fda20-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fda20-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="fda20-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="fda20-144">Response</span></span>
<span data-ttu-id="fda20-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fda20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





