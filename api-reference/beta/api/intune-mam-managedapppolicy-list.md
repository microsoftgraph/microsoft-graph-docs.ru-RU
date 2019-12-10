---
title: Перечисление объектов managedAppPolicy
description: Список свойств и связей объектов managedAppPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c34710300674f4cd6f38c38294ca1a3b4a0ce45
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942424"
---
# <a name="list-managedapppolicies"></a><span data-ttu-id="8c74d-103">Перечисление объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8c74d-103">List managedAppPolicies</span></span>

> <span data-ttu-id="8c74d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c74d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c74d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c74d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c74d-106">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8c74d-106">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c74d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c74d-107">Prerequisites</span></span>
<span data-ttu-id="8c74d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c74d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c74d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c74d-110">Permission type</span></span>|<span data-ttu-id="8c74d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c74d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c74d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c74d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c74d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c74d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8c74d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c74d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c74d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c74d-115">Not supported.</span></span>|
|<span data-ttu-id="8c74d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c74d-116">Application</span></span>|<span data-ttu-id="8c74d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c74d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c74d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c74d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8c74d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8c74d-119">Request headers</span></span>
|<span data-ttu-id="8c74d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c74d-120">Header</span></span>|<span data-ttu-id="8c74d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8c74d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c74d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c74d-122">Authorization</span></span>|<span data-ttu-id="8c74d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c74d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c74d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8c74d-124">Accept</span></span>|<span data-ttu-id="8c74d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c74d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c74d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c74d-126">Request body</span></span>
<span data-ttu-id="8c74d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c74d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c74d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c74d-128">Response</span></span>
<span data-ttu-id="8c74d-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c74d-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c74d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8c74d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c74d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c74d-131">Request</span></span>
<span data-ttu-id="8c74d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c74d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="8c74d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c74d-133">Response</span></span>
<span data-ttu-id="8c74d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c74d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "value": [
    {
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
  ]
}
```





