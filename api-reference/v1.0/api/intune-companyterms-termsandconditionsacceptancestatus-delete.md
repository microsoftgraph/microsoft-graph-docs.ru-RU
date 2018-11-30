---
title: Delete termsAndConditionsAcceptanceStatus
description: Удаляет объект termsAndConditionsAcceptanceStatus.
ms.openlocfilehash: a034cf9574cd8e9894924aa555c999a31408e0b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026175"
---
# <a name="delete-termsandconditionsacceptancestatus"></a><span data-ttu-id="3a864-103">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="3a864-103">Delete termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="3a864-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3a864-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a864-105">Удаляет объект [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="3a864-105">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3a864-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3a864-106">Prerequisites</span></span>
<span data-ttu-id="3a864-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a864-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a864-109">Permission type</span></span>|<span data-ttu-id="3a864-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a864-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a864-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a864-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a864-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a864-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a864-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a864-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a864-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a864-114">Not supported.</span></span>|
|<span data-ttu-id="3a864-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a864-115">Application</span></span>|<span data-ttu-id="3a864-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a864-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a864-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a864-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="3a864-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a864-118">Request headers</span></span>
|<span data-ttu-id="3a864-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a864-119">Header</span></span>|<span data-ttu-id="3a864-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3a864-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a864-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a864-121">Authorization</span></span>|<span data-ttu-id="3a864-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a864-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a864-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3a864-123">Accept</span></span>|<span data-ttu-id="3a864-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3a864-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a864-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a864-125">Request body</span></span>
<span data-ttu-id="3a864-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a864-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a864-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a864-127">Response</span></span>
<span data-ttu-id="3a864-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3a864-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3a864-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3a864-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3a864-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a864-130">Request</span></span>
<span data-ttu-id="3a864-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a864-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="3a864-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a864-132">Response</span></span>
<span data-ttu-id="3a864-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3a864-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



