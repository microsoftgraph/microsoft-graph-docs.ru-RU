---
title: Функция getAuditCategories
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbdf940d56e8bdb7a02b5af8749a525305bd44a8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934392"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="e1ea1-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="e1ea1-103">getAuditCategories function</span></span>

> <span data-ttu-id="e1ea1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1ea1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1ea1-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1ea1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e1ea1-107">Prerequisites</span></span>
<span data-ttu-id="e1ea1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ea1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1ea1-110">Permission type</span></span>|<span data-ttu-id="e1ea1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1ea1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1ea1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1ea1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1ea1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1ea1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e1ea1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1ea1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1ea1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-115">Not supported.</span></span>|
|<span data-ttu-id="e1ea1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1ea1-116">Application</span></span>|<span data-ttu-id="e1ea1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1ea1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1ea1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="e1ea1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1ea1-119">Request headers</span></span>
|<span data-ttu-id="e1ea1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1ea1-120">Header</span></span>|<span data-ttu-id="e1ea1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e1ea1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1ea1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1ea1-122">Authorization</span></span>|<span data-ttu-id="e1ea1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1ea1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e1ea1-124">Accept</span></span>|<span data-ttu-id="e1ea1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ea1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ea1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1ea1-126">Request body</span></span>
<span data-ttu-id="e1ea1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1ea1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1ea1-128">Response</span></span>
<span data-ttu-id="e1ea1-129">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-129">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ea1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e1ea1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1ea1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1ea1-131">Request</span></span>
<span data-ttu-id="e1ea1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="e1ea1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1ea1-133">Response</span></span>
<span data-ttu-id="e1ea1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1ea1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```




