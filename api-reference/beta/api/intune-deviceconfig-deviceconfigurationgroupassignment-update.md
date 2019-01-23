---
title: Обновление deviceConfigurationGroupAssignment
description: Обновление свойства объекта deviceConfigurationGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93399328a5be63bcb994fab58b6cad638a44d97f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396289"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="6d7d2-103">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d7d2-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="6d7d2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d7d2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d7d2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d7d2-107">Обновление свойства объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6d7d2-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d7d2-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="6d7d2-108">Prerequisites</span></span>
<span data-ttu-id="6d7d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d7d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6d7d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7d2-111">Permission type</span></span>|<span data-ttu-id="6d7d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d7d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d7d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d7d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d7d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d7d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d7d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d7d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d7d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-116">Not supported.</span></span>|
|<span data-ttu-id="6d7d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d7d2-117">Application</span></span>|<span data-ttu-id="6d7d2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d7d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d7d2-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6d7d2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d7d2-120">Request headers</span></span>
|<span data-ttu-id="6d7d2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d7d2-121">Header</span></span>|<span data-ttu-id="6d7d2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d7d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d7d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d7d2-123">Authorization</span></span>|<span data-ttu-id="6d7d2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6d7d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d7d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d7d2-125">Accept</span></span>|<span data-ttu-id="6d7d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d7d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d7d2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d7d2-127">Request body</span></span>
<span data-ttu-id="6d7d2-128">В тексте запроса укажите представление JSON для объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6d7d2-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="6d7d2-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6d7d2-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="6d7d2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d7d2-130">Property</span></span>|<span data-ttu-id="6d7d2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6d7d2-131">Type</span></span>|<span data-ttu-id="6d7d2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6d7d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d7d2-133">id</span><span class="sxs-lookup"><span data-stu-id="6d7d2-133">id</span></span>|<span data-ttu-id="6d7d2-134">String</span><span class="sxs-lookup"><span data-stu-id="6d7d2-134">String</span></span>|<span data-ttu-id="6d7d2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-135">Key of the entity.</span></span>|
|<span data-ttu-id="6d7d2-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="6d7d2-136">targetGroupId</span></span>|<span data-ttu-id="6d7d2-137">String</span><span class="sxs-lookup"><span data-stu-id="6d7d2-137">String</span></span>|<span data-ttu-id="6d7d2-138">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="6d7d2-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="6d7d2-139">excludeGroup</span></span>|<span data-ttu-id="6d7d2-140">Логический</span><span class="sxs-lookup"><span data-stu-id="6d7d2-140">Boolean</span></span>|<span data-ttu-id="6d7d2-141">Указывает, является ли эта группа следует исключить.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="6d7d2-142">Параметры по умолчанию, что группы должны быть включены</span><span class="sxs-lookup"><span data-stu-id="6d7d2-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="6d7d2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7d2-143">Response</span></span>
<span data-ttu-id="6d7d2-144">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d7d2-145">Пример</span><span class="sxs-lookup"><span data-stu-id="6d7d2-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d7d2-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d7d2-146">Request</span></span>
<span data-ttu-id="6d7d2-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="6d7d2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7d2-148">Response</span></span>
<span data-ttu-id="6d7d2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6d7d2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




