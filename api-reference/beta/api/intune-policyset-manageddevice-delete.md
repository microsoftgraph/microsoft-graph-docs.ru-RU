---
title: Delete managedDevice
description: Удаляет объект managedDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64fb894984a577f3332cce66c8f698e2818de7b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160589"
---
# <a name="delete-manageddevice"></a><span data-ttu-id="49f24-103">Delete managedDevice</span><span class="sxs-lookup"><span data-stu-id="49f24-103">Delete managedDevice</span></span>

<span data-ttu-id="49f24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49f24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49f24-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49f24-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49f24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49f24-107">Удаляет объект [managedDevice](../resources/intune-shared-manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="49f24-107">Deletes a [managedDevice](../resources/intune-shared-manageddevice.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49f24-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="49f24-108">Prerequisites</span></span>
<span data-ttu-id="49f24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49f24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49f24-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49f24-111">Permission type</span></span>|<span data-ttu-id="49f24-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49f24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49f24-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49f24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49f24-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f24-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49f24-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49f24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49f24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49f24-116">Not supported.</span></span>|
|<span data-ttu-id="49f24-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49f24-117">Application</span></span>|<span data-ttu-id="49f24-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49f24-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49f24-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49f24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="49f24-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49f24-120">Request headers</span></span>
|<span data-ttu-id="49f24-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49f24-121">Header</span></span>|<span data-ttu-id="49f24-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49f24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49f24-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49f24-123">Authorization</span></span>|<span data-ttu-id="49f24-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49f24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49f24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49f24-125">Accept</span></span>|<span data-ttu-id="49f24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49f24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49f24-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49f24-127">Request body</span></span>
<span data-ttu-id="49f24-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49f24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49f24-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f24-129">Response</span></span>
<span data-ttu-id="49f24-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49f24-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="49f24-131">Пример</span><span class="sxs-lookup"><span data-stu-id="49f24-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="49f24-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="49f24-132">Request</span></span>
<span data-ttu-id="49f24-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49f24-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
```

### <a name="response"></a><span data-ttu-id="49f24-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="49f24-134">Response</span></span>
<span data-ttu-id="49f24-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49f24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




