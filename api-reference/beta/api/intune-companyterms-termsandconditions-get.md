---
title: Get termsAndConditions
description: Чтение свойств и связей объекта termsAndConditions.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea09ded1dac537798b86fa35a361015bfac1fe35
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085080"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="8269b-103">Get termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="8269b-103">Get termsAndConditions</span></span>

> <span data-ttu-id="8269b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8269b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8269b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8269b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8269b-106">Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="8269b-106">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8269b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8269b-107">Prerequisites</span></span>
<span data-ttu-id="8269b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8269b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8269b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8269b-110">Permission type</span></span>|<span data-ttu-id="8269b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8269b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8269b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8269b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8269b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8269b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8269b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8269b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8269b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8269b-115">Not supported.</span></span>|
|<span data-ttu-id="8269b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8269b-116">Application</span></span>|<span data-ttu-id="8269b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8269b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8269b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8269b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8269b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8269b-119">Optional query parameters</span></span>
<span data-ttu-id="8269b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8269b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8269b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8269b-121">Request headers</span></span>
|<span data-ttu-id="8269b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8269b-122">Header</span></span>|<span data-ttu-id="8269b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8269b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8269b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8269b-124">Authorization</span></span>|<span data-ttu-id="8269b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8269b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8269b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8269b-126">Accept</span></span>|<span data-ttu-id="8269b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8269b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8269b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8269b-128">Request body</span></span>
<span data-ttu-id="8269b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8269b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8269b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8269b-130">Response</span></span>
<span data-ttu-id="8269b-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8269b-131">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8269b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8269b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8269b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8269b-133">Request</span></span>
<span data-ttu-id="8269b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8269b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="8269b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8269b-135">Response</span></span>
<span data-ttu-id="8269b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8269b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






