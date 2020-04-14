---
title: Delete windows10GeneralConfiguration
description: Удаляет объект windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f26d4a5056ef691e14d618df48ed817f78f94b19
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431041"
---
# <a name="delete-windows10generalconfiguration"></a><span data-ttu-id="3a842-103">Delete windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="3a842-103">Delete windows10GeneralConfiguration</span></span>

<span data-ttu-id="3a842-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a842-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a842-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a842-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a842-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a842-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a842-107">Удаляет объект [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a842-107">Deletes a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a842-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3a842-108">Prerequisites</span></span>
<span data-ttu-id="3a842-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a842-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a842-111">Permission type</span></span>|<span data-ttu-id="3a842-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a842-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a842-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a842-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a842-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a842-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a842-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a842-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a842-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a842-116">Not supported.</span></span>|
|<span data-ttu-id="3a842-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a842-117">Application</span></span>|<span data-ttu-id="3a842-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a842-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a842-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a842-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3a842-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a842-120">Request headers</span></span>
|<span data-ttu-id="3a842-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a842-121">Header</span></span>|<span data-ttu-id="3a842-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a842-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a842-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a842-123">Authorization</span></span>|<span data-ttu-id="3a842-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a842-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a842-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a842-125">Accept</span></span>|<span data-ttu-id="3a842-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a842-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a842-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a842-127">Request body</span></span>
<span data-ttu-id="3a842-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a842-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a842-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a842-129">Response</span></span>
<span data-ttu-id="3a842-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a842-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a842-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3a842-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a842-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a842-132">Request</span></span>
<span data-ttu-id="3a842-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a842-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3a842-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a842-134">Response</span></span>
<span data-ttu-id="3a842-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a842-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



