---
title: Функция getUserIdsWithFlaggedAppRegistration
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8af9b640a07be379cc4fba084ad92344f5b42753
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465608"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="d2975-103">Функция getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d2975-103">getUserIdsWithFlaggedAppRegistration function</span></span>

<span data-ttu-id="d2975-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2975-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2975-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2975-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2975-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2975-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2975-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d2975-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2975-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d2975-108">Prerequisites</span></span>
<span data-ttu-id="d2975-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2975-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2975-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2975-111">Permission type</span></span>|<span data-ttu-id="d2975-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2975-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2975-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2975-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2975-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2975-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2975-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2975-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2975-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2975-116">Not supported.</span></span>|
|<span data-ttu-id="d2975-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2975-117">Application</span></span>|<span data-ttu-id="d2975-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2975-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2975-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2975-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="d2975-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2975-120">Request headers</span></span>
|<span data-ttu-id="d2975-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2975-121">Header</span></span>|<span data-ttu-id="d2975-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d2975-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2975-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2975-123">Authorization</span></span>|<span data-ttu-id="d2975-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2975-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2975-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2975-125">Accept</span></span>|<span data-ttu-id="d2975-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2975-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2975-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2975-127">Request body</span></span>
<span data-ttu-id="d2975-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2975-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2975-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2975-129">Response</span></span>
<span data-ttu-id="d2975-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2975-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2975-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d2975-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2975-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2975-132">Request</span></span>
<span data-ttu-id="d2975-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2975-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="d2975-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2975-134">Response</span></span>
<span data-ttu-id="d2975-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2975-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



