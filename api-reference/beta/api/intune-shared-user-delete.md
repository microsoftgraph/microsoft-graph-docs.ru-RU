---
title: Удаление пользователя
description: Удаляет объект user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdb17f2610d7e4f0634e2809bd500c40f6f32557
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458079"
---
# <a name="delete-user"></a><span data-ttu-id="d7535-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="d7535-103">Delete user</span></span>

<span data-ttu-id="d7535-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d7535-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7535-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7535-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d7535-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7535-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7535-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7535-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7535-108">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d7535-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7535-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7535-109">Prerequisites</span></span>
<span data-ttu-id="d7535-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="d7535-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d7535-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7535-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="d7535-112">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="d7535-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="d7535-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7535-113">Permission type</span></span>|<span data-ttu-id="d7535-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7535-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7535-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7535-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d7535-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d7535-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d7535-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d7535-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d7535-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d7535-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d7535-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d7535-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d7535-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d7535-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d7535-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d7535-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d7535-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7535-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7535-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7535-125">Not supported.</span></span>|
|<span data-ttu-id="d7535-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7535-126">Application</span></span>||
| <span data-ttu-id="d7535-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d7535-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d7535-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d7535-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d7535-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d7535-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d7535-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d7535-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d7535-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d7535-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d7535-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d7535-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7535-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7535-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7535-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d7535-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7535-136">Request headers</span></span>

|<span data-ttu-id="d7535-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7535-137">Header</span></span>|<span data-ttu-id="d7535-138">Значение</span><span class="sxs-lookup"><span data-stu-id="d7535-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7535-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7535-139">Authorization</span></span>|<span data-ttu-id="d7535-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7535-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7535-141">Accept</span><span class="sxs-lookup"><span data-stu-id="d7535-141">Accept</span></span>|<span data-ttu-id="d7535-142">application/json</span><span class="sxs-lookup"><span data-stu-id="d7535-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7535-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7535-143">Request body</span></span>

<span data-ttu-id="d7535-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7535-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7535-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7535-145">Response</span></span>

<span data-ttu-id="d7535-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d7535-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d7535-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d7535-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7535-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7535-148">Request</span></span>

<span data-ttu-id="d7535-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7535-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="d7535-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7535-150">Response</span></span>

<span data-ttu-id="d7535-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7535-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```











