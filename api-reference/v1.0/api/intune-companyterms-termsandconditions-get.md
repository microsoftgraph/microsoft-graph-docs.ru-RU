---
title: Get termsAndConditions
description: Чтение свойств и связей объекта termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bf00c3b04d69dec54e19e74ca56a5565fd17e6c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468925"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="c8659-103">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="c8659-103">Get termsAndConditions</span></span>

<span data-ttu-id="c8659-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8659-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8659-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8659-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8659-106">Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="c8659-106">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8659-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c8659-107">Prerequisites</span></span>
<span data-ttu-id="c8659-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8659-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8659-110">Permission type</span></span>|<span data-ttu-id="c8659-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8659-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8659-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8659-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8659-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8659-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c8659-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8659-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8659-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8659-115">Not supported.</span></span>|
|<span data-ttu-id="c8659-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8659-116">Application</span></span>|<span data-ttu-id="c8659-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8659-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8659-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8659-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8659-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8659-119">Optional query parameters</span></span>
<span data-ttu-id="c8659-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c8659-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8659-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8659-121">Request headers</span></span>
|<span data-ttu-id="c8659-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8659-122">Header</span></span>|<span data-ttu-id="c8659-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c8659-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8659-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8659-124">Authorization</span></span>|<span data-ttu-id="c8659-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8659-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8659-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c8659-126">Accept</span></span>|<span data-ttu-id="c8659-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c8659-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8659-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c8659-128">Request body</span></span>
<span data-ttu-id="c8659-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8659-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8659-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8659-130">Response</span></span>
<span data-ttu-id="c8659-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c8659-131">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8659-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c8659-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8659-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8659-133">Request</span></span>
<span data-ttu-id="c8659-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8659-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="c8659-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8659-135">Response</span></span>
<span data-ttu-id="c8659-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8659-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






