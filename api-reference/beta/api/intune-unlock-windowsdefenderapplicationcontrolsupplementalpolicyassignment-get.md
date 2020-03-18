---
title: Получение Виндовсдефендераппликатионконтролсупплементалполициассигнмент
description: Чтение свойств и связей объекта Виндовсдефендераппликатионконтролсупплементалполициассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 524c330c0d66d5535b93fa70e146907f38e0d41b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799817"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="10be1-103">Получение Виндовсдефендераппликатионконтролсупплементалполициассигнмент</span><span class="sxs-lookup"><span data-stu-id="10be1-103">Get windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="10be1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10be1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10be1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10be1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10be1-106">Чтение свойств и связей объекта [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="10be1-106">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10be1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10be1-107">Prerequisites</span></span>
<span data-ttu-id="10be1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10be1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10be1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10be1-110">Permission type</span></span>|<span data-ttu-id="10be1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10be1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10be1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10be1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10be1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10be1-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10be1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10be1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10be1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10be1-115">Not supported.</span></span>|
|<span data-ttu-id="10be1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="10be1-116">Application</span></span>|<span data-ttu-id="10be1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10be1-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10be1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10be1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10be1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10be1-119">Optional query parameters</span></span>
<span data-ttu-id="10be1-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10be1-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10be1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10be1-121">Request headers</span></span>
|<span data-ttu-id="10be1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10be1-122">Header</span></span>|<span data-ttu-id="10be1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="10be1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10be1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="10be1-124">Authorization</span></span>|<span data-ttu-id="10be1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10be1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10be1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="10be1-126">Accept</span></span>|<span data-ttu-id="10be1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="10be1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10be1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10be1-128">Request body</span></span>
<span data-ttu-id="10be1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10be1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10be1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="10be1-130">Response</span></span>
<span data-ttu-id="10be1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполициассигнмент](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10be1-131">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10be1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="10be1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="10be1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10be1-133">Request</span></span>
<span data-ttu-id="10be1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10be1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="10be1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="10be1-135">Response</span></span>
<span data-ttu-id="10be1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10be1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
    "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




