---
title: Удаление Депмакосенроллментпрофиле
description: Удаляет объект Депмакосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 223a0e34a08c7a2bfb75511f8370f9a548a87e6c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166964"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="13eed-103">Удаление Депмакосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="13eed-103">Delete depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="13eed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13eed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13eed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13eed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13eed-106">Удаляет объект [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="13eed-106">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13eed-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13eed-107">Prerequisites</span></span>
<span data-ttu-id="13eed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13eed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13eed-110">Permission type</span></span>|<span data-ttu-id="13eed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13eed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13eed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13eed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13eed-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13eed-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="13eed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13eed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13eed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13eed-115">Not supported.</span></span>|
|<span data-ttu-id="13eed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13eed-116">Application</span></span>|<span data-ttu-id="13eed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13eed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13eed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13eed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="13eed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13eed-119">Request headers</span></span>
|<span data-ttu-id="13eed-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13eed-120">Header</span></span>|<span data-ttu-id="13eed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13eed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13eed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13eed-122">Authorization</span></span>|<span data-ttu-id="13eed-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="13eed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13eed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="13eed-124">Accept</span></span>|<span data-ttu-id="13eed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13eed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13eed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13eed-126">Request body</span></span>
<span data-ttu-id="13eed-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13eed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13eed-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="13eed-128">Response</span></span>
<span data-ttu-id="13eed-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="13eed-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="13eed-130">Пример</span><span class="sxs-lookup"><span data-stu-id="13eed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="13eed-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="13eed-131">Request</span></span>
<span data-ttu-id="13eed-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13eed-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="13eed-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="13eed-133">Response</span></span>
<span data-ttu-id="13eed-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13eed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




