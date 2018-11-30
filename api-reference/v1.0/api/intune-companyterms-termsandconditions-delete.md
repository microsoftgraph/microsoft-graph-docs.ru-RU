---
title: Delete termsAndConditions
description: Удаляет объект termsAndConditions.
ms.openlocfilehash: 9f267d2b4ee635d80ad293562b0d122c00df03d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024934"
---
# <a name="delete-termsandconditions"></a><span data-ttu-id="dc937-103">Delete termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="dc937-103">Delete termsAndConditions</span></span>

> <span data-ttu-id="dc937-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc937-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc937-105">Удаляет объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="dc937-105">Deletes a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc937-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dc937-106">Prerequisites</span></span>
<span data-ttu-id="dc937-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc937-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc937-109">Permission type</span></span>|<span data-ttu-id="dc937-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc937-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc937-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc937-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc937-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc937-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dc937-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc937-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc937-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc937-114">Not supported.</span></span>|
|<span data-ttu-id="dc937-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc937-115">Application</span></span>|<span data-ttu-id="dc937-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc937-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc937-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc937-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="dc937-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc937-118">Request headers</span></span>
|<span data-ttu-id="dc937-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc937-119">Header</span></span>|<span data-ttu-id="dc937-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dc937-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc937-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc937-121">Authorization</span></span>|<span data-ttu-id="dc937-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="dc937-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc937-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc937-123">Accept</span></span>|<span data-ttu-id="dc937-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc937-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc937-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc937-125">Request body</span></span>
<span data-ttu-id="dc937-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc937-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc937-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc937-127">Response</span></span>
<span data-ttu-id="dc937-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc937-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc937-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dc937-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc937-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc937-130">Request</span></span>
<span data-ttu-id="dc937-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc937-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="dc937-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc937-132">Response</span></span>
<span data-ttu-id="dc937-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="dc937-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



