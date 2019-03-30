---
title: Get managedAppPolicy
description: Чтение свойств и связей объекта managedAppPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7593b2d5a12d68c0e4669749b2a52cff3982fb2b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988548"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="4fa9d-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="4fa9d-103">Get managedAppPolicy</span></span>

> <span data-ttu-id="4fa9d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fa9d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fa9d-106">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4fa9d-106">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fa9d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa9d-107">Prerequisites</span></span>
<span data-ttu-id="4fa9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fa9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fa9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa9d-110">Permission type</span></span>|<span data-ttu-id="4fa9d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fa9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fa9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fa9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fa9d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fa9d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4fa9d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fa9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fa9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-115">Not supported.</span></span>|
|<span data-ttu-id="4fa9d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fa9d-116">Application</span></span>|<span data-ttu-id="4fa9d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fa9d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fa9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4fa9d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4fa9d-119">Optional query parameters</span></span>
<span data-ttu-id="4fa9d-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fa9d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fa9d-121">Request headers</span></span>
|<span data-ttu-id="4fa9d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fa9d-122">Header</span></span>|<span data-ttu-id="4fa9d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4fa9d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fa9d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fa9d-124">Authorization</span></span>|<span data-ttu-id="4fa9d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fa9d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4fa9d-126">Accept</span></span>|<span data-ttu-id="4fa9d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4fa9d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fa9d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fa9d-128">Request body</span></span>
<span data-ttu-id="4fa9d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fa9d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fa9d-130">Response</span></span>
<span data-ttu-id="4fa9d-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-131">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fa9d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4fa9d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fa9d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fa9d-133">Request</span></span>
<span data-ttu-id="4fa9d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="4fa9d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fa9d-135">Response</span></span>
<span data-ttu-id="4fa9d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fa9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
    "version": "Version value"
  }
}
```




