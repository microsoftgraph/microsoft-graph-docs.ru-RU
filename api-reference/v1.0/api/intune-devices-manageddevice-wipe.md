---
title: Действие wipe
description: Очистка устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56d29523f42f1948548bc9a3c16fd988a32ae6c4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364230"
---
# <a name="wipe-action"></a><span data-ttu-id="8bc16-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="8bc16-103">wipe action</span></span>

> <span data-ttu-id="8bc16-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bc16-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc16-105">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="8bc16-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bc16-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8bc16-106">Prerequisites</span></span>
<span data-ttu-id="8bc16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bc16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bc16-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bc16-109">Permission type</span></span>|<span data-ttu-id="8bc16-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bc16-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bc16-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bc16-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8bc16-112">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8bc16-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8bc16-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bc16-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bc16-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bc16-114">Not supported.</span></span>|
|<span data-ttu-id="8bc16-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bc16-115">Application</span></span>|<span data-ttu-id="8bc16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bc16-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bc16-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bc16-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="8bc16-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bc16-118">Request headers</span></span>
|<span data-ttu-id="8bc16-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bc16-119">Header</span></span>|<span data-ttu-id="8bc16-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8bc16-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bc16-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bc16-121">Authorization</span></span>|<span data-ttu-id="8bc16-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bc16-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bc16-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8bc16-123">Accept</span></span>|<span data-ttu-id="8bc16-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8bc16-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bc16-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bc16-125">Request body</span></span>
<span data-ttu-id="8bc16-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bc16-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8bc16-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8bc16-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8bc16-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bc16-128">Property</span></span>|<span data-ttu-id="8bc16-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8bc16-129">Type</span></span>|<span data-ttu-id="8bc16-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8bc16-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc16-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="8bc16-131">keepEnrollmentData</span></span>|<span data-ttu-id="8bc16-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bc16-132">Boolean</span></span>|<span data-ttu-id="8bc16-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8bc16-133">Not yet documented</span></span>|
|<span data-ttu-id="8bc16-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="8bc16-134">keepUserData</span></span>|<span data-ttu-id="8bc16-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bc16-135">Boolean</span></span>|<span data-ttu-id="8bc16-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8bc16-136">Not yet documented</span></span>|
|<span data-ttu-id="8bc16-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="8bc16-137">macOsUnlockCode</span></span>|<span data-ttu-id="8bc16-138">String</span><span class="sxs-lookup"><span data-stu-id="8bc16-138">String</span></span>|<span data-ttu-id="8bc16-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8bc16-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8bc16-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bc16-140">Response</span></span>
<span data-ttu-id="8bc16-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8bc16-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8bc16-142">Пример</span><span class="sxs-lookup"><span data-stu-id="8bc16-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bc16-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bc16-143">Request</span></span>
<span data-ttu-id="8bc16-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bc16-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="8bc16-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bc16-145">Response</span></span>
<span data-ttu-id="8bc16-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bc16-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




