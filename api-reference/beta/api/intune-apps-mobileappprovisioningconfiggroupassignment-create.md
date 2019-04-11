---
title: Создание К mobileappprovisioningconfiggroupassignment.
description: Создание нового объекта К mobileappprovisioningconfiggroupassignment..
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 155dff65bae47b5486e49fcbf268da5ab453f701
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790342"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="ffafe-103">Создание К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="ffafe-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="ffafe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffafe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffafe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffafe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffafe-106">Создание нового объекта [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ffafe-106">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffafe-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ffafe-107">Prerequisites</span></span>
<span data-ttu-id="ffafe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffafe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffafe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffafe-110">Permission type</span></span>|<span data-ttu-id="ffafe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffafe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffafe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffafe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffafe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffafe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ffafe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffafe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffafe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffafe-115">Not supported.</span></span>|
|<span data-ttu-id="ffafe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffafe-116">Application</span></span>|<span data-ttu-id="ffafe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffafe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffafe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffafe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ffafe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffafe-119">Request headers</span></span>
|<span data-ttu-id="ffafe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffafe-120">Header</span></span>|<span data-ttu-id="ffafe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ffafe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffafe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffafe-122">Authorization</span></span>|<span data-ttu-id="ffafe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffafe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffafe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ffafe-124">Accept</span></span>|<span data-ttu-id="ffafe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffafe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffafe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffafe-126">Request body</span></span>
<span data-ttu-id="ffafe-127">В тексте запроса добавьте представление объекта К mobileappprovisioningconfiggroupassignment. в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffafe-127">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="ffafe-128">В следующей таблице приведены свойства, необходимые при создании К mobileappprovisioningconfiggroupassignment..</span><span class="sxs-lookup"><span data-stu-id="ffafe-128">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="ffafe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffafe-129">Property</span></span>|<span data-ttu-id="ffafe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ffafe-130">Type</span></span>|<span data-ttu-id="ffafe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ffafe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffafe-132">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="ffafe-132">targetGroupId</span></span>|<span data-ttu-id="ffafe-133">String</span><span class="sxs-lookup"><span data-stu-id="ffafe-133">String</span></span>|<span data-ttu-id="ffafe-134">Идентификатор группы AAD, в которой нацелена конфигурация подготовки приложений.</span><span class="sxs-lookup"><span data-stu-id="ffafe-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="ffafe-135">id</span><span class="sxs-lookup"><span data-stu-id="ffafe-135">id</span></span>|<span data-ttu-id="ffafe-136">String</span><span class="sxs-lookup"><span data-stu-id="ffafe-136">String</span></span>|<span data-ttu-id="ffafe-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffafe-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ffafe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffafe-138">Response</span></span>
<span data-ttu-id="ffafe-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffafe-139">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffafe-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ffafe-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffafe-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffafe-141">Request</span></span>
<span data-ttu-id="ffafe-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffafe-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="ffafe-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffafe-143">Response</span></span>
<span data-ttu-id="ffafe-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffafe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





