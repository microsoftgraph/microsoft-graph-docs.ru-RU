---
title: Функция Жетлиценсесфорапп
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 679f44364dc5d534fa58e874502b5b51609a995f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975954"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="ee75a-103">Функция Жетлиценсесфорапп</span><span class="sxs-lookup"><span data-stu-id="ee75a-103">getLicensesForApp function</span></span>

> <span data-ttu-id="ee75a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee75a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee75a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee75a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee75a-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ee75a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee75a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ee75a-107">Prerequisites</span></span>
<span data-ttu-id="ee75a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee75a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee75a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee75a-110">Permission type</span></span>|<span data-ttu-id="ee75a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee75a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee75a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee75a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee75a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee75a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ee75a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee75a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee75a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee75a-115">Not supported.</span></span>|
|<span data-ttu-id="ee75a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee75a-116">Application</span></span>|<span data-ttu-id="ee75a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee75a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee75a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee75a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="ee75a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee75a-119">Request headers</span></span>
|<span data-ttu-id="ee75a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee75a-120">Header</span></span>|<span data-ttu-id="ee75a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee75a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee75a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee75a-122">Authorization</span></span>|<span data-ttu-id="ee75a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee75a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee75a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee75a-124">Accept</span></span>|<span data-ttu-id="ee75a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee75a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee75a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee75a-126">Request body</span></span>
<span data-ttu-id="ee75a-127">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ee75a-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ee75a-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="ee75a-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ee75a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee75a-129">Property</span></span>|<span data-ttu-id="ee75a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee75a-130">Type</span></span>|<span data-ttu-id="ee75a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee75a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee75a-132">bundleId</span><span class="sxs-lookup"><span data-stu-id="ee75a-132">bundleId</span></span>|<span data-ttu-id="ee75a-133">String</span><span class="sxs-lookup"><span data-stu-id="ee75a-133">String</span></span>|<span data-ttu-id="ee75a-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ee75a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ee75a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee75a-135">Response</span></span>
<span data-ttu-id="ee75a-136">В случае успеха эта функция возвращает код `200 OK` отклика и коллекцию [впптокенлиценсесуммари](../resources/intune-onboarding-vpptokenlicensesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee75a-136">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee75a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ee75a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee75a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee75a-138">Request</span></span>
<span data-ttu-id="ee75a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee75a-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ee75a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee75a-140">Response</span></span>
<span data-ttu-id="ee75a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee75a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




