---
title: Get termsAndConditions
description: Чтение свойств и связей объекта termsAndConditions.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bc87715b6d497395449138ef75a3c1e50e1d04e4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417086"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="ed8f1-103">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="ed8f1-103">Get termsAndConditions</span></span>

> <span data-ttu-id="ed8f1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed8f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed8f1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed8f1-107">Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="ed8f1-107">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed8f1-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ed8f1-108">Prerequisites</span></span>
<span data-ttu-id="ed8f1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed8f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed8f1-111">Permission type</span></span>|<span data-ttu-id="ed8f1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed8f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed8f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed8f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed8f1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed8f1-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ed8f1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed8f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed8f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-116">Not supported.</span></span>|
|<span data-ttu-id="ed8f1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed8f1-117">Application</span></span>|<span data-ttu-id="ed8f1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed8f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed8f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed8f1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ed8f1-120">Optional query parameters</span></span>
<span data-ttu-id="ed8f1-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed8f1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed8f1-122">Request headers</span></span>
|<span data-ttu-id="ed8f1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed8f1-123">Header</span></span>|<span data-ttu-id="ed8f1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ed8f1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed8f1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed8f1-125">Authorization</span></span>|<span data-ttu-id="ed8f1-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed8f1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed8f1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ed8f1-127">Accept</span></span>|<span data-ttu-id="ed8f1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ed8f1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed8f1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed8f1-129">Request body</span></span>
<span data-ttu-id="ed8f1-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed8f1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed8f1-131">Response</span></span>
<span data-ttu-id="ed8f1-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-132">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed8f1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ed8f1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed8f1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed8f1-134">Request</span></span>
<span data-ttu-id="ed8f1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="ed8f1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed8f1-136">Response</span></span>
<span data-ttu-id="ed8f1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ed8f1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
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




