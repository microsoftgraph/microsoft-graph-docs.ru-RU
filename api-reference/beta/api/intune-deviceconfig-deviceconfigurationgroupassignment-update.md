---
title: Обновление deviceConfigurationGroupAssignment
description: Обновление свойства объекта deviceConfigurationGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632ade6d8c2fdb2cfb859c3b480606547d9b0ead
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938519"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="673d8-103">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="673d8-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="673d8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="673d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="673d8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="673d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="673d8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="673d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="673d8-107">Обновление свойства объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="673d8-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="673d8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="673d8-108">Prerequisites</span></span>
<span data-ttu-id="673d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="673d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="673d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="673d8-111">Permission type</span></span>|<span data-ttu-id="673d8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="673d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="673d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="673d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="673d8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673d8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="673d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="673d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="673d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="673d8-116">Not supported.</span></span>|
|<span data-ttu-id="673d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="673d8-117">Application</span></span>|<span data-ttu-id="673d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="673d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="673d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="673d8-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="673d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="673d8-120">Request headers</span></span>
|<span data-ttu-id="673d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="673d8-121">Header</span></span>|<span data-ttu-id="673d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="673d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="673d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="673d8-123">Authorization</span></span>|<span data-ttu-id="673d8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="673d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="673d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="673d8-125">Accept</span></span>|<span data-ttu-id="673d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="673d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="673d8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="673d8-127">Request body</span></span>
<span data-ttu-id="673d8-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="673d8-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="673d8-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="673d8-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="673d8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="673d8-130">Property</span></span>|<span data-ttu-id="673d8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="673d8-131">Type</span></span>|<span data-ttu-id="673d8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="673d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="673d8-133">id</span><span class="sxs-lookup"><span data-stu-id="673d8-133">id</span></span>|<span data-ttu-id="673d8-134">String</span><span class="sxs-lookup"><span data-stu-id="673d8-134">String</span></span>|<span data-ttu-id="673d8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="673d8-135">Key of the entity.</span></span>|
|<span data-ttu-id="673d8-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="673d8-136">targetGroupId</span></span>|<span data-ttu-id="673d8-137">String</span><span class="sxs-lookup"><span data-stu-id="673d8-137">String</span></span>|<span data-ttu-id="673d8-138">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="673d8-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="673d8-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="673d8-139">excludeGroup</span></span>|<span data-ttu-id="673d8-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="673d8-140">Boolean</span></span>|<span data-ttu-id="673d8-141">Указывает, является ли эта группа следует исключить.</span><span class="sxs-lookup"><span data-stu-id="673d8-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="673d8-142">Параметры по умолчанию, что группы должны быть включены</span><span class="sxs-lookup"><span data-stu-id="673d8-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="673d8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="673d8-143">Response</span></span>
<span data-ttu-id="673d8-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="673d8-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="673d8-145">Пример</span><span class="sxs-lookup"><span data-stu-id="673d8-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="673d8-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="673d8-146">Request</span></span>
<span data-ttu-id="673d8-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="673d8-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 73

{
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="673d8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="673d8-148">Response</span></span>
<span data-ttu-id="673d8-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="673d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





