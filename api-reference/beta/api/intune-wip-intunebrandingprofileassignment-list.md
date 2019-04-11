---
title: Список Интунебрандингпрофилеассигнментс
description: Список свойств и связей объектов Интунебрандингпрофилеассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10b728c7a371a7fcf5dadd28b5884048d3758a95
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775781"
---
# <a name="list-intunebrandingprofileassignments"></a><span data-ttu-id="9d953-103">Список Интунебрандингпрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="9d953-103">List intuneBrandingProfileAssignments</span></span>

> <span data-ttu-id="9d953-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d953-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d953-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d953-106">Список свойств и связей объектов [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9d953-106">List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d953-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d953-107">Prerequisites</span></span>
<span data-ttu-id="9d953-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d953-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d953-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d953-110">Permission type</span></span>|<span data-ttu-id="9d953-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d953-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d953-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d953-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d953-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d953-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9d953-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d953-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d953-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d953-115">Not supported.</span></span>|
|<span data-ttu-id="9d953-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d953-116">Application</span></span>|<span data-ttu-id="9d953-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d953-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d953-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d953-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9d953-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d953-119">Request headers</span></span>
|<span data-ttu-id="9d953-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d953-120">Header</span></span>|<span data-ttu-id="9d953-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9d953-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d953-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d953-122">Authorization</span></span>|<span data-ttu-id="9d953-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d953-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d953-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9d953-124">Accept</span></span>|<span data-ttu-id="9d953-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d953-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d953-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d953-126">Request body</span></span>
<span data-ttu-id="9d953-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d953-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d953-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d953-128">Response</span></span>
<span data-ttu-id="9d953-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d953-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d953-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9d953-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d953-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d953-131">Request</span></span>
<span data-ttu-id="9d953-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d953-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="9d953-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d953-133">Response</span></span>
<span data-ttu-id="9d953-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d953-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





