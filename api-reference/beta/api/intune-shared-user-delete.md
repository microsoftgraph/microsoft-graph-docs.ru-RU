---
title: Удаление пользователя
description: Удаляет объект user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e2faa54999dbca660ce8bd3df7d4449fa4fa5d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999757"
---
# <a name="delete-user"></a><span data-ttu-id="faa77-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="faa77-103">Delete user</span></span>

<span data-ttu-id="faa77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faa77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="faa77-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="faa77-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faa77-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faa77-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faa77-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faa77-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa77-108">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="faa77-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="faa77-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="faa77-109">Prerequisites</span></span>
<span data-ttu-id="faa77-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="faa77-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="faa77-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faa77-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="faa77-112">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="faa77-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="faa77-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faa77-113">Permission type</span></span>|<span data-ttu-id="faa77-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="faa77-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faa77-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faa77-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="faa77-116">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="faa77-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="faa77-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="faa77-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="faa77-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="faa77-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="faa77-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="faa77-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="faa77-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="faa77-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="faa77-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="faa77-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="faa77-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faa77-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faa77-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faa77-125">Not supported.</span></span>|
|<span data-ttu-id="faa77-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faa77-126">Application</span></span>||
| <span data-ttu-id="faa77-127">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="faa77-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="faa77-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="faa77-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="faa77-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="faa77-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="faa77-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="faa77-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="faa77-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="faa77-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="faa77-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="faa77-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faa77-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="faa77-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faa77-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="faa77-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="faa77-136">Request headers</span></span>

|<span data-ttu-id="faa77-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faa77-137">Header</span></span>|<span data-ttu-id="faa77-138">Значение</span><span class="sxs-lookup"><span data-stu-id="faa77-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faa77-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="faa77-139">Authorization</span></span>|<span data-ttu-id="faa77-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faa77-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faa77-141">Accept</span><span class="sxs-lookup"><span data-stu-id="faa77-141">Accept</span></span>|<span data-ttu-id="faa77-142">application/json</span><span class="sxs-lookup"><span data-stu-id="faa77-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faa77-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="faa77-143">Request body</span></span>

<span data-ttu-id="faa77-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="faa77-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faa77-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="faa77-145">Response</span></span>

<span data-ttu-id="faa77-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="faa77-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="faa77-147">Пример</span><span class="sxs-lookup"><span data-stu-id="faa77-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="faa77-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="faa77-148">Request</span></span>

<span data-ttu-id="faa77-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="faa77-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="faa77-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="faa77-150">Response</span></span>

<span data-ttu-id="faa77-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="faa77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












