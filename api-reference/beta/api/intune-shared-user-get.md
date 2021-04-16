---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66cb634de90c65bb6ca6b020c97373c57a446b21
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865665"
---
# <a name="get-user"></a><span data-ttu-id="4af9a-103">Получение пользователя</span><span class="sxs-lookup"><span data-stu-id="4af9a-103">Get user</span></span>

<span data-ttu-id="4af9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4af9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4af9a-105">**Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="4af9a-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4af9a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4af9a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4af9a-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4af9a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4af9a-108">Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="4af9a-108">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4af9a-109">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4af9a-109">Prerequisites</span></span>

<span data-ttu-id="4af9a-110">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="4af9a-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4af9a-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4af9a-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="4af9a-112">Конкретное разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="4af9a-112">The specific permission depends on the context.</span></span>

|<span data-ttu-id="4af9a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4af9a-113">Permission type</span></span>|<span data-ttu-id="4af9a-114">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4af9a-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4af9a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4af9a-115">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4af9a-116">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="4af9a-116">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4af9a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4af9a-118">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="4af9a-118">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4af9a-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-119">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4af9a-120">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4af9a-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4af9a-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4af9a-122">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="4af9a-122">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4af9a-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="4af9a-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4af9a-124">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4af9a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4af9a-125">Not supported.</span></span>|
|<span data-ttu-id="4af9a-126">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4af9a-126">Application</span></span>||
| <span data-ttu-id="4af9a-127">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="4af9a-127">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4af9a-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-128">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4af9a-129">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="4af9a-129">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="4af9a-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-130">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4af9a-131">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4af9a-131">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4af9a-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-132">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4af9a-133">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="4af9a-133">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4af9a-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4af9a-134">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4af9a-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4af9a-135">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4af9a-136">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4af9a-136">Optional query parameters</span></span>

<span data-ttu-id="4af9a-137">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4af9a-137">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4af9a-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4af9a-138">Request headers</span></span>

|<span data-ttu-id="4af9a-139">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4af9a-139">Header</span></span>|<span data-ttu-id="4af9a-140">Значение</span><span class="sxs-lookup"><span data-stu-id="4af9a-140">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4af9a-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4af9a-141">Authorization</span></span>|<span data-ttu-id="4af9a-142">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4af9a-142">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4af9a-143">Accept</span><span class="sxs-lookup"><span data-stu-id="4af9a-143">Accept</span></span>|<span data-ttu-id="4af9a-144">application/json</span><span class="sxs-lookup"><span data-stu-id="4af9a-144">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4af9a-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4af9a-145">Request body</span></span>

<span data-ttu-id="4af9a-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4af9a-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4af9a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4af9a-147">Response</span></span>

<span data-ttu-id="4af9a-148">В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4af9a-148">If successful, this method returns a `200 OK` response code and [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4af9a-149">Пример</span><span class="sxs-lookup"><span data-stu-id="4af9a-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="4af9a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4af9a-150">Request</span></span>

<span data-ttu-id="4af9a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4af9a-151">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="4af9a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4af9a-152">Response</span></span>

<span data-ttu-id="4af9a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4af9a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










