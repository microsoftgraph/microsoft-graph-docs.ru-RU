---
title: Удалить iosMobileAppConfiguration
description: Удаляет iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bbb6b8932f75063ac4092d6034d2ee681be90953
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757383"
---
# <a name="delete-iosmobileappconfiguration"></a><span data-ttu-id="6d4da-103">Удалить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d4da-103">Delete iosMobileAppConfiguration</span></span>

<span data-ttu-id="6d4da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d4da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d4da-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d4da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d4da-106">Удаляет [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d4da-106">Deletes a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d4da-107">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="6d4da-107">Prerequisites</span></span>
<span data-ttu-id="6d4da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d4da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d4da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d4da-110">Permission type</span></span>|<span data-ttu-id="6d4da-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d4da-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d4da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d4da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d4da-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d4da-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d4da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d4da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d4da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d4da-115">Not supported.</span></span>|
|<span data-ttu-id="6d4da-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d4da-116">Application</span></span>|<span data-ttu-id="6d4da-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d4da-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d4da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d4da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6d4da-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6d4da-119">Request headers</span></span>
|<span data-ttu-id="6d4da-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d4da-120">Header</span></span>|<span data-ttu-id="6d4da-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6d4da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d4da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d4da-122">Authorization</span></span>|<span data-ttu-id="6d4da-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d4da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d4da-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6d4da-124">Accept</span></span>|<span data-ttu-id="6d4da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d4da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d4da-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d4da-126">Request body</span></span>
<span data-ttu-id="6d4da-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d4da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d4da-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d4da-128">Response</span></span>
<span data-ttu-id="6d4da-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6d4da-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d4da-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6d4da-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d4da-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d4da-131">Request</span></span>
<span data-ttu-id="6d4da-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d4da-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6d4da-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d4da-133">Response</span></span>
<span data-ttu-id="6d4da-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d4da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




