---
title: Удаление iosEnterpriseWiFiConfiguration
description: Удаляет объект iosEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eba198978161afa2125c34cd351dbfede5364632
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731262"
---
# <a name="delete-iosenterprisewificonfiguration"></a><span data-ttu-id="1f58e-103">Удаление iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f58e-103">Delete iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="1f58e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f58e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f58e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f58e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f58e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f58e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f58e-107">Удаляет объект [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f58e-107">Deletes a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f58e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f58e-108">Prerequisites</span></span>
<span data-ttu-id="1f58e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f58e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f58e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f58e-111">Permission type</span></span>|<span data-ttu-id="1f58e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f58e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f58e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f58e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f58e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f58e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f58e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f58e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f58e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f58e-116">Not supported.</span></span>|
|<span data-ttu-id="1f58e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f58e-117">Application</span></span>|<span data-ttu-id="1f58e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f58e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f58e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f58e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1f58e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f58e-120">Request headers</span></span>
|<span data-ttu-id="1f58e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f58e-121">Header</span></span>|<span data-ttu-id="1f58e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f58e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f58e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f58e-123">Authorization</span></span>|<span data-ttu-id="1f58e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f58e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f58e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f58e-125">Accept</span></span>|<span data-ttu-id="1f58e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f58e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f58e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f58e-127">Request body</span></span>
<span data-ttu-id="1f58e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f58e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f58e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f58e-129">Response</span></span>
<span data-ttu-id="1f58e-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1f58e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f58e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1f58e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f58e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f58e-132">Request</span></span>
<span data-ttu-id="1f58e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f58e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1f58e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f58e-134">Response</span></span>
<span data-ttu-id="1f58e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f58e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





