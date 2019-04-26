---
title: Функция getUserIdsWithFlaggedAppRegistration
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fb55917b9172fa5836e44a864c1ba41e9e06371
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570850"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="bf939-103">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="bf939-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="bf939-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf939-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf939-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bf939-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf939-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf939-106">Prerequisites</span></span>
<span data-ttu-id="bf939-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf939-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf939-109">Permission type</span></span>|<span data-ttu-id="bf939-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf939-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf939-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf939-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bf939-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf939-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bf939-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf939-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf939-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf939-114">Not supported.</span></span>|
|<span data-ttu-id="bf939-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf939-115">Application</span></span>|<span data-ttu-id="bf939-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf939-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf939-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf939-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="bf939-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf939-118">Request headers</span></span>
|<span data-ttu-id="bf939-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf939-119">Header</span></span>|<span data-ttu-id="bf939-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bf939-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf939-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf939-121">Authorization</span></span>|<span data-ttu-id="bf939-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf939-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf939-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bf939-123">Accept</span></span>|<span data-ttu-id="bf939-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bf939-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf939-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf939-125">Request body</span></span>
<span data-ttu-id="bf939-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf939-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf939-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf939-127">Response</span></span>
<span data-ttu-id="bf939-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bf939-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf939-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bf939-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf939-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf939-130">Request</span></span>
<span data-ttu-id="bf939-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf939-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="bf939-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf939-132">Response</span></span>
<span data-ttu-id="bf939-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```



