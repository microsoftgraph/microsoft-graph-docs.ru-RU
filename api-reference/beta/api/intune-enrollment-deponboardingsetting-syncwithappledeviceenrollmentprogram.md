---
title: Действие syncWithAppleDeviceEnrollmentProgram
description: Синхронизация между программой регистрации устройств Apple и Intune
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3ab3225fa30431b72b38f51c0d2cc5354d38fc5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981554"
---
# <a name="syncwithappledeviceenrollmentprogram-action"></a><span data-ttu-id="67fc4-103">Действие syncWithAppleDeviceEnrollmentProgram</span><span class="sxs-lookup"><span data-stu-id="67fc4-103">syncWithAppleDeviceEnrollmentProgram action</span></span>

> <span data-ttu-id="67fc4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67fc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67fc4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67fc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fc4-106">Синхронизация между программой регистрации устройств Apple и Intune</span><span class="sxs-lookup"><span data-stu-id="67fc4-106">Synchronizes between Apple Device Enrollment Program and Intune</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67fc4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="67fc4-107">Prerequisites</span></span>
<span data-ttu-id="67fc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67fc4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67fc4-110">Permission type</span></span>|<span data-ttu-id="67fc4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67fc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67fc4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67fc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67fc4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67fc4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67fc4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67fc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67fc4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67fc4-115">Not supported.</span></span>|
|<span data-ttu-id="67fc4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67fc4-116">Application</span></span>|<span data-ttu-id="67fc4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67fc4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67fc4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67fc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/syncWithAppleDeviceEnrollmentProgram
```

## <a name="request-headers"></a><span data-ttu-id="67fc4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67fc4-119">Request headers</span></span>
|<span data-ttu-id="67fc4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67fc4-120">Header</span></span>|<span data-ttu-id="67fc4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="67fc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67fc4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67fc4-122">Authorization</span></span>|<span data-ttu-id="67fc4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67fc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67fc4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="67fc4-124">Accept</span></span>|<span data-ttu-id="67fc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67fc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67fc4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67fc4-126">Request body</span></span>
<span data-ttu-id="67fc4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67fc4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67fc4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="67fc4-128">Response</span></span>
<span data-ttu-id="67fc4-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67fc4-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="67fc4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="67fc4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="67fc4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="67fc4-131">Request</span></span>
<span data-ttu-id="67fc4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67fc4-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/syncWithAppleDeviceEnrollmentProgram
```

### <a name="response"></a><span data-ttu-id="67fc4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="67fc4-133">Response</span></span>
<span data-ttu-id="67fc4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67fc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





