---
title: Получение Виндовсдефендераппликатионконтролсупплементалполици
description: Чтение свойств и связей объекта Виндовсдефендераппликатионконтролсупплементалполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2767666632b45357c4f690d4ad545a6e41bcc8ce
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938889"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="860ea-103">Получение Виндовсдефендераппликатионконтролсупплементалполици</span><span class="sxs-lookup"><span data-stu-id="860ea-103">Get windowsDefenderApplicationControlSupplementalPolicy</span></span>

> <span data-ttu-id="860ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="860ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="860ea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="860ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="860ea-106">Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="860ea-106">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="860ea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="860ea-107">Prerequisites</span></span>
<span data-ttu-id="860ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="860ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="860ea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="860ea-110">Permission type</span></span>|<span data-ttu-id="860ea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="860ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="860ea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="860ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="860ea-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="860ea-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="860ea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="860ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="860ea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="860ea-115">Not supported.</span></span>|
|<span data-ttu-id="860ea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="860ea-116">Application</span></span>|<span data-ttu-id="860ea-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="860ea-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="860ea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="860ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="860ea-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="860ea-119">Optional query parameters</span></span>
<span data-ttu-id="860ea-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="860ea-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="860ea-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="860ea-121">Request headers</span></span>
|<span data-ttu-id="860ea-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="860ea-122">Header</span></span>|<span data-ttu-id="860ea-123">Значение</span><span class="sxs-lookup"><span data-stu-id="860ea-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="860ea-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="860ea-124">Authorization</span></span>|<span data-ttu-id="860ea-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="860ea-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="860ea-126">Accept</span><span class="sxs-lookup"><span data-stu-id="860ea-126">Accept</span></span>|<span data-ttu-id="860ea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="860ea-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="860ea-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="860ea-128">Request body</span></span>
<span data-ttu-id="860ea-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="860ea-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="860ea-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="860ea-130">Response</span></span>
<span data-ttu-id="860ea-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="860ea-131">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="860ea-132">Пример</span><span class="sxs-lookup"><span data-stu-id="860ea-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="860ea-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="860ea-133">Request</span></span>
<span data-ttu-id="860ea-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="860ea-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
```

### <a name="response"></a><span data-ttu-id="860ea-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="860ea-135">Response</span></span>
<span data-ttu-id="860ea-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="860ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
    "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
    "displayName": "Display Name value",
    "description": "Description value",
    "content": "Y29udGVudA==",
    "contentFileName": "Content File Name value",
    "version": "Version value",
    "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```





