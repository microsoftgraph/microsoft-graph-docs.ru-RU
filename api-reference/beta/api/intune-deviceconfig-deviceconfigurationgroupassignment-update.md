---
title: Обновление deviceConfigurationGroupAssignment
description: Обновление свойства объекта deviceConfigurationGroupAssignment.
ms.openlocfilehash: 303ecefdccafc133c4680bc0fd7eb866b682fded
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079907"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="c0b0f-103">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="c0b0f-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="c0b0f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0b0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0b0f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0b0f-107">Обновление свойства объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c0b0f-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0b0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0b0f-108">Prerequisites</span></span>
<span data-ttu-id="c0b0f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0b0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0b0f-111">Permission type</span></span>|<span data-ttu-id="c0b0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0b0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0b0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0b0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0b0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0b0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0b0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0b0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-116">Not supported.</span></span>|
|<span data-ttu-id="c0b0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0b0f-117">Application</span></span>|<span data-ttu-id="c0b0f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0b0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0b0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c0b0f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0b0f-120">Request headers</span></span>
|<span data-ttu-id="c0b0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0b0f-121">Header</span></span>|<span data-ttu-id="c0b0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0b0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0b0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b0f-123">Authorization</span></span>|<span data-ttu-id="c0b0f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c0b0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0b0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0b0f-125">Accept</span></span>|<span data-ttu-id="c0b0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0b0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0b0f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0b0f-127">Request body</span></span>
<span data-ttu-id="c0b0f-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c0b0f-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="c0b0f-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0b0f-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="c0b0f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0b0f-130">Property</span></span>|<span data-ttu-id="c0b0f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c0b0f-131">Type</span></span>|<span data-ttu-id="c0b0f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c0b0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b0f-133">id</span><span class="sxs-lookup"><span data-stu-id="c0b0f-133">id</span></span>|<span data-ttu-id="c0b0f-134">String</span><span class="sxs-lookup"><span data-stu-id="c0b0f-134">String</span></span>|<span data-ttu-id="c0b0f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-135">Key of the entity.</span></span>|
|<span data-ttu-id="c0b0f-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="c0b0f-136">targetGroupId</span></span>|<span data-ttu-id="c0b0f-137">String</span><span class="sxs-lookup"><span data-stu-id="c0b0f-137">String</span></span>|<span data-ttu-id="c0b0f-138">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="c0b0f-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="c0b0f-139">excludeGroup</span></span>|<span data-ttu-id="c0b0f-140">Логический</span><span class="sxs-lookup"><span data-stu-id="c0b0f-140">Boolean</span></span>|<span data-ttu-id="c0b0f-141">Указывает, является ли эта группа следует исключить.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="c0b0f-142">Параметры по умолчанию, что группы должны быть включены</span><span class="sxs-lookup"><span data-stu-id="c0b0f-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="c0b0f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0b0f-143">Response</span></span>
<span data-ttu-id="c0b0f-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b0f-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c0b0f-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0b0f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0b0f-146">Request</span></span>
<span data-ttu-id="c0b0f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0b0f-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 73

{
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="c0b0f-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0b0f-148">Response</span></span>
<span data-ttu-id="c0b0f-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c0b0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





