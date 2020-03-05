---
title: Get managedAppPolicy
description: Чтение свойств и связей объекта managedAppPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 202e777f168870c85afc3c431e2559b7db39b375
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463484"
---
# <a name="get-managedapppolicy"></a><span data-ttu-id="36d1c-103">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="36d1c-103">Get managedAppPolicy</span></span>

<span data-ttu-id="36d1c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="36d1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36d1c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36d1c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36d1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36d1c-107">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="36d1c-107">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36d1c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="36d1c-108">Prerequisites</span></span>
<span data-ttu-id="36d1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36d1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36d1c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36d1c-111">Permission type</span></span>|<span data-ttu-id="36d1c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36d1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36d1c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36d1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36d1c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="36d1c-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="36d1c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36d1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36d1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d1c-116">Not supported.</span></span>|
|<span data-ttu-id="36d1c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36d1c-117">Application</span></span>|<span data-ttu-id="36d1c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="36d1c-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36d1c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36d1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36d1c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="36d1c-120">Optional query parameters</span></span>
<span data-ttu-id="36d1c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="36d1c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36d1c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36d1c-122">Request headers</span></span>
|<span data-ttu-id="36d1c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36d1c-123">Header</span></span>|<span data-ttu-id="36d1c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="36d1c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36d1c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="36d1c-125">Authorization</span></span>|<span data-ttu-id="36d1c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36d1c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36d1c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="36d1c-127">Accept</span></span>|<span data-ttu-id="36d1c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="36d1c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36d1c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36d1c-129">Request body</span></span>
<span data-ttu-id="36d1c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36d1c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36d1c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="36d1c-131">Response</span></span>
<span data-ttu-id="36d1c-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="36d1c-132">If successful, this method returns a `200 OK` response code and [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36d1c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="36d1c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="36d1c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="36d1c-134">Request</span></span>
<span data-ttu-id="36d1c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36d1c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="36d1c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="36d1c-136">Response</span></span>
<span data-ttu-id="36d1c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36d1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





