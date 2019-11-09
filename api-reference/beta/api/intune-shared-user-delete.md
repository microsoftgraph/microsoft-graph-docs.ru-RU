---
title: Удаление пользователя
description: Удаляет объект user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b856ecf5ab486b717d4bf4d861d94c6536c1eca2
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085593"
---
# <a name="delete-user"></a><span data-ttu-id="f207e-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="f207e-103">Delete user</span></span>

> <span data-ttu-id="f207e-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f207e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f207e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f207e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f207e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f207e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f207e-107">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="f207e-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f207e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f207e-108">Prerequisites</span></span>
<span data-ttu-id="f207e-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="f207e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f207e-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f207e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f207e-111">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="f207e-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="f207e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f207e-112">Permission type</span></span>|<span data-ttu-id="f207e-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f207e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f207e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f207e-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f207e-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f207e-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f207e-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f207e-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f207e-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f207e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f207e-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f207e-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f207e-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="f207e-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f207e-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f207e-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f207e-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f207e-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f207e-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f207e-124">Not supported.</span></span>|
|<span data-ttu-id="f207e-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f207e-125">Application</span></span>||
| <span data-ttu-id="f207e-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="f207e-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f207e-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="f207e-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="f207e-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f207e-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f207e-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="f207e-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="f207e-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="f207e-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="f207e-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="f207e-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f207e-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f207e-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f207e-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="f207e-135">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f207e-135">Request headers</span></span>

|<span data-ttu-id="f207e-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f207e-136">Header</span></span>|<span data-ttu-id="f207e-137">Значение</span><span class="sxs-lookup"><span data-stu-id="f207e-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f207e-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f207e-138">Authorization</span></span>|<span data-ttu-id="f207e-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f207e-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f207e-140">Accept</span><span class="sxs-lookup"><span data-stu-id="f207e-140">Accept</span></span>|<span data-ttu-id="f207e-141">application/json</span><span class="sxs-lookup"><span data-stu-id="f207e-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f207e-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f207e-142">Request body</span></span>

<span data-ttu-id="f207e-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f207e-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f207e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f207e-144">Response</span></span>

<span data-ttu-id="f207e-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f207e-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f207e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="f207e-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="f207e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="f207e-147">Request</span></span>

<span data-ttu-id="f207e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f207e-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="f207e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f207e-149">Response</span></span>

<span data-ttu-id="f207e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f207e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```












