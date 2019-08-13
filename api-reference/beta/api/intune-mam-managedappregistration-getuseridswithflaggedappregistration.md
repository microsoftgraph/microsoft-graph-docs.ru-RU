---
title: Функция getUserIdsWithFlaggedAppRegistration
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a207e809e5ba3bccc6752630fd9a2c4e4cce6a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354046"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="16a0d-103">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="16a0d-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="16a0d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16a0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16a0d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16a0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16a0d-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="16a0d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16a0d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16a0d-107">Prerequisites</span></span>
<span data-ttu-id="16a0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16a0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16a0d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16a0d-110">Permission type</span></span>|<span data-ttu-id="16a0d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16a0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16a0d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16a0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16a0d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a0d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="16a0d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16a0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16a0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16a0d-115">Not supported.</span></span>|
|<span data-ttu-id="16a0d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16a0d-116">Application</span></span>|<span data-ttu-id="16a0d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="16a0d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16a0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16a0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="16a0d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16a0d-119">Request headers</span></span>
|<span data-ttu-id="16a0d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16a0d-120">Header</span></span>|<span data-ttu-id="16a0d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16a0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16a0d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16a0d-122">Authorization</span></span>|<span data-ttu-id="16a0d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16a0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16a0d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16a0d-124">Accept</span></span>|<span data-ttu-id="16a0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16a0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16a0d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16a0d-126">Request body</span></span>
<span data-ttu-id="16a0d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16a0d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16a0d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="16a0d-128">Response</span></span>
<span data-ttu-id="16a0d-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16a0d-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16a0d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="16a0d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="16a0d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="16a0d-131">Request</span></span>
<span data-ttu-id="16a0d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16a0d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="16a0d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="16a0d-133">Response</span></span>
<span data-ttu-id="16a0d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16a0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






