---
title: Создание deviceConfigurationGroupAssignment
description: Создание нового объекта deviceConfigurationGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1c7edbe6e646647ffa9887ae49a16539c451e20
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785729"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="35941-103">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="35941-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="35941-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35941-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35941-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35941-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35941-106">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="35941-106">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35941-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35941-107">Prerequisites</span></span>
<span data-ttu-id="35941-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35941-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35941-110">Permission type</span></span>|<span data-ttu-id="35941-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35941-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35941-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35941-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35941-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35941-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35941-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35941-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35941-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35941-115">Not supported.</span></span>|
|<span data-ttu-id="35941-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35941-116">Application</span></span>|<span data-ttu-id="35941-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35941-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35941-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35941-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="35941-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35941-119">Request headers</span></span>
|<span data-ttu-id="35941-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35941-120">Header</span></span>|<span data-ttu-id="35941-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35941-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35941-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35941-122">Authorization</span></span>|<span data-ttu-id="35941-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35941-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35941-124">Accept</span><span class="sxs-lookup"><span data-stu-id="35941-124">Accept</span></span>|<span data-ttu-id="35941-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35941-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35941-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35941-126">Request body</span></span>
<span data-ttu-id="35941-127">В тексте запроса добавьте представление объекта deviceConfigurationGroupAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35941-127">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="35941-128">В следующей таблице приведены свойства, необходимые при создании deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="35941-128">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="35941-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="35941-129">Property</span></span>|<span data-ttu-id="35941-130">Тип</span><span class="sxs-lookup"><span data-stu-id="35941-130">Type</span></span>|<span data-ttu-id="35941-131">Описание</span><span class="sxs-lookup"><span data-stu-id="35941-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35941-132">id</span><span class="sxs-lookup"><span data-stu-id="35941-132">id</span></span>|<span data-ttu-id="35941-133">String</span><span class="sxs-lookup"><span data-stu-id="35941-133">String</span></span>|<span data-ttu-id="35941-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35941-134">Key of the entity.</span></span>|
|<span data-ttu-id="35941-135">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="35941-135">targetGroupId</span></span>|<span data-ttu-id="35941-136">String</span><span class="sxs-lookup"><span data-stu-id="35941-136">String</span></span>|<span data-ttu-id="35941-137">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="35941-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="35941-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="35941-138">excludeGroup</span></span>|<span data-ttu-id="35941-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="35941-139">Boolean</span></span>|<span data-ttu-id="35941-140">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="35941-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="35941-141">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="35941-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="35941-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="35941-142">Response</span></span>
<span data-ttu-id="35941-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35941-143">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35941-144">Пример</span><span class="sxs-lookup"><span data-stu-id="35941-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="35941-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="35941-145">Request</span></span>
<span data-ttu-id="35941-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35941-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="35941-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="35941-147">Response</span></span>
<span data-ttu-id="35941-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35941-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





