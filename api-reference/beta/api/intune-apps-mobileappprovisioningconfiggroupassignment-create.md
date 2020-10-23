---
title: Создание К mobileappprovisioningconfiggroupassignment.
description: Создание нового объекта К mobileappprovisioningconfiggroupassignment..
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ef52e33a898e99187d7e7692403d4f9b88243d3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723695"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="72777-103">Создание К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="72777-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="72777-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72777-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72777-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72777-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72777-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72777-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72777-107">Создание нового объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="72777-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72777-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72777-108">Prerequisites</span></span>
<span data-ttu-id="72777-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72777-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72777-111">Permission type</span></span>|<span data-ttu-id="72777-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72777-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72777-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72777-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72777-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72777-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72777-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72777-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72777-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72777-116">Not supported.</span></span>|
|<span data-ttu-id="72777-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72777-117">Application</span></span>|<span data-ttu-id="72777-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72777-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72777-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72777-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="72777-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72777-120">Request headers</span></span>
|<span data-ttu-id="72777-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72777-121">Header</span></span>|<span data-ttu-id="72777-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72777-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72777-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72777-123">Authorization</span></span>|<span data-ttu-id="72777-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72777-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72777-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72777-125">Accept</span></span>|<span data-ttu-id="72777-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72777-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72777-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72777-127">Request body</span></span>
<span data-ttu-id="72777-128">В тексте запроса добавьте представление объекта К mobileappprovisioningconfiggroupassignment. в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72777-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="72777-129">В следующей таблице приведены свойства, необходимые при создании К mobileappprovisioningconfiggroupassignment..</span><span class="sxs-lookup"><span data-stu-id="72777-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="72777-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72777-130">Property</span></span>|<span data-ttu-id="72777-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72777-131">Type</span></span>|<span data-ttu-id="72777-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72777-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72777-133">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="72777-133">targetGroupId</span></span>|<span data-ttu-id="72777-134">Строка</span><span class="sxs-lookup"><span data-stu-id="72777-134">String</span></span>|<span data-ttu-id="72777-135">Идентификатор группы AAD, в которой нацелена конфигурация подготовки приложений.</span><span class="sxs-lookup"><span data-stu-id="72777-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="72777-136">id</span><span class="sxs-lookup"><span data-stu-id="72777-136">id</span></span>|<span data-ttu-id="72777-137">Строка</span><span class="sxs-lookup"><span data-stu-id="72777-137">String</span></span>|<span data-ttu-id="72777-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72777-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="72777-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="72777-139">Response</span></span>
<span data-ttu-id="72777-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72777-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72777-141">Пример</span><span class="sxs-lookup"><span data-stu-id="72777-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="72777-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="72777-142">Request</span></span>
<span data-ttu-id="72777-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72777-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="72777-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="72777-144">Response</span></span>
<span data-ttu-id="72777-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72777-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





