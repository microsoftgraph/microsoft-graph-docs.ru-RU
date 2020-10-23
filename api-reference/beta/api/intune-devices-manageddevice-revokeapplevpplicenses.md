---
title: Действие revokeAppleVppLicenses
description: Отзыв всех лицензий на Apple VPP для устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f65791e90913e257c4d7767b34be7b656910df12
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706711"
---
# <a name="revokeapplevpplicenses-action"></a><span data-ttu-id="7660a-103">Действие revokeAppleVppLicenses</span><span class="sxs-lookup"><span data-stu-id="7660a-103">revokeAppleVppLicenses action</span></span>

<span data-ttu-id="7660a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7660a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7660a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7660a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7660a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7660a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7660a-107">Отзыв всех лицензий на Apple VPP для устройства</span><span class="sxs-lookup"><span data-stu-id="7660a-107">Revoke all Apple Vpp licenses for a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7660a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7660a-108">Prerequisites</span></span>
<span data-ttu-id="7660a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7660a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7660a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7660a-111">Permission type</span></span>|<span data-ttu-id="7660a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7660a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7660a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7660a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7660a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7660a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="7660a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7660a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7660a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7660a-116">Not supported.</span></span>|
|<span data-ttu-id="7660a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7660a-117">Application</span></span>|<span data-ttu-id="7660a-118">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="7660a-118">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7660a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7660a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
POST /deviceManagement/comanagedDevices/{managedDeviceId}/revokeAppleVppLicenses
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/revokeAppleVppLicenses
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/revokeAppleVppLicenses
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/revokeAppleVppLicenses
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
```

## <a name="request-headers"></a><span data-ttu-id="7660a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7660a-120">Request headers</span></span>
|<span data-ttu-id="7660a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7660a-121">Header</span></span>|<span data-ttu-id="7660a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7660a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7660a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7660a-123">Authorization</span></span>|<span data-ttu-id="7660a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7660a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7660a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7660a-125">Accept</span></span>|<span data-ttu-id="7660a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7660a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7660a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7660a-127">Request body</span></span>
<span data-ttu-id="7660a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7660a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7660a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="7660a-129">Response</span></span>
<span data-ttu-id="7660a-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7660a-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7660a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7660a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7660a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7660a-132">Request</span></span>
<span data-ttu-id="7660a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7660a-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/revokeAppleVppLicenses
```

### <a name="response"></a><span data-ttu-id="7660a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7660a-134">Response</span></span>
<span data-ttu-id="7660a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7660a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





