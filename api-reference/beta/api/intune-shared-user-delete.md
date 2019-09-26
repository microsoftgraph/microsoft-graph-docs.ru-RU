---
title: Удаление пользователя
description: Удаляет объект user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0822d3e0e3e720ae1f80510dca1d904f64443978
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194378"
---
# <a name="delete-user"></a><span data-ttu-id="2bc94-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="2bc94-103">Delete user</span></span>

> <span data-ttu-id="2bc94-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2bc94-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2bc94-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bc94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bc94-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bc94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bc94-107">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="2bc94-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2bc94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2bc94-108">Prerequisites</span></span>
<span data-ttu-id="2bc94-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="2bc94-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2bc94-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bc94-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="2bc94-111">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="2bc94-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="2bc94-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bc94-112">Permission type</span></span>|<span data-ttu-id="2bc94-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bc94-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bc94-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bc94-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2bc94-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2bc94-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2bc94-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2bc94-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="2bc94-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="2bc94-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2bc94-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="2bc94-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2bc94-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="2bc94-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="2bc94-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2bc94-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2bc94-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bc94-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bc94-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bc94-124">Not supported.</span></span>|
|<span data-ttu-id="2bc94-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bc94-125">Application</span></span>||
| <span data-ttu-id="2bc94-126">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2bc94-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2bc94-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2bc94-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="2bc94-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="2bc94-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2bc94-130">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="2bc94-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2bc94-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="2bc94-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="2bc94-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2bc94-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc94-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bc94-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bc94-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="2bc94-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bc94-135">Request headers</span></span>

|<span data-ttu-id="2bc94-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bc94-136">Header</span></span>|<span data-ttu-id="2bc94-137">Значение</span><span class="sxs-lookup"><span data-stu-id="2bc94-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bc94-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2bc94-138">Authorization</span></span>|<span data-ttu-id="2bc94-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bc94-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bc94-140">Accept</span><span class="sxs-lookup"><span data-stu-id="2bc94-140">Accept</span></span>|<span data-ttu-id="2bc94-141">application/json</span><span class="sxs-lookup"><span data-stu-id="2bc94-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bc94-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bc94-142">Request body</span></span>

<span data-ttu-id="2bc94-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bc94-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc94-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bc94-144">Response</span></span>

<span data-ttu-id="2bc94-145">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2bc94-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2bc94-146">Пример</span><span class="sxs-lookup"><span data-stu-id="2bc94-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bc94-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bc94-147">Request</span></span>

<span data-ttu-id="2bc94-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bc94-148">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="2bc94-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bc94-149">Response</span></span>

<span data-ttu-id="2bc94-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bc94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```







