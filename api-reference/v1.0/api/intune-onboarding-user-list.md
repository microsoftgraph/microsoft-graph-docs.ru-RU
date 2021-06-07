---
title: Перечисление пользователей
description: Список свойств и связей объектов user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dcb25811cd9ba56959ec8c203f00d95c7a87f15
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752064"
---
# <a name="list-users"></a><span data-ttu-id="50212-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="50212-103">List users</span></span>

<span data-ttu-id="50212-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50212-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50212-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50212-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50212-106">Список свойств и связей объектов [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="50212-106">List properties and relationships of the [user](../resources/intune-onboarding-user.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50212-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50212-107">Prerequisites</span></span>
<span data-ttu-id="50212-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50212-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50212-110">Permission type</span></span>|<span data-ttu-id="50212-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50212-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50212-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50212-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50212-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50212-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="50212-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50212-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50212-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50212-115">Not supported.</span></span>|
|<span data-ttu-id="50212-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="50212-116">Application</span></span>|<span data-ttu-id="50212-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50212-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50212-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50212-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="50212-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50212-119">Request headers</span></span>
|<span data-ttu-id="50212-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50212-120">Header</span></span>|<span data-ttu-id="50212-121">Значение</span><span class="sxs-lookup"><span data-stu-id="50212-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50212-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50212-122">Authorization</span></span>|<span data-ttu-id="50212-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50212-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50212-124">Accept</span><span class="sxs-lookup"><span data-stu-id="50212-124">Accept</span></span>|<span data-ttu-id="50212-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50212-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50212-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50212-126">Request body</span></span>
<span data-ttu-id="50212-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50212-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50212-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="50212-128">Response</span></span>
<span data-ttu-id="50212-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/intune-onboarding-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="50212-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune-onboarding-user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50212-130">Пример</span><span class="sxs-lookup"><span data-stu-id="50212-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="50212-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="50212-131">Request</span></span>
<span data-ttu-id="50212-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50212-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="50212-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="50212-133">Response</span></span>
<span data-ttu-id="50212-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50212-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
      "deviceEnrollmentLimit": 5
    }
  ]
}
```




