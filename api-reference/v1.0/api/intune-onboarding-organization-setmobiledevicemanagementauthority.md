---
title: Действие setMobileDeviceManagementAuthority
description: Задание центра управления мобильными устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4b808567295816595267b12fe7d69fdc8a357ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087273"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="5db81-103">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="5db81-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="5db81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5db81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5db81-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5db81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5db81-106">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="5db81-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5db81-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5db81-107">Prerequisites</span></span>
<span data-ttu-id="5db81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5db81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5db81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5db81-110">Permission type</span></span>|<span data-ttu-id="5db81-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5db81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5db81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5db81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5db81-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5db81-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5db81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5db81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5db81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db81-115">Not supported.</span></span>|
|<span data-ttu-id="5db81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5db81-116">Application</span></span>|<span data-ttu-id="5db81-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5db81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5db81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="5db81-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5db81-119">Request headers</span></span>
|<span data-ttu-id="5db81-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5db81-120">Header</span></span>|<span data-ttu-id="5db81-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5db81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5db81-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5db81-122">Authorization</span></span>|<span data-ttu-id="5db81-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5db81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5db81-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5db81-124">Accept</span></span>|<span data-ttu-id="5db81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5db81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5db81-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5db81-126">Request body</span></span>
<span data-ttu-id="5db81-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5db81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5db81-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db81-128">Response</span></span>
<span data-ttu-id="5db81-129">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5db81-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db81-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5db81-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5db81-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5db81-131">Request</span></span>
<span data-ttu-id="5db81-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5db81-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="5db81-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db81-133">Response</span></span>
<span data-ttu-id="5db81-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5db81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```









