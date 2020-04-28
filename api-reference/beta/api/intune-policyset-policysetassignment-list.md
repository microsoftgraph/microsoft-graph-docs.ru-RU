---
title: Список Полицисетассигнментс
description: Список свойств и связей объектов Полицисетассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c939334f8c2a6bc950560a161520898c8150267
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471303"
---
# <a name="list-policysetassignments"></a><span data-ttu-id="c9b23-103">Список Полицисетассигнментс</span><span class="sxs-lookup"><span data-stu-id="c9b23-103">List policySetAssignments</span></span>

<span data-ttu-id="c9b23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9b23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9b23-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9b23-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9b23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9b23-107">Список свойств и связей объектов [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c9b23-107">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9b23-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9b23-108">Prerequisites</span></span>
<span data-ttu-id="c9b23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9b23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9b23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9b23-111">Permission type</span></span>|<span data-ttu-id="c9b23-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9b23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9b23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9b23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9b23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9b23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9b23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9b23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9b23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9b23-116">Not supported.</span></span>|
|<span data-ttu-id="c9b23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9b23-117">Application</span></span>|<span data-ttu-id="c9b23-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9b23-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9b23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9b23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c9b23-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9b23-120">Request headers</span></span>
|<span data-ttu-id="c9b23-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9b23-121">Header</span></span>|<span data-ttu-id="c9b23-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9b23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9b23-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9b23-123">Authorization</span></span>|<span data-ttu-id="c9b23-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9b23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9b23-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9b23-125">Accept</span></span>|<span data-ttu-id="c9b23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9b23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9b23-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9b23-127">Request body</span></span>
<span data-ttu-id="c9b23-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9b23-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9b23-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9b23-129">Response</span></span>
<span data-ttu-id="c9b23-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9b23-130">If successful, this method returns a `200 OK` response code and a collection of [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9b23-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c9b23-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9b23-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9b23-132">Request</span></span>
<span data-ttu-id="c9b23-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9b23-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
```

### <a name="response"></a><span data-ttu-id="c9b23-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9b23-134">Response</span></span>
<span data-ttu-id="c9b23-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9b23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySetAssignment",
      "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



