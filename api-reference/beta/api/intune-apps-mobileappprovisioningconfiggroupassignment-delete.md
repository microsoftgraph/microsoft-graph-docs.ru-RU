---
title: Удаление К mobileappprovisioningconfiggroupassignment.
description: Удаляет объект К mobileappprovisioningconfiggroupassignment..
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 090965e321696ab328e741fd3011f1c860c55d1b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248240"
---
# <a name="delete-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="c986d-103">Удаление К mobileappprovisioningconfiggroupassignment.</span><span class="sxs-lookup"><span data-stu-id="c986d-103">Delete mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="c986d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c986d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c986d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c986d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c986d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c986d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c986d-107">Удаляет объект [к mobileappprovisioningconfiggroupassignment.](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c986d-107">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c986d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c986d-108">Prerequisites</span></span>
<span data-ttu-id="c986d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c986d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c986d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c986d-111">Permission type</span></span>|<span data-ttu-id="c986d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c986d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c986d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c986d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c986d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c986d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c986d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c986d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c986d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c986d-116">Not supported.</span></span>|
|<span data-ttu-id="c986d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c986d-117">Application</span></span>|<span data-ttu-id="c986d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c986d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c986d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c986d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c986d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c986d-120">Request headers</span></span>
|<span data-ttu-id="c986d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c986d-121">Header</span></span>|<span data-ttu-id="c986d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c986d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c986d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c986d-123">Authorization</span></span>|<span data-ttu-id="c986d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c986d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c986d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c986d-125">Accept</span></span>|<span data-ttu-id="c986d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c986d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c986d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c986d-127">Request body</span></span>
<span data-ttu-id="c986d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c986d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c986d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c986d-129">Response</span></span>
<span data-ttu-id="c986d-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c986d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c986d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c986d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c986d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c986d-132">Request</span></span>
<span data-ttu-id="c986d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c986d-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c986d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c986d-134">Response</span></span>
<span data-ttu-id="c986d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c986d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




