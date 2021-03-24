---
title: функция getManagedAppBlockedUsers
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d6bcc526395c473197a762a675f35160f733b7b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148955"
---
# <a name="getmanagedappblockedusers-function"></a><span data-ttu-id="2cc89-103">функция getManagedAppBlockedUsers</span><span class="sxs-lookup"><span data-stu-id="2cc89-103">getManagedAppBlockedUsers function</span></span>

<span data-ttu-id="2cc89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cc89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cc89-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc89-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc89-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2cc89-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cc89-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2cc89-108">Prerequisites</span></span>
<span data-ttu-id="2cc89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc89-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cc89-111">Permission type</span></span>|<span data-ttu-id="2cc89-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cc89-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc89-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cc89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc89-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc89-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2cc89-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cc89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc89-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc89-116">Not supported.</span></span>|
|<span data-ttu-id="2cc89-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2cc89-117">Application</span></span>|<span data-ttu-id="2cc89-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc89-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc89-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cc89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/getManagedAppBlockedUsers
```

## <a name="request-headers"></a><span data-ttu-id="2cc89-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2cc89-120">Request headers</span></span>
|<span data-ttu-id="2cc89-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cc89-121">Header</span></span>|<span data-ttu-id="2cc89-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cc89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cc89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cc89-123">Authorization</span></span>|<span data-ttu-id="2cc89-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cc89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cc89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cc89-125">Accept</span></span>|<span data-ttu-id="2cc89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cc89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cc89-127">Request body</span></span>
<span data-ttu-id="2cc89-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cc89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cc89-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc89-129">Response</span></span>
<span data-ttu-id="2cc89-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2cc89-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc89-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2cc89-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cc89-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cc89-132">Request</span></span>
<span data-ttu-id="2cc89-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cc89-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/getManagedAppBlockedUsers
```

### <a name="response"></a><span data-ttu-id="2cc89-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc89-134">Response</span></span>
<span data-ttu-id="2cc89-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cc89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 66

{
  "value": [
    "Get Managed App Blocked Users value"
  ]
}
```




