---
title: Удаление К mobileappprovisioningconfiggroupassignment.
description: Удаляет объект К mobileappprovisioningconfiggroupassignment..
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f49da55ba4f2f00c1da57c975f690841e5ec1b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977098"
---
# <a name="delete-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="eaf04-103">Удаление К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="eaf04-103">Delete mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="eaf04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaf04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaf04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaf04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaf04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaf04-107">Удаляет объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eaf04-107">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaf04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eaf04-108">Prerequisites</span></span>
<span data-ttu-id="eaf04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf04-111">Permission type</span></span>|<span data-ttu-id="eaf04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaf04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaf04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaf04-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf04-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eaf04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaf04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf04-116">Not supported.</span></span>|
|<span data-ttu-id="eaf04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaf04-117">Application</span></span>|<span data-ttu-id="eaf04-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf04-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaf04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="eaf04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eaf04-120">Request headers</span></span>
|<span data-ttu-id="eaf04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaf04-121">Header</span></span>|<span data-ttu-id="eaf04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eaf04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaf04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaf04-123">Authorization</span></span>|<span data-ttu-id="eaf04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaf04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaf04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eaf04-125">Accept</span></span>|<span data-ttu-id="eaf04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaf04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eaf04-127">Request body</span></span>
<span data-ttu-id="eaf04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eaf04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaf04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf04-129">Response</span></span>
<span data-ttu-id="eaf04-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eaf04-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eaf04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="eaf04-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaf04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaf04-132">Request</span></span>
<span data-ttu-id="eaf04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaf04-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="eaf04-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf04-134">Response</span></span>
<span data-ttu-id="eaf04-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaf04-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






