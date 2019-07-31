---
title: Get managedAppConfiguration
description: Чтение свойств и связей объекта managedAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb0d6e34ab0367a4a904f63ff670f3b9986c2977
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994782"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="39529-103">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="39529-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="39529-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39529-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39529-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39529-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39529-106">Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39529-106">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39529-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="39529-107">Prerequisites</span></span>
<span data-ttu-id="39529-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39529-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39529-110">Permission type</span></span>|<span data-ttu-id="39529-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39529-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39529-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39529-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39529-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="39529-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="39529-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39529-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39529-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39529-115">Not supported.</span></span>|
|<span data-ttu-id="39529-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39529-116">Application</span></span>|<span data-ttu-id="39529-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39529-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39529-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39529-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39529-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="39529-119">Optional query parameters</span></span>
<span data-ttu-id="39529-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="39529-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39529-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39529-121">Request headers</span></span>
|<span data-ttu-id="39529-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39529-122">Header</span></span>|<span data-ttu-id="39529-123">Значение</span><span class="sxs-lookup"><span data-stu-id="39529-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39529-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39529-124">Authorization</span></span>|<span data-ttu-id="39529-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39529-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39529-126">Accept</span><span class="sxs-lookup"><span data-stu-id="39529-126">Accept</span></span>|<span data-ttu-id="39529-127">application/json</span><span class="sxs-lookup"><span data-stu-id="39529-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39529-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39529-128">Request body</span></span>
<span data-ttu-id="39529-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39529-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39529-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="39529-130">Response</span></span>
<span data-ttu-id="39529-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="39529-131">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39529-132">Пример</span><span class="sxs-lookup"><span data-stu-id="39529-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="39529-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="39529-133">Request</span></span>
<span data-ttu-id="39529-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39529-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="39529-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="39529-135">Response</span></span>
<span data-ttu-id="39529-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39529-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 618

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```





