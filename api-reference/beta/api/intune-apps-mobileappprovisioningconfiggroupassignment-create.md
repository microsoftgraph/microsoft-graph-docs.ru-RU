---
title: Создание К mobileappprovisioningconfiggroupassignment.
description: Создание нового объекта К mobileappprovisioningconfiggroupassignment..
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6684046b6587838370ae01349a0e0cf6a962b814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444947"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="1eafe-103">Создание К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="1eafe-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="1eafe-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1eafe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1eafe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1eafe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eafe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1eafe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eafe-107">Создание нового объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1eafe-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1eafe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1eafe-108">Prerequisites</span></span>
<span data-ttu-id="1eafe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eafe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1eafe-111">Permission type</span></span>|<span data-ttu-id="1eafe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1eafe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1eafe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1eafe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1eafe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eafe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1eafe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1eafe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1eafe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1eafe-116">Not supported.</span></span>|
|<span data-ttu-id="1eafe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1eafe-117">Application</span></span>|<span data-ttu-id="1eafe-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eafe-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1eafe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1eafe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="1eafe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1eafe-120">Request headers</span></span>
|<span data-ttu-id="1eafe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1eafe-121">Header</span></span>|<span data-ttu-id="1eafe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1eafe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1eafe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1eafe-123">Authorization</span></span>|<span data-ttu-id="1eafe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1eafe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1eafe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1eafe-125">Accept</span></span>|<span data-ttu-id="1eafe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1eafe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eafe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1eafe-127">Request body</span></span>
<span data-ttu-id="1eafe-128">В тексте запроса добавьте представление объекта К mobileappprovisioningconfiggroupassignment. в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1eafe-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="1eafe-129">В следующей таблице приведены свойства, необходимые при создании К mobileappprovisioningconfiggroupassignment..</span><span class="sxs-lookup"><span data-stu-id="1eafe-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="1eafe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1eafe-130">Property</span></span>|<span data-ttu-id="1eafe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1eafe-131">Type</span></span>|<span data-ttu-id="1eafe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1eafe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1eafe-133">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="1eafe-133">targetGroupId</span></span>|<span data-ttu-id="1eafe-134">String</span><span class="sxs-lookup"><span data-stu-id="1eafe-134">String</span></span>|<span data-ttu-id="1eafe-135">Идентификатор группы AAD, в которой нацелена конфигурация подготовки приложений.</span><span class="sxs-lookup"><span data-stu-id="1eafe-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="1eafe-136">id</span><span class="sxs-lookup"><span data-stu-id="1eafe-136">id</span></span>|<span data-ttu-id="1eafe-137">String</span><span class="sxs-lookup"><span data-stu-id="1eafe-137">String</span></span>|<span data-ttu-id="1eafe-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1eafe-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1eafe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1eafe-139">Response</span></span>
<span data-ttu-id="1eafe-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1eafe-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eafe-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1eafe-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1eafe-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1eafe-142">Request</span></span>
<span data-ttu-id="1eafe-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1eafe-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="1eafe-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1eafe-144">Response</span></span>
<span data-ttu-id="1eafe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1eafe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```





