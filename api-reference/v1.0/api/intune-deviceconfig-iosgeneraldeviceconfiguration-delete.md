---
title: Delete iosGeneralDeviceConfiguration
description: Удаляет объект iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 898f7bdce43525f50db70c9bc6317d6c86052066
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756339"
---
# <a name="delete-iosgeneraldeviceconfiguration"></a><span data-ttu-id="46d18-103">Delete iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="46d18-103">Delete iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="46d18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46d18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46d18-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46d18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46d18-106">Удаляет объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46d18-106">Deletes a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46d18-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="46d18-107">Prerequisites</span></span>
<span data-ttu-id="46d18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46d18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46d18-110">Permission type</span></span>|<span data-ttu-id="46d18-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46d18-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46d18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46d18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46d18-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d18-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46d18-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46d18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46d18-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46d18-115">Not supported.</span></span>|
|<span data-ttu-id="46d18-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="46d18-116">Application</span></span>|<span data-ttu-id="46d18-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d18-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46d18-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46d18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="46d18-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46d18-119">Request headers</span></span>
|<span data-ttu-id="46d18-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46d18-120">Header</span></span>|<span data-ttu-id="46d18-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46d18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46d18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46d18-122">Authorization</span></span>|<span data-ttu-id="46d18-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46d18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46d18-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46d18-124">Accept</span></span>|<span data-ttu-id="46d18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46d18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d18-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46d18-126">Request body</span></span>
<span data-ttu-id="46d18-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46d18-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46d18-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="46d18-128">Response</span></span>
<span data-ttu-id="46d18-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46d18-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="46d18-130">Пример</span><span class="sxs-lookup"><span data-stu-id="46d18-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46d18-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="46d18-131">Request</span></span>
<span data-ttu-id="46d18-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46d18-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="46d18-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="46d18-133">Response</span></span>
<span data-ttu-id="46d18-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46d18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




