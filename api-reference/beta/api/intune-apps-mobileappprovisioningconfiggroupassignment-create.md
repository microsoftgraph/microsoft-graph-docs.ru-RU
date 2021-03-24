---
title: Создание mobileAppProvisioningConfigGroupAssignment
description: Создание нового объекта mobileAppProvisioningConfigGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 173f8704ffb44750e3ef382160363dc6e1ce2e48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139687"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="38a97-103">Создание mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="38a97-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="38a97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38a97-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38a97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38a97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38a97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a97-107">Создание нового [объекта mobileAppProvisioningConfigGroupAssignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="38a97-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38a97-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38a97-108">Prerequisites</span></span>
<span data-ttu-id="38a97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38a97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38a97-111">Permission type</span></span>|<span data-ttu-id="38a97-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38a97-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38a97-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38a97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38a97-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a97-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38a97-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38a97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38a97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38a97-116">Not supported.</span></span>|
|<span data-ttu-id="38a97-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="38a97-117">Application</span></span>|<span data-ttu-id="38a97-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38a97-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38a97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38a97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="38a97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38a97-120">Request headers</span></span>
|<span data-ttu-id="38a97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38a97-121">Header</span></span>|<span data-ttu-id="38a97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="38a97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38a97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38a97-123">Authorization</span></span>|<span data-ttu-id="38a97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38a97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38a97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38a97-125">Accept</span></span>|<span data-ttu-id="38a97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38a97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38a97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38a97-127">Request body</span></span>
<span data-ttu-id="38a97-128">В теле запроса поставляем представление JSON для объекта mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="38a97-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="38a97-129">В следующей таблице показаны свойства, необходимые при создании mobileAppProvisioningConfigGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="38a97-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="38a97-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="38a97-130">Property</span></span>|<span data-ttu-id="38a97-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38a97-131">Type</span></span>|<span data-ttu-id="38a97-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38a97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38a97-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="38a97-133">targetGroupId</span></span>|<span data-ttu-id="38a97-134">Строка</span><span class="sxs-lookup"><span data-stu-id="38a97-134">String</span></span>|<span data-ttu-id="38a97-135">ID группы AAD, в которой ориентирована конфигурация подготовка приложений.</span><span class="sxs-lookup"><span data-stu-id="38a97-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="38a97-136">id</span><span class="sxs-lookup"><span data-stu-id="38a97-136">id</span></span>|<span data-ttu-id="38a97-137">Строка</span><span class="sxs-lookup"><span data-stu-id="38a97-137">String</span></span>|<span data-ttu-id="38a97-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38a97-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="38a97-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a97-139">Response</span></span>
<span data-ttu-id="38a97-140">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="38a97-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38a97-141">Пример</span><span class="sxs-lookup"><span data-stu-id="38a97-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="38a97-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="38a97-142">Request</span></span>
<span data-ttu-id="38a97-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38a97-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="38a97-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a97-144">Response</span></span>
<span data-ttu-id="38a97-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38a97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




