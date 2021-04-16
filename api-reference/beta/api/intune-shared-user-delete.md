---
title: Удаление пользователя
description: Удаляет объект user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdce3e09a37010a746314a0d7dfc7112a69ab68e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864566"
---
# <a name="delete-user"></a><span data-ttu-id="d5a57-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="d5a57-103">Delete user</span></span>

<span data-ttu-id="d5a57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5a57-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="d5a57-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5a57-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a57-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5a57-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5a57-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5a57-108">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d5a57-108">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5a57-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5a57-109">Prerequisites</span></span>
<span data-ttu-id="d5a57-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="d5a57-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d5a57-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a57-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="d5a57-112">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="d5a57-112">The specific permission required depends on context.</span></span>

|<span data-ttu-id="d5a57-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a57-113">Permission type</span></span>|<span data-ttu-id="d5a57-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5a57-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5a57-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a57-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5a57-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d5a57-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d5a57-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a57-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d5a57-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d5a57-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-119">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a57-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d5a57-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d5a57-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a57-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d5a57-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d5a57-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d5a57-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a57-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5a57-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a57-125">Not supported.</span></span>|
|<span data-ttu-id="d5a57-126">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d5a57-126">Application</span></span>||
| <span data-ttu-id="d5a57-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d5a57-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d5a57-128">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-128">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a57-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="d5a57-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="d5a57-130">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-130">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a57-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d5a57-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d5a57-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-132">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="d5a57-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="d5a57-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="d5a57-134">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a57-134">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5a57-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a57-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d5a57-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5a57-136">Request headers</span></span>

|<span data-ttu-id="d5a57-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5a57-137">Header</span></span>|<span data-ttu-id="d5a57-138">Значение</span><span class="sxs-lookup"><span data-stu-id="d5a57-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5a57-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5a57-139">Authorization</span></span>|<span data-ttu-id="d5a57-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a57-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5a57-141">Accept</span><span class="sxs-lookup"><span data-stu-id="d5a57-141">Accept</span></span>|<span data-ttu-id="d5a57-142">application/json</span><span class="sxs-lookup"><span data-stu-id="d5a57-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5a57-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5a57-143">Request body</span></span>

<span data-ttu-id="d5a57-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5a57-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5a57-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a57-145">Response</span></span>

<span data-ttu-id="d5a57-146">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5a57-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5a57-147">Пример</span><span class="sxs-lookup"><span data-stu-id="d5a57-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5a57-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a57-148">Request</span></span>

<span data-ttu-id="d5a57-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5a57-149">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="d5a57-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a57-150">Response</span></span>

<span data-ttu-id="d5a57-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5a57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```










