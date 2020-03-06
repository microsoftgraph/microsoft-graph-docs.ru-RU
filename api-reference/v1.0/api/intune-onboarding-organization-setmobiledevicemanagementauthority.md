---
title: Действие setMobileDeviceManagementAuthority
description: Задание центра управления мобильными устройствами
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f8713d62ed082a368b915ca4e44706209f73ee7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512414"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="244dd-103">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="244dd-103">setMobileDeviceManagementAuthority action</span></span>

<span data-ttu-id="244dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="244dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="244dd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="244dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="244dd-106">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="244dd-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="244dd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="244dd-107">Prerequisites</span></span>
<span data-ttu-id="244dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="244dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="244dd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="244dd-110">Permission type</span></span>|<span data-ttu-id="244dd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="244dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="244dd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="244dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="244dd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="244dd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="244dd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="244dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="244dd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="244dd-115">Not supported.</span></span>|
|<span data-ttu-id="244dd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="244dd-116">Application</span></span>|<span data-ttu-id="244dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="244dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="244dd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="244dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="244dd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="244dd-119">Request headers</span></span>
|<span data-ttu-id="244dd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="244dd-120">Header</span></span>|<span data-ttu-id="244dd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="244dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="244dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="244dd-122">Authorization</span></span>|<span data-ttu-id="244dd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="244dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="244dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="244dd-124">Accept</span></span>|<span data-ttu-id="244dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="244dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="244dd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="244dd-126">Request body</span></span>
<span data-ttu-id="244dd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="244dd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="244dd-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="244dd-128">Response</span></span>
<span data-ttu-id="244dd-129">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="244dd-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="244dd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="244dd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="244dd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="244dd-131">Request</span></span>
<span data-ttu-id="244dd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="244dd-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="244dd-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="244dd-133">Response</span></span>
<span data-ttu-id="244dd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="244dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```




