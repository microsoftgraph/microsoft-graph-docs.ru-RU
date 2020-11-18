---
title: Удаление Депмакосенроллментпрофиле
description: Удаляет объект Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cfcda1f128b7fb95ef0487e6d9fbe76e2b0408d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201928"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="b6634-103">Удаление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="b6634-103">Delete depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="b6634-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6634-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6634-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6634-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6634-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6634-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6634-107">Удаляет объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b6634-107">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6634-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6634-108">Prerequisites</span></span>
<span data-ttu-id="b6634-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6634-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6634-111">Permission type</span></span>|<span data-ttu-id="b6634-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6634-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6634-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6634-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6634-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6634-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6634-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6634-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6634-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6634-116">Not supported.</span></span>|
|<span data-ttu-id="b6634-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b6634-117">Application</span></span>|<span data-ttu-id="b6634-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6634-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6634-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6634-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="b6634-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6634-120">Request headers</span></span>
|<span data-ttu-id="b6634-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6634-121">Header</span></span>|<span data-ttu-id="b6634-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6634-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6634-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6634-123">Authorization</span></span>|<span data-ttu-id="b6634-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6634-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6634-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6634-125">Accept</span></span>|<span data-ttu-id="b6634-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6634-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6634-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6634-127">Request body</span></span>
<span data-ttu-id="b6634-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6634-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6634-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6634-129">Response</span></span>
<span data-ttu-id="b6634-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b6634-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6634-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b6634-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6634-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6634-132">Request</span></span>
<span data-ttu-id="b6634-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6634-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="b6634-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6634-134">Response</span></span>
<span data-ttu-id="b6634-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6634-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




