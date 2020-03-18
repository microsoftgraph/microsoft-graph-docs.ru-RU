---
title: Функция Жетманажедаппблоккедусерс
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a6fbd78e1d461c9112a4ccea99b0be6adae4ffa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803388"
---
# <a name="getmanagedappblockedusers-function"></a><span data-ttu-id="2ff45-103">Функция Жетманажедаппблоккедусерс</span><span class="sxs-lookup"><span data-stu-id="2ff45-103">getManagedAppBlockedUsers function</span></span>

> <span data-ttu-id="2ff45-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ff45-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ff45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ff45-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2ff45-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ff45-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2ff45-107">Prerequisites</span></span>
<span data-ttu-id="2ff45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ff45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ff45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff45-110">Permission type</span></span>|<span data-ttu-id="2ff45-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ff45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ff45-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ff45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ff45-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ff45-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2ff45-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ff45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ff45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff45-115">Not supported.</span></span>|
|<span data-ttu-id="2ff45-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2ff45-116">Application</span></span>|<span data-ttu-id="2ff45-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ff45-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ff45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ff45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/getManagedAppBlockedUsers
```

## <a name="request-headers"></a><span data-ttu-id="2ff45-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ff45-119">Request headers</span></span>
|<span data-ttu-id="2ff45-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ff45-120">Header</span></span>|<span data-ttu-id="2ff45-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2ff45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ff45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ff45-122">Authorization</span></span>|<span data-ttu-id="2ff45-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ff45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ff45-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2ff45-124">Accept</span></span>|<span data-ttu-id="2ff45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ff45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ff45-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ff45-126">Request body</span></span>
<span data-ttu-id="2ff45-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ff45-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ff45-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ff45-128">Response</span></span>
<span data-ttu-id="2ff45-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ff45-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ff45-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2ff45-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ff45-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ff45-131">Request</span></span>
<span data-ttu-id="2ff45-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ff45-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/getManagedAppBlockedUsers
```

### <a name="response"></a><span data-ttu-id="2ff45-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ff45-133">Response</span></span>
<span data-ttu-id="2ff45-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ff45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




