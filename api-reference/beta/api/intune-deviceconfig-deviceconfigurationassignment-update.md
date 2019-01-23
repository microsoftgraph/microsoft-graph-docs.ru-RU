---
title: Обновление объекта deviceConfigurationAssignment
description: Обновление свойств объекта deviceConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 21457f4d7de5f63d2f6399edb0d36036391ed864
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425339"
---
# <a name="update-deviceconfigurationassignment"></a><span data-ttu-id="32a48-103">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="32a48-103">Update deviceConfigurationAssignment</span></span>

> <span data-ttu-id="32a48-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32a48-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="32a48-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32a48-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32a48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a48-107">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32a48-107">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32a48-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32a48-108">Prerequisites</span></span>
<span data-ttu-id="32a48-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="32a48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32a48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32a48-111">Permission type</span></span>|<span data-ttu-id="32a48-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32a48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32a48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32a48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32a48-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a48-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32a48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32a48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32a48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a48-116">Not supported.</span></span>|
|<span data-ttu-id="32a48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32a48-117">Application</span></span>|<span data-ttu-id="32a48-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a48-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32a48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32a48-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="32a48-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32a48-120">Request headers</span></span>
|<span data-ttu-id="32a48-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32a48-121">Header</span></span>|<span data-ttu-id="32a48-122">Значение</span><span class="sxs-lookup"><span data-stu-id="32a48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32a48-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32a48-123">Authorization</span></span>|<span data-ttu-id="32a48-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="32a48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32a48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32a48-125">Accept</span></span>|<span data-ttu-id="32a48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32a48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32a48-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32a48-127">Request body</span></span>
<span data-ttu-id="32a48-128">В тексте запроса добавьте представление объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32a48-128">In the request body, supply a JSON representation for the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

<span data-ttu-id="32a48-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="32a48-129">The following table shows the properties that are required when you create the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

|<span data-ttu-id="32a48-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="32a48-130">Property</span></span>|<span data-ttu-id="32a48-131">Тип</span><span class="sxs-lookup"><span data-stu-id="32a48-131">Type</span></span>|<span data-ttu-id="32a48-132">Описание</span><span class="sxs-lookup"><span data-stu-id="32a48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a48-133">id</span><span class="sxs-lookup"><span data-stu-id="32a48-133">id</span></span>|<span data-ttu-id="32a48-134">String</span><span class="sxs-lookup"><span data-stu-id="32a48-134">String</span></span>|<span data-ttu-id="32a48-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="32a48-135">The key of the assignment.</span></span>|
|<span data-ttu-id="32a48-136">target</span><span class="sxs-lookup"><span data-stu-id="32a48-136">target</span></span>|[<span data-ttu-id="32a48-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="32a48-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="32a48-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="32a48-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="32a48-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a48-139">Response</span></span>
<span data-ttu-id="32a48-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32a48-140">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32a48-141">Пример</span><span class="sxs-lookup"><span data-stu-id="32a48-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="32a48-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="32a48-142">Request</span></span>
<span data-ttu-id="32a48-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32a48-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="32a48-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a48-144">Response</span></span>
<span data-ttu-id="32a48-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="32a48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




