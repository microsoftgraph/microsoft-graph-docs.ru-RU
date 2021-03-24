---
title: Get termsAndConditions
description: Чтение свойств и связей объекта termsAndConditions.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d1b4c75ddd8de00b85d0fc98deb8fd613074d77d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133642"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="79886-103">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="79886-103">Get termsAndConditions</span></span>

<span data-ttu-id="79886-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79886-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79886-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79886-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79886-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79886-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79886-107">Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="79886-107">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79886-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="79886-108">Prerequisites</span></span>
<span data-ttu-id="79886-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79886-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79886-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79886-111">Permission type</span></span>|<span data-ttu-id="79886-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79886-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79886-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79886-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79886-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79886-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="79886-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79886-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79886-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79886-116">Not supported.</span></span>|
|<span data-ttu-id="79886-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="79886-117">Application</span></span>|<span data-ttu-id="79886-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79886-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79886-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79886-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79886-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79886-120">Optional query parameters</span></span>
<span data-ttu-id="79886-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="79886-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79886-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79886-122">Request headers</span></span>
|<span data-ttu-id="79886-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79886-123">Header</span></span>|<span data-ttu-id="79886-124">Значение</span><span class="sxs-lookup"><span data-stu-id="79886-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79886-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="79886-125">Authorization</span></span>|<span data-ttu-id="79886-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79886-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79886-127">Accept</span><span class="sxs-lookup"><span data-stu-id="79886-127">Accept</span></span>|<span data-ttu-id="79886-128">application/json</span><span class="sxs-lookup"><span data-stu-id="79886-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79886-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79886-129">Request body</span></span>
<span data-ttu-id="79886-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79886-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79886-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="79886-131">Response</span></span>
<span data-ttu-id="79886-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="79886-132">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79886-133">Пример</span><span class="sxs-lookup"><span data-stu-id="79886-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="79886-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="79886-134">Request</span></span>
<span data-ttu-id="79886-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79886-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="79886-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="79886-136">Response</span></span>
<span data-ttu-id="79886-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79886-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 614

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
    "version": 7,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




