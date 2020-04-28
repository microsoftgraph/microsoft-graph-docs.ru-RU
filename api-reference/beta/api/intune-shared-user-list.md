---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a06eff8418c16de11578a9a2da09dd7a0b5a873
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447471"
---
# <a name="list-users"></a><span data-ttu-id="892f6-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="892f6-103">List users</span></span>

<span data-ttu-id="892f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="892f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="892f6-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="892f6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="892f6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="892f6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="892f6-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="892f6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="892f6-108">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="892f6-108">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="892f6-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="892f6-109">Prerequisites</span></span>

<span data-ttu-id="892f6-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="892f6-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="892f6-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892f6-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="892f6-112">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="892f6-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="892f6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="892f6-113">Permission type</span></span>|<span data-ttu-id="892f6-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="892f6-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="892f6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="892f6-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="892f6-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="892f6-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="892f6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="892f6-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="892f6-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="892f6-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="892f6-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="892f6-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="892f6-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="892f6-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="892f6-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="892f6-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="892f6-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="892f6-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="892f6-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="892f6-125">Not supported.</span></span>|
|<span data-ttu-id="892f6-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="892f6-126">Application</span></span>||
| <span data-ttu-id="892f6-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="892f6-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="892f6-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="892f6-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="892f6-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="892f6-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="892f6-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="892f6-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="892f6-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="892f6-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="892f6-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="892f6-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="892f6-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="892f6-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="892f6-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="892f6-136">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="892f6-136">Request headers</span></span>

|<span data-ttu-id="892f6-137">Заголовок</span><span class="sxs-lookup"><span data-stu-id="892f6-137">Header</span></span>|<span data-ttu-id="892f6-138">Значение</span><span class="sxs-lookup"><span data-stu-id="892f6-138">Value</span></span>|
|:---|:---|
|<span data-ttu-id="892f6-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="892f6-139">Authorization</span></span>|<span data-ttu-id="892f6-140">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="892f6-140">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="892f6-141">Accept</span><span class="sxs-lookup"><span data-stu-id="892f6-141">Accept</span></span>|<span data-ttu-id="892f6-142">application/json</span><span class="sxs-lookup"><span data-stu-id="892f6-142">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="892f6-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="892f6-143">Request body</span></span>

<span data-ttu-id="892f6-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="892f6-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="892f6-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="892f6-145">Response</span></span>

<span data-ttu-id="892f6-146">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="892f6-146">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892f6-147">Пример</span><span class="sxs-lookup"><span data-stu-id="892f6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="892f6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="892f6-148">Request</span></span>

<span data-ttu-id="892f6-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="892f6-149">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="892f6-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="892f6-150">Response</span></span>

<span data-ttu-id="892f6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="892f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```









