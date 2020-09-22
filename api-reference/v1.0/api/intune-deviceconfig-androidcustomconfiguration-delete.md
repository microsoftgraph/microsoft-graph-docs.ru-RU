---
title: Delete androidCustomConfiguration
description: Удаляет объект androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df04b40b48529fd07c21ed4416b49cef92ef7a80
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985526"
---
# <a name="delete-androidcustomconfiguration"></a><span data-ttu-id="5bb62-103">Delete androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="5bb62-103">Delete androidCustomConfiguration</span></span>

<span data-ttu-id="5bb62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bb62-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bb62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb62-106">Удаляет объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bb62-106">Deletes a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bb62-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5bb62-107">Prerequisites</span></span>
<span data-ttu-id="5bb62-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bb62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb62-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bb62-110">Permission type</span></span>|<span data-ttu-id="5bb62-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bb62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb62-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bb62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bb62-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bb62-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5bb62-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bb62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb62-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bb62-115">Not supported.</span></span>|
|<span data-ttu-id="5bb62-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bb62-116">Application</span></span>|<span data-ttu-id="5bb62-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bb62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb62-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bb62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5bb62-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5bb62-119">Request headers</span></span>
|<span data-ttu-id="5bb62-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bb62-120">Header</span></span>|<span data-ttu-id="5bb62-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5bb62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bb62-122">Authorization</span></span>|<span data-ttu-id="5bb62-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bb62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb62-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5bb62-124">Accept</span></span>|<span data-ttu-id="5bb62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb62-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bb62-126">Request body</span></span>
<span data-ttu-id="5bb62-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bb62-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bb62-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bb62-128">Response</span></span>
<span data-ttu-id="5bb62-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5bb62-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5bb62-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5bb62-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bb62-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bb62-131">Request</span></span>
<span data-ttu-id="5bb62-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bb62-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5bb62-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bb62-133">Response</span></span>
<span data-ttu-id="5bb62-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bb62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









