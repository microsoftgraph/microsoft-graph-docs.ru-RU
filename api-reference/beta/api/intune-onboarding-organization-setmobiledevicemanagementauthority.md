---
title: Действие setMobileDeviceManagementAuthority
description: Задание центра управления мобильными устройствами
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 975891da8d0f8f5677d73d39577f114bb1eafe2f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899930"
---
# <a name="setmobiledevicemanagementauthority-action"></a><span data-ttu-id="bec4e-103">Действие setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="bec4e-103">setMobileDeviceManagementAuthority action</span></span>

> <span data-ttu-id="bec4e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bec4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bec4e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bec4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bec4e-106">Задание центра управления мобильными устройствами</span><span class="sxs-lookup"><span data-stu-id="bec4e-106">Set mobile device management authority</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bec4e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bec4e-107">Prerequisites</span></span>
<span data-ttu-id="bec4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bec4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bec4e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bec4e-110">Permission type</span></span>|<span data-ttu-id="bec4e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bec4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bec4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bec4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bec4e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bec4e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bec4e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bec4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bec4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bec4e-115">Not supported.</span></span>|
|<span data-ttu-id="bec4e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bec4e-116">Application</span></span>|<span data-ttu-id="bec4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bec4e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bec4e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bec4e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/setMobileDeviceManagementAuthority
```

## <a name="request-headers"></a><span data-ttu-id="bec4e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bec4e-119">Request headers</span></span>
|<span data-ttu-id="bec4e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bec4e-120">Header</span></span>|<span data-ttu-id="bec4e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bec4e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bec4e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bec4e-122">Authorization</span></span>|<span data-ttu-id="bec4e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bec4e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bec4e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bec4e-124">Accept</span></span>|<span data-ttu-id="bec4e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bec4e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bec4e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bec4e-126">Request body</span></span>
<span data-ttu-id="bec4e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bec4e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bec4e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bec4e-128">Response</span></span>
<span data-ttu-id="bec4e-129">При успешном выполнении это действие возвращает код отклика `200 OK` и объект Int32 в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bec4e-129">If successful, this action returns a `200 OK` response code and a Int32 in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bec4e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bec4e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bec4e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bec4e-131">Request</span></span>
<span data-ttu-id="bec4e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bec4e-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/organization/{organizationId}/setMobileDeviceManagementAuthority
```

### <a name="response"></a><span data-ttu-id="bec4e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bec4e-133">Response</span></span>
<span data-ttu-id="bec4e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bec4e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 18

{
  "value": 2
}
```




