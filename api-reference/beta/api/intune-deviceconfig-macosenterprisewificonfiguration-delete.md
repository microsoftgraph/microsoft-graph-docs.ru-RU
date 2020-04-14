---
title: Удаление macOSEnterpriseWiFiConfiguration
description: Удаляет объект macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4179b0f27e7894e60d20f7f8ef34938a2aba142
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438004"
---
# <a name="delete-macosenterprisewificonfiguration"></a><span data-ttu-id="f7554-103">Удаление macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7554-103">Delete macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="f7554-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7554-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7554-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7554-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7554-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7554-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7554-107">Удаляет объект [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7554-107">Deletes a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7554-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f7554-108">Prerequisites</span></span>
<span data-ttu-id="f7554-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7554-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7554-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7554-111">Permission type</span></span>|<span data-ttu-id="f7554-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7554-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7554-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7554-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7554-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7554-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7554-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7554-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7554-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7554-116">Not supported.</span></span>|
|<span data-ttu-id="f7554-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f7554-117">Application</span></span>|<span data-ttu-id="f7554-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7554-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7554-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7554-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7554-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7554-120">Request headers</span></span>
|<span data-ttu-id="f7554-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7554-121">Header</span></span>|<span data-ttu-id="f7554-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f7554-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7554-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7554-123">Authorization</span></span>|<span data-ttu-id="f7554-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7554-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7554-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7554-125">Accept</span></span>|<span data-ttu-id="f7554-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7554-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7554-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7554-127">Request body</span></span>
<span data-ttu-id="f7554-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7554-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7554-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7554-129">Response</span></span>
<span data-ttu-id="f7554-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f7554-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7554-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f7554-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7554-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7554-132">Request</span></span>
<span data-ttu-id="f7554-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7554-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f7554-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7554-134">Response</span></span>
<span data-ttu-id="f7554-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7554-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



