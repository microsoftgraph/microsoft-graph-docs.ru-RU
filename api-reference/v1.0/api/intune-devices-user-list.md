---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e160dcf921b76eeedc51999c65e03ab590fd73b5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753438"
---
# <a name="list-users"></a><span data-ttu-id="90c4f-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="90c4f-103">List users</span></span>

<span data-ttu-id="90c4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90c4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90c4f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90c4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c4f-106">Список свойств и связей объектов [user](../resources/intune-devices-user.md).</span><span class="sxs-lookup"><span data-stu-id="90c4f-106">List properties and relationships of the [user](../resources/intune-devices-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90c4f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="90c4f-107">Prerequisites</span></span>
<span data-ttu-id="90c4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c4f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c4f-110">Permission type</span></span>|<span data-ttu-id="90c4f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c4f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90c4f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90c4f-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c4f-113">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="90c4f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90c4f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c4f-115">Not supported.</span></span>|
|<span data-ttu-id="90c4f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="90c4f-116">Application</span></span>|<span data-ttu-id="90c4f-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c4f-117">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90c4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="90c4f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90c4f-119">Request headers</span></span>
|<span data-ttu-id="90c4f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90c4f-120">Header</span></span>|<span data-ttu-id="90c4f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="90c4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90c4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90c4f-122">Authorization</span></span>|<span data-ttu-id="90c4f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90c4f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="90c4f-124">Accept</span></span>|<span data-ttu-id="90c4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90c4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c4f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90c4f-126">Request body</span></span>
<span data-ttu-id="90c4f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90c4f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90c4f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c4f-128">Response</span></span>
<span data-ttu-id="90c4f-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-devices-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90c4f-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-devices-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90c4f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90c4f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="90c4f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c4f-131">Request</span></span>
<span data-ttu-id="90c4f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c4f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="90c4f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c4f-133">Response</span></span>
<span data-ttu-id="90c4f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90c4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




