---
title: Действие wipe
description: Очистка устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23d4d9536c57d4a9f2af863473b85d2062a06b3a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259159"
---
# <a name="wipe-action"></a><span data-ttu-id="dc624-103">Действие wipe</span><span class="sxs-lookup"><span data-stu-id="dc624-103">wipe action</span></span>

> <span data-ttu-id="dc624-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc624-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc624-105">Очистка устройства</span><span class="sxs-lookup"><span data-stu-id="dc624-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc624-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dc624-106">Prerequisites</span></span>
<span data-ttu-id="dc624-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc624-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc624-109">Permission type</span></span>|<span data-ttu-id="dc624-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc624-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc624-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc624-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc624-112">DeviceManagementManagedDevices. Привилижедоператион. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dc624-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dc624-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc624-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc624-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc624-114">Not supported.</span></span>|
|<span data-ttu-id="dc624-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc624-115">Application</span></span>|<span data-ttu-id="dc624-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc624-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc624-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc624-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="dc624-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc624-118">Request headers</span></span>
|<span data-ttu-id="dc624-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc624-119">Header</span></span>|<span data-ttu-id="dc624-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dc624-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc624-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc624-121">Authorization</span></span>|<span data-ttu-id="dc624-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc624-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc624-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc624-123">Accept</span></span>|<span data-ttu-id="dc624-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc624-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc624-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc624-125">Request body</span></span>
<span data-ttu-id="dc624-126">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc624-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dc624-127">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dc624-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dc624-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc624-128">Property</span></span>|<span data-ttu-id="dc624-129">Тип</span><span class="sxs-lookup"><span data-stu-id="dc624-129">Type</span></span>|<span data-ttu-id="dc624-130">Описание</span><span class="sxs-lookup"><span data-stu-id="dc624-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc624-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="dc624-131">keepEnrollmentData</span></span>|<span data-ttu-id="dc624-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc624-132">Boolean</span></span>|<span data-ttu-id="dc624-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dc624-133">Not yet documented</span></span>|
|<span data-ttu-id="dc624-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="dc624-134">keepUserData</span></span>|<span data-ttu-id="dc624-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc624-135">Boolean</span></span>|<span data-ttu-id="dc624-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dc624-136">Not yet documented</span></span>|
|<span data-ttu-id="dc624-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="dc624-137">macOsUnlockCode</span></span>|<span data-ttu-id="dc624-138">String</span><span class="sxs-lookup"><span data-stu-id="dc624-138">String</span></span>|<span data-ttu-id="dc624-139">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc624-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="dc624-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc624-140">Response</span></span>
<span data-ttu-id="dc624-141">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc624-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc624-142">Пример</span><span class="sxs-lookup"><span data-stu-id="dc624-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc624-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc624-143">Request</span></span>
<span data-ttu-id="dc624-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc624-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc624-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc624-145">Response</span></span>
<span data-ttu-id="dc624-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dc624-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



