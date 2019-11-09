---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26ed6faf65bd5a2512840eb3c9cd088ab61e3553
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085579"
---
# <a name="get-user"></a><span data-ttu-id="01b2b-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="01b2b-103">Get user</span></span>

> <span data-ttu-id="01b2b-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01b2b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="01b2b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01b2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01b2b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01b2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01b2b-107">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="01b2b-107">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01b2b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="01b2b-108">Prerequisites</span></span>

<span data-ttu-id="01b2b-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="01b2b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="01b2b-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01b2b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="01b2b-111">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="01b2b-111">The specific permission depends on the context.</span></span>

|<span data-ttu-id="01b2b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01b2b-112">Permission type</span></span>|<span data-ttu-id="01b2b-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01b2b-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01b2b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01b2b-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="01b2b-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="01b2b-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="01b2b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="01b2b-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="01b2b-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="01b2b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="01b2b-119">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="01b2b-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="01b2b-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="01b2b-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="01b2b-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="01b2b-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="01b2b-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01b2b-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01b2b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01b2b-124">Not supported.</span></span>|
|<span data-ttu-id="01b2b-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01b2b-125">Application</span></span>||
| <span data-ttu-id="01b2b-126">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="01b2b-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="01b2b-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-127">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="01b2b-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="01b2b-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="01b2b-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-129">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="01b2b-130">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="01b2b-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="01b2b-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="01b2b-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="01b2b-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="01b2b-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="01b2b-133">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01b2b-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01b2b-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01b2b-135">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01b2b-135">Optional query parameters</span></span>

<span data-ttu-id="01b2b-136">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01b2b-136">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01b2b-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01b2b-137">Request headers</span></span>

|<span data-ttu-id="01b2b-138">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01b2b-138">Header</span></span>|<span data-ttu-id="01b2b-139">Значение</span><span class="sxs-lookup"><span data-stu-id="01b2b-139">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01b2b-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01b2b-140">Authorization</span></span>|<span data-ttu-id="01b2b-141">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01b2b-141">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01b2b-142">Accept</span><span class="sxs-lookup"><span data-stu-id="01b2b-142">Accept</span></span>|<span data-ttu-id="01b2b-143">application/json</span><span class="sxs-lookup"><span data-stu-id="01b2b-143">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01b2b-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01b2b-144">Request body</span></span>

<span data-ttu-id="01b2b-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01b2b-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01b2b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="01b2b-146">Response</span></span>

<span data-ttu-id="01b2b-147">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01b2b-147">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01b2b-148">Пример</span><span class="sxs-lookup"><span data-stu-id="01b2b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="01b2b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="01b2b-149">Request</span></span>

<span data-ttu-id="01b2b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01b2b-150">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="01b2b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="01b2b-151">Response</span></span>

<span data-ttu-id="01b2b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01b2b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












