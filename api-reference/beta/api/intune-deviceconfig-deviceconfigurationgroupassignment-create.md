---
title: Создание deviceConfigurationGroupAssignment
description: Создание нового объекта deviceConfigurationGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a74acc7b2be82506195d5d3646e6932533a62ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413229"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="f69e1-103">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f69e1-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="f69e1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f69e1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f69e1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f69e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f69e1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f69e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f69e1-107">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f69e1-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f69e1-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f69e1-108">Prerequisites</span></span>
<span data-ttu-id="f69e1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f69e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f69e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f69e1-111">Permission type</span></span>|<span data-ttu-id="f69e1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f69e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f69e1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f69e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f69e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f69e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f69e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f69e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f69e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f69e1-116">Not supported.</span></span>|
|<span data-ttu-id="f69e1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f69e1-117">Application</span></span>|<span data-ttu-id="f69e1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f69e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f69e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f69e1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f69e1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f69e1-120">Request headers</span></span>
|<span data-ttu-id="f69e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f69e1-121">Header</span></span>|<span data-ttu-id="f69e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f69e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f69e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f69e1-123">Authorization</span></span>|<span data-ttu-id="f69e1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f69e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f69e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f69e1-125">Accept</span></span>|<span data-ttu-id="f69e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f69e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f69e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f69e1-127">Request body</span></span>
<span data-ttu-id="f69e1-128">В тексте запроса укажите представление JSON для объекта deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="f69e1-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="f69e1-129">В следующей таблице показаны свойства, которые необходимы для создания deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="f69e1-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="f69e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f69e1-130">Property</span></span>|<span data-ttu-id="f69e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f69e1-131">Type</span></span>|<span data-ttu-id="f69e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f69e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f69e1-133">id</span><span class="sxs-lookup"><span data-stu-id="f69e1-133">id</span></span>|<span data-ttu-id="f69e1-134">String</span><span class="sxs-lookup"><span data-stu-id="f69e1-134">String</span></span>|<span data-ttu-id="f69e1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f69e1-135">Key of the entity.</span></span>|
|<span data-ttu-id="f69e1-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="f69e1-136">targetGroupId</span></span>|<span data-ttu-id="f69e1-137">String</span><span class="sxs-lookup"><span data-stu-id="f69e1-137">String</span></span>|<span data-ttu-id="f69e1-138">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="f69e1-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="f69e1-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="f69e1-139">excludeGroup</span></span>|<span data-ttu-id="f69e1-140">Логический</span><span class="sxs-lookup"><span data-stu-id="f69e1-140">Boolean</span></span>|<span data-ttu-id="f69e1-141">Указывает, является ли эта группа следует исключить.</span><span class="sxs-lookup"><span data-stu-id="f69e1-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="f69e1-142">Параметры по умолчанию, что группы должны быть включены</span><span class="sxs-lookup"><span data-stu-id="f69e1-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="f69e1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f69e1-143">Response</span></span>
<span data-ttu-id="f69e1-144">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f69e1-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f69e1-145">Пример</span><span class="sxs-lookup"><span data-stu-id="f69e1-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="f69e1-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f69e1-146">Request</span></span>
<span data-ttu-id="f69e1-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f69e1-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f69e1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f69e1-148">Response</span></span>
<span data-ttu-id="f69e1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f69e1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




