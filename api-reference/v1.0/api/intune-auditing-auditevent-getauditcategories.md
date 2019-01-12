---
title: Функция getAuditCategories
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513df3b403bcde9839ff2a1e9a7e8568c5720d67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959302"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="06bb6-103">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="06bb6-103">getAuditCategories function</span></span>

> <span data-ttu-id="06bb6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06bb6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06bb6-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="06bb6-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06bb6-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="06bb6-106">Prerequisites</span></span>
<span data-ttu-id="06bb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06bb6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06bb6-109">Permission type</span></span>|<span data-ttu-id="06bb6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06bb6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06bb6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06bb6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06bb6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="06bb6-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="06bb6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06bb6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06bb6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06bb6-114">Not supported.</span></span>|
|<span data-ttu-id="06bb6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06bb6-115">Application</span></span>|<span data-ttu-id="06bb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06bb6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06bb6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06bb6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="06bb6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06bb6-118">Request headers</span></span>
|<span data-ttu-id="06bb6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06bb6-119">Header</span></span>|<span data-ttu-id="06bb6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="06bb6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06bb6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06bb6-121">Authorization</span></span>|<span data-ttu-id="06bb6-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="06bb6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06bb6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="06bb6-123">Accept</span></span>|<span data-ttu-id="06bb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06bb6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06bb6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06bb6-125">Request body</span></span>
<span data-ttu-id="06bb6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06bb6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06bb6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="06bb6-127">Response</span></span>
<span data-ttu-id="06bb6-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06bb6-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06bb6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="06bb6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="06bb6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="06bb6-130">Request</span></span>
<span data-ttu-id="06bb6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06bb6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="06bb6-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="06bb6-132">Response</span></span>
<span data-ttu-id="06bb6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="06bb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



