---
title: функция getLicensesForApp
description: Н/Д
ms.openlocfilehash: d96a2736ee0fe0bcb2303aa12791e6222e8d55d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079660"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="c2727-103">функция getLicensesForApp</span><span class="sxs-lookup"><span data-stu-id="c2727-103">getLicensesForApp function</span></span>

> <span data-ttu-id="c2727-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2727-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2727-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2727-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2727-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2727-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2727-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c2727-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2727-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2727-108">Prerequisites</span></span>
<span data-ttu-id="c2727-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2727-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2727-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2727-111">Permission type</span></span>|<span data-ttu-id="c2727-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2727-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2727-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2727-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2727-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c2727-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2727-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2727-116">Not supported.</span></span>|
|<span data-ttu-id="c2727-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2727-117">Application</span></span>|<span data-ttu-id="c2727-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2727-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2727-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="c2727-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2727-120">Request headers</span></span>
|<span data-ttu-id="c2727-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2727-121">Header</span></span>|<span data-ttu-id="c2727-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2727-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2727-123">Authorization</span></span>|<span data-ttu-id="c2727-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2727-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2727-125">Accept</span></span>|<span data-ttu-id="c2727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2727-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2727-127">Request body</span></span>
<span data-ttu-id="c2727-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="c2727-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c2727-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="c2727-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c2727-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2727-130">Property</span></span>|<span data-ttu-id="c2727-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2727-131">Type</span></span>|<span data-ttu-id="c2727-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2727-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2727-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="c2727-133">bundleId</span></span>|<span data-ttu-id="c2727-134">String</span><span class="sxs-lookup"><span data-stu-id="c2727-134">String</span></span>|<span data-ttu-id="c2727-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c2727-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c2727-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2727-136">Response</span></span>
<span data-ttu-id="c2727-137">Если успешно завершена, эта функция возвращает `200 OK` код ответа и семейства [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2727-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2727-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c2727-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2727-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2727-139">Request</span></span>
<span data-ttu-id="c2727-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2727-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c2727-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2727-141">Response</span></span>
<span data-ttu-id="c2727-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c2727-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": [
    {
      "@odata.type": "microsoft.graph.vppTokenLicenseSummary",
      "vppTokenId": "Vpp Token Id value",
      "appleId": "Apple Id value",
      "organizationName": "Organization Name value",
      "availableLicenseCount": 5,
      "usedLicenseCount": 0
    }
  ]
}
```





