---
title: Удаление пользователя
description: Удаляет объект user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42bf2372deed17528b610ca719213ff2e282b9ac
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800594"
---
# <a name="delete-user"></a><span data-ttu-id="060c4-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="060c4-103">Delete user</span></span>

> <span data-ttu-id="060c4-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="060c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="060c4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="060c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="060c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060c4-107">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="060c4-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="060c4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="060c4-108">Prerequisites</span></span>
<span data-ttu-id="060c4-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="060c4-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="060c4-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="060c4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="060c4-111">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="060c4-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="060c4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="060c4-112">Permission type</span></span>|<span data-ttu-id="060c4-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="060c4-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="060c4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="060c4-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="060c4-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="060c4-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="060c4-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="060c4-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="060c4-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="060c4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="060c4-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="060c4-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="060c4-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="060c4-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="060c4-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="060c4-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="060c4-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="060c4-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="060c4-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="060c4-124">Not supported.</span></span>|
|<span data-ttu-id="060c4-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="060c4-125">Application</span></span>||
| <span data-ttu-id="060c4-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="060c4-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="060c4-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="060c4-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="060c4-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="060c4-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="060c4-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="060c4-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="060c4-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="060c4-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="060c4-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="060c4-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="060c4-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="060c4-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="060c4-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="060c4-135">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="060c4-135">Request headers</span></span>

|<span data-ttu-id="060c4-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="060c4-136">Header</span></span>|<span data-ttu-id="060c4-137">Значение</span><span class="sxs-lookup"><span data-stu-id="060c4-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="060c4-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="060c4-138">Authorization</span></span>|<span data-ttu-id="060c4-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="060c4-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="060c4-140">Accept</span><span class="sxs-lookup"><span data-stu-id="060c4-140">Accept</span></span>|<span data-ttu-id="060c4-141">application/json</span><span class="sxs-lookup"><span data-stu-id="060c4-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="060c4-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="060c4-142">Request body</span></span>

<span data-ttu-id="060c4-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="060c4-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="060c4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="060c4-144">Response</span></span>

<span data-ttu-id="060c4-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="060c4-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="060c4-146">Пример</span><span class="sxs-lookup"><span data-stu-id="060c4-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="060c4-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="060c4-147">Request</span></span>

<span data-ttu-id="060c4-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="060c4-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="060c4-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="060c4-149">Response</span></span>

<span data-ttu-id="060c4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="060c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










