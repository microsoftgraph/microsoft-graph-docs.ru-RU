---
title: Обновление К mobileappprovisioningconfiggroupassignment.
description: Обновление свойств объекта К mobileappprovisioningconfiggroupassignment..
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e1d7b80d5ed0d24e8b85b343704442e80bbe8fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32488737"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="95bfe-103">Обновление К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="95bfe-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="95bfe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95bfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95bfe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95bfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95bfe-106">Обновление свойств объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="95bfe-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95bfe-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95bfe-107">Prerequisites</span></span>
<span data-ttu-id="95bfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95bfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95bfe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95bfe-110">Permission type</span></span>|<span data-ttu-id="95bfe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95bfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95bfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95bfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95bfe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95bfe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95bfe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95bfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95bfe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95bfe-115">Not supported.</span></span>|
|<span data-ttu-id="95bfe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95bfe-116">Application</span></span>|<span data-ttu-id="95bfe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95bfe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95bfe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95bfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="95bfe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95bfe-119">Request headers</span></span>
|<span data-ttu-id="95bfe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95bfe-120">Header</span></span>|<span data-ttu-id="95bfe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95bfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95bfe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95bfe-122">Authorization</span></span>|<span data-ttu-id="95bfe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95bfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95bfe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95bfe-124">Accept</span></span>|<span data-ttu-id="95bfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95bfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95bfe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95bfe-126">Request body</span></span>
<span data-ttu-id="95bfe-127">В тексте запроса добавьте представление объекта [К mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95bfe-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="95bfe-128">В следующей таблице приведены свойства, необходимые при создании [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="95bfe-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="95bfe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95bfe-129">Property</span></span>|<span data-ttu-id="95bfe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95bfe-130">Type</span></span>|<span data-ttu-id="95bfe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95bfe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95bfe-132">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="95bfe-132">targetGroupId</span></span>|<span data-ttu-id="95bfe-133">String</span><span class="sxs-lookup"><span data-stu-id="95bfe-133">String</span></span>|<span data-ttu-id="95bfe-134">Идентификатор группы AAD, в которой нацелена конфигурация подготовки приложений.</span><span class="sxs-lookup"><span data-stu-id="95bfe-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="95bfe-135">id</span><span class="sxs-lookup"><span data-stu-id="95bfe-135">id</span></span>|<span data-ttu-id="95bfe-136">String</span><span class="sxs-lookup"><span data-stu-id="95bfe-136">String</span></span>|<span data-ttu-id="95bfe-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95bfe-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="95bfe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="95bfe-138">Response</span></span>
<span data-ttu-id="95bfe-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95bfe-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95bfe-140">Пример</span><span class="sxs-lookup"><span data-stu-id="95bfe-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="95bfe-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="95bfe-141">Request</span></span>
<span data-ttu-id="95bfe-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95bfe-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="95bfe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="95bfe-143">Response</span></span>
<span data-ttu-id="95bfe-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95bfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





