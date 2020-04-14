---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c07935d242e9cf25ddb996c87e530122eea1b1fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447530"
---
# <a name="get-user"></a><span data-ttu-id="72c61-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="72c61-103">Get user</span></span>

<span data-ttu-id="72c61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72c61-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72c61-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72c61-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c61-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72c61-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72c61-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72c61-108">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="72c61-108">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72c61-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72c61-109">Prerequisites</span></span>

<span data-ttu-id="72c61-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="72c61-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="72c61-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c61-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="72c61-112">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="72c61-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="72c61-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72c61-113">Permission type</span></span>|<span data-ttu-id="72c61-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72c61-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72c61-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72c61-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="72c61-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="72c61-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="72c61-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="72c61-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="72c61-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="72c61-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="72c61-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="72c61-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="72c61-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="72c61-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="72c61-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="72c61-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="72c61-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72c61-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72c61-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c61-125">Not supported.</span></span>|
|<span data-ttu-id="72c61-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72c61-126">Application</span></span>||
| <span data-ttu-id="72c61-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="72c61-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="72c61-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="72c61-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="72c61-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="72c61-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="72c61-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="72c61-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="72c61-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="72c61-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="72c61-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="72c61-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="72c61-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72c61-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72c61-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72c61-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72c61-136">Optional query parameters</span></span>

<span data-ttu-id="72c61-137">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72c61-137">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72c61-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72c61-138">Request headers</span></span>

|<span data-ttu-id="72c61-139">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72c61-139">Header</span></span>|<span data-ttu-id="72c61-140">Значение</span><span class="sxs-lookup"><span data-stu-id="72c61-140">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72c61-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="72c61-141">Authorization</span></span>|<span data-ttu-id="72c61-142">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72c61-142">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72c61-143">Accept</span><span class="sxs-lookup"><span data-stu-id="72c61-143">Accept</span></span>|<span data-ttu-id="72c61-144">application/json</span><span class="sxs-lookup"><span data-stu-id="72c61-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72c61-145">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72c61-145">Request body</span></span>

<span data-ttu-id="72c61-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72c61-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c61-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c61-147">Response</span></span>

<span data-ttu-id="72c61-148">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72c61-148">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72c61-149">Пример</span><span class="sxs-lookup"><span data-stu-id="72c61-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="72c61-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="72c61-150">Request</span></span>

<span data-ttu-id="72c61-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72c61-151">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="72c61-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c61-152">Response</span></span>

<span data-ttu-id="72c61-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72c61-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```









