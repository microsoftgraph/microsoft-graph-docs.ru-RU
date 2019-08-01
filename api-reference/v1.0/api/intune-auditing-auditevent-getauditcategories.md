---
title: Функция getAuditCategories
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a1363f2aef76d5ce2e6c4f9e3e1e20c3bd7d0bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001910"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="6db97-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="6db97-103">getAuditCategories function</span></span>

> <span data-ttu-id="6db97-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6db97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6db97-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6db97-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6db97-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6db97-106">Prerequisites</span></span>
<span data-ttu-id="6db97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6db97-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6db97-109">Permission type</span></span>|<span data-ttu-id="6db97-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6db97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6db97-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6db97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6db97-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6db97-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6db97-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6db97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6db97-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6db97-114">Not supported.</span></span>|
|<span data-ttu-id="6db97-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6db97-115">Application</span></span>|<span data-ttu-id="6db97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6db97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6db97-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6db97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="6db97-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6db97-118">Request headers</span></span>
|<span data-ttu-id="6db97-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6db97-119">Header</span></span>|<span data-ttu-id="6db97-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6db97-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6db97-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6db97-121">Authorization</span></span>|<span data-ttu-id="6db97-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6db97-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6db97-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6db97-123">Accept</span></span>|<span data-ttu-id="6db97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6db97-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6db97-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6db97-125">Request body</span></span>
<span data-ttu-id="6db97-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6db97-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6db97-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6db97-127">Response</span></span>
<span data-ttu-id="6db97-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6db97-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db97-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6db97-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6db97-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6db97-130">Request</span></span>
<span data-ttu-id="6db97-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6db97-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="6db97-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6db97-132">Response</span></span>
<span data-ttu-id="6db97-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6db97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



