---
title: Get termsAndConditions
description: Чтение свойств и связей объекта termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf053e329202784d94122cac79cf79300b2029ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976178"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="3207d-103">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3207d-103">Get termsAndConditions</span></span>

> <span data-ttu-id="3207d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3207d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3207d-105">Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="3207d-105">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3207d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3207d-106">Prerequisites</span></span>
<span data-ttu-id="3207d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3207d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3207d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3207d-109">Permission type</span></span>|<span data-ttu-id="3207d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3207d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3207d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3207d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3207d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3207d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3207d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3207d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3207d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3207d-114">Not supported.</span></span>|
|<span data-ttu-id="3207d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3207d-115">Application</span></span>|<span data-ttu-id="3207d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3207d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3207d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3207d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3207d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3207d-118">Optional query parameters</span></span>
<span data-ttu-id="3207d-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3207d-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3207d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3207d-120">Request headers</span></span>
|<span data-ttu-id="3207d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3207d-121">Header</span></span>|<span data-ttu-id="3207d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3207d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3207d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3207d-123">Authorization</span></span>|<span data-ttu-id="3207d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3207d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3207d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3207d-125">Accept</span></span>|<span data-ttu-id="3207d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3207d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3207d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3207d-127">Request body</span></span>
<span data-ttu-id="3207d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3207d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3207d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3207d-129">Response</span></span>
<span data-ttu-id="3207d-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3207d-130">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3207d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3207d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3207d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3207d-132">Request</span></span>
<span data-ttu-id="3207d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3207d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="3207d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3207d-134">Response</span></span>
<span data-ttu-id="3207d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3207d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7
  }
}
```



