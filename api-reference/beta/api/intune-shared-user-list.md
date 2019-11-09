---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc565f8c51aae2448153d85d3cf6bcc4b130a217
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085537"
---
# <a name="list-users"></a><span data-ttu-id="c0635-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="c0635-103">List users</span></span>

> <span data-ttu-id="c0635-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0635-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0635-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0635-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0635-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0635-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0635-107">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c0635-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0635-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0635-108">Prerequisites</span></span>

<span data-ttu-id="c0635-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="c0635-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c0635-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0635-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c0635-111">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="c0635-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="c0635-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0635-112">Permission type</span></span>|<span data-ttu-id="c0635-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0635-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0635-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0635-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c0635-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c0635-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c0635-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c0635-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c0635-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c0635-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c0635-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c0635-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c0635-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c0635-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c0635-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c0635-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="c0635-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0635-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0635-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0635-124">Not supported.</span></span>|
|<span data-ttu-id="c0635-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0635-125">Application</span></span>||
| <span data-ttu-id="c0635-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="c0635-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c0635-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c0635-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c0635-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c0635-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c0635-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="c0635-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c0635-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c0635-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="c0635-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c0635-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0635-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0635-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0635-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="c0635-135">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0635-135">Request headers</span></span>

|<span data-ttu-id="c0635-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0635-136">Header</span></span>|<span data-ttu-id="c0635-137">Значение</span><span class="sxs-lookup"><span data-stu-id="c0635-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0635-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0635-138">Authorization</span></span>|<span data-ttu-id="c0635-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0635-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0635-140">Accept</span><span class="sxs-lookup"><span data-stu-id="c0635-140">Accept</span></span>|<span data-ttu-id="c0635-141">application/json</span><span class="sxs-lookup"><span data-stu-id="c0635-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0635-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0635-142">Request body</span></span>

<span data-ttu-id="c0635-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0635-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0635-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0635-144">Response</span></span>

<span data-ttu-id="c0635-145">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c0635-145">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0635-146">Пример</span><span class="sxs-lookup"><span data-stu-id="c0635-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0635-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0635-147">Request</span></span>

<span data-ttu-id="c0635-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0635-148">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="c0635-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0635-149">Response</span></span>

<span data-ttu-id="c0635-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0635-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












