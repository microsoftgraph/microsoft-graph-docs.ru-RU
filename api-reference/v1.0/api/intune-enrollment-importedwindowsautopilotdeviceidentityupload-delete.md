---
title: Удаление Импортедвиндовсаутопилотдевицеидентитюплоад
description: Удаляет объект Импортедвиндовсаутопилотдевицеидентитюплоад.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ce6f21a7e40366ba7286fca9495f6d11e142a62
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996870"
---
# <a name="delete-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="ee270-103">Удаление Импортедвиндовсаутопилотдевицеидентитюплоад</span><span class="sxs-lookup"><span data-stu-id="ee270-103">Delete importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="ee270-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee270-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee270-105">Удаляет объект [импортедвиндовсаутопилотдевицеидентитюплоад](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span><span class="sxs-lookup"><span data-stu-id="ee270-105">Deletes a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee270-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee270-106">Prerequisites</span></span>
<span data-ttu-id="ee270-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee270-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee270-109">Permission type</span></span>|<span data-ttu-id="ee270-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee270-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee270-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee270-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee270-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee270-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ee270-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee270-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee270-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee270-114">Not supported.</span></span>|
|<span data-ttu-id="ee270-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee270-115">Application</span></span>|<span data-ttu-id="ee270-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee270-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee270-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee270-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="ee270-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee270-118">Request headers</span></span>
|<span data-ttu-id="ee270-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee270-119">Header</span></span>|<span data-ttu-id="ee270-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ee270-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee270-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee270-121">Authorization</span></span>|<span data-ttu-id="ee270-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee270-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee270-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ee270-123">Accept</span></span>|<span data-ttu-id="ee270-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ee270-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee270-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee270-125">Request body</span></span>
<span data-ttu-id="ee270-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee270-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee270-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee270-127">Response</span></span>
<span data-ttu-id="ee270-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee270-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ee270-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ee270-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee270-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee270-130">Request</span></span>
<span data-ttu-id="ee270-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee270-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

### <a name="response"></a><span data-ttu-id="ee270-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee270-132">Response</span></span>
<span data-ttu-id="ee270-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee270-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



