---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d8602445eab740d18b2edf7036dd4b737d5be5a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537883"
---
# <a name="list-users"></a><span data-ttu-id="323d6-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="323d6-103">List users</span></span>

> <span data-ttu-id="323d6-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="323d6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="323d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="323d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="323d6-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="323d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="323d6-107">Список свойств и связей объектов [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="323d6-107">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="323d6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="323d6-108">Prerequisites</span></span>

<span data-ttu-id="323d6-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="323d6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="323d6-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="323d6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="323d6-111">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="323d6-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="323d6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="323d6-112">Permission type</span></span>|<span data-ttu-id="323d6-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="323d6-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="323d6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="323d6-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="323d6-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="323d6-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="323d6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="323d6-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="323d6-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="323d6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="323d6-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="323d6-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="323d6-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="323d6-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="323d6-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="323d6-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="323d6-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="323d6-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="323d6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="323d6-124">Not supported.</span></span>|
|<span data-ttu-id="323d6-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="323d6-125">Application</span></span>||
| <span data-ttu-id="323d6-126">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="323d6-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="323d6-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="323d6-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="323d6-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="323d6-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="323d6-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="323d6-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="323d6-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="323d6-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="323d6-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="323d6-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="323d6-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="323d6-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="323d6-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="323d6-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="323d6-135">Request headers</span></span>

|<span data-ttu-id="323d6-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="323d6-136">Header</span></span>|<span data-ttu-id="323d6-137">Значение</span><span class="sxs-lookup"><span data-stu-id="323d6-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="323d6-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="323d6-138">Authorization</span></span>|<span data-ttu-id="323d6-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="323d6-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="323d6-140">Accept</span><span class="sxs-lookup"><span data-stu-id="323d6-140">Accept</span></span>|<span data-ttu-id="323d6-141">application/json</span><span class="sxs-lookup"><span data-stu-id="323d6-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="323d6-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="323d6-142">Request body</span></span>

<span data-ttu-id="323d6-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="323d6-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="323d6-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="323d6-144">Response</span></span>

<span data-ttu-id="323d6-145">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="323d6-145">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-shared-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="323d6-146">Пример</span><span class="sxs-lookup"><span data-stu-id="323d6-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="323d6-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="323d6-147">Request</span></span>

<span data-ttu-id="323d6-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="323d6-148">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users
```

### <a name="response"></a><span data-ttu-id="323d6-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="323d6-149">Response</span></span>

<span data-ttu-id="323d6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="323d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









