---
title: Список Интунебрандингпрофилеассигнментс
description: Список свойств и связей объектов Интунебрандингпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ec2c844b798ee24e787b05d5db45ab203e09a27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457400"
---
# <a name="list-intunebrandingprofileassignments"></a><span data-ttu-id="2df2f-103">Список Интунебрандингпрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="2df2f-103">List intuneBrandingProfileAssignments</span></span>

<span data-ttu-id="2df2f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2df2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2df2f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2df2f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2df2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2df2f-107">Список свойств и связей объектов [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2df2f-107">List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2df2f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2df2f-108">Prerequisites</span></span>
<span data-ttu-id="2df2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2df2f-111">Permission type</span></span>|<span data-ttu-id="2df2f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2df2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2df2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2df2f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df2f-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2df2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2df2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df2f-116">Not supported.</span></span>|
|<span data-ttu-id="2df2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2df2f-117">Application</span></span>|<span data-ttu-id="2df2f-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df2f-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2df2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2df2f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2df2f-120">Request headers</span></span>
|<span data-ttu-id="2df2f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2df2f-121">Header</span></span>|<span data-ttu-id="2df2f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2df2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df2f-123">Authorization</span></span>|<span data-ttu-id="2df2f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2df2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2df2f-125">Accept</span></span>|<span data-ttu-id="2df2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2df2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df2f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2df2f-127">Request body</span></span>
<span data-ttu-id="2df2f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2df2f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df2f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2df2f-129">Response</span></span>
<span data-ttu-id="2df2f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2df2f-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df2f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2df2f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2df2f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2df2f-132">Request</span></span>
<span data-ttu-id="2df2f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2df2f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="2df2f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2df2f-134">Response</span></span>
<span data-ttu-id="2df2f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2df2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





