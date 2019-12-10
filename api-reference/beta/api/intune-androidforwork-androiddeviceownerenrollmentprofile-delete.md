---
title: Удаление Андроиддевицеовнеренроллментпрофиле
description: Удаляет объект Андроиддевицеовнеренроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 31976f18d15cf903d006fb250273f5b506c2bbdb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39923562"
---
# <a name="delete-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="0eafd-103">Удаление Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="0eafd-103">Delete androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="0eafd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eafd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eafd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eafd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eafd-106">Удаляет объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0eafd-106">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eafd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0eafd-107">Prerequisites</span></span>
<span data-ttu-id="0eafd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eafd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eafd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eafd-110">Permission type</span></span>|<span data-ttu-id="0eafd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eafd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eafd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eafd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0eafd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eafd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0eafd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eafd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eafd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eafd-115">Not supported.</span></span>|
|<span data-ttu-id="0eafd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eafd-116">Application</span></span>|<span data-ttu-id="0eafd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eafd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eafd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eafd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0eafd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0eafd-119">Request headers</span></span>
|<span data-ttu-id="0eafd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0eafd-120">Header</span></span>|<span data-ttu-id="0eafd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0eafd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eafd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eafd-122">Authorization</span></span>|<span data-ttu-id="0eafd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eafd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eafd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0eafd-124">Accept</span></span>|<span data-ttu-id="0eafd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0eafd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eafd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0eafd-126">Request body</span></span>
<span data-ttu-id="0eafd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0eafd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eafd-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="0eafd-128">Response</span></span>
<span data-ttu-id="0eafd-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0eafd-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0eafd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0eafd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eafd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eafd-131">Request</span></span>
<span data-ttu-id="0eafd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eafd-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="0eafd-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0eafd-133">Response</span></span>
<span data-ttu-id="0eafd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eafd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





