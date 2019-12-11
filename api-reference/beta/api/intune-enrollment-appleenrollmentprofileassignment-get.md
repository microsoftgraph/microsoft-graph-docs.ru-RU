---
title: Получение Апплинроллментпрофилеассигнмент
description: Чтение свойств и связей объекта Апплинроллментпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aef5bbd8fd83ce5a3148096cb76d48bfec75282b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944148"
---
# <a name="get-appleenrollmentprofileassignment"></a><span data-ttu-id="f1a10-103">Получение Апплинроллментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="f1a10-103">Get appleEnrollmentProfileAssignment</span></span>

> <span data-ttu-id="f1a10-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1a10-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1a10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1a10-106">Чтение свойств и связей объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f1a10-106">Read properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1a10-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1a10-107">Prerequisites</span></span>
<span data-ttu-id="f1a10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a10-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a10-110">Permission type</span></span>|<span data-ttu-id="f1a10-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1a10-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1a10-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1a10-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f1a10-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1a10-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a10-115">Not supported.</span></span>|
|<span data-ttu-id="f1a10-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1a10-116">Application</span></span>|<span data-ttu-id="f1a10-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1a10-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1a10-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1a10-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f1a10-119">Optional query parameters</span></span>
<span data-ttu-id="f1a10-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f1a10-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1a10-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1a10-121">Request headers</span></span>
|<span data-ttu-id="f1a10-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1a10-122">Header</span></span>|<span data-ttu-id="f1a10-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a10-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1a10-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a10-124">Authorization</span></span>|<span data-ttu-id="f1a10-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a10-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1a10-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f1a10-126">Accept</span></span>|<span data-ttu-id="f1a10-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f1a10-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1a10-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1a10-128">Request body</span></span>
<span data-ttu-id="f1a10-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1a10-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1a10-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1a10-130">Response</span></span>
<span data-ttu-id="f1a10-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a10-131">If successful, this method returns a `200 OK` response code and [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a10-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f1a10-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1a10-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a10-133">Request</span></span>
<span data-ttu-id="f1a10-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a10-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f1a10-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a10-135">Response</span></span>
<span data-ttu-id="f1a10-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
    "id": "5b603771-3771-5b60-7137-605b7137605b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





