---
title: Удаление Депиосенроллментпрофиле
description: Удаляет объект Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 172934dcd8fef8bb38218b6cb678461d3bd215fb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442283"
---
# <a name="delete-depiosenrollmentprofile"></a><span data-ttu-id="6d520-103">Удаление Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="6d520-103">Delete depIOSEnrollmentProfile</span></span>

<span data-ttu-id="6d520-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d520-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d520-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d520-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d520-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d520-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d520-107">Удаляет объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6d520-107">Deletes a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d520-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d520-108">Prerequisites</span></span>
<span data-ttu-id="6d520-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d520-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d520-111">Permission type</span></span>|<span data-ttu-id="6d520-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d520-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d520-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d520-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d520-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d520-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6d520-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d520-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d520-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d520-116">Not supported.</span></span>|
|<span data-ttu-id="6d520-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d520-117">Application</span></span>|<span data-ttu-id="6d520-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d520-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d520-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d520-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="6d520-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6d520-120">Request headers</span></span>
|<span data-ttu-id="6d520-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d520-121">Header</span></span>|<span data-ttu-id="6d520-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d520-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d520-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d520-123">Authorization</span></span>|<span data-ttu-id="6d520-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d520-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d520-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d520-125">Accept</span></span>|<span data-ttu-id="6d520-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d520-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d520-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d520-127">Request body</span></span>
<span data-ttu-id="6d520-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d520-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d520-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d520-129">Response</span></span>
<span data-ttu-id="6d520-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6d520-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6d520-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6d520-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d520-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d520-132">Request</span></span>
<span data-ttu-id="6d520-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d520-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="6d520-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d520-134">Response</span></span>
<span data-ttu-id="6d520-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d520-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



