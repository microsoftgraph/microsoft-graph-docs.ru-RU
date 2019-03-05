---
title: Действие setDefaultProfile
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db1ab2e894ea80d0b32ecc4f726ee9a43d94818a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141673"
---
# <a name="setdefaultprofile-action"></a><span data-ttu-id="e04fe-103">Действие setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="e04fe-103">setDefaultProfile action</span></span>

> <span data-ttu-id="e04fe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e04fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e04fe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e04fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e04fe-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e04fe-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e04fe-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e04fe-107">Prerequisites</span></span>
<span data-ttu-id="e04fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e04fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e04fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e04fe-110">Permission type</span></span>|<span data-ttu-id="e04fe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e04fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e04fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e04fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e04fe-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e04fe-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e04fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e04fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e04fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e04fe-115">Not supported.</span></span>|
|<span data-ttu-id="e04fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e04fe-116">Application</span></span>|<span data-ttu-id="e04fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e04fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e04fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e04fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

## <a name="request-headers"></a><span data-ttu-id="e04fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e04fe-119">Request headers</span></span>
|<span data-ttu-id="e04fe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e04fe-120">Header</span></span>|<span data-ttu-id="e04fe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e04fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e04fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e04fe-122">Authorization</span></span>|<span data-ttu-id="e04fe-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e04fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e04fe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e04fe-124">Accept</span></span>|<span data-ttu-id="e04fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e04fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e04fe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e04fe-126">Request body</span></span>
<span data-ttu-id="e04fe-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e04fe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e04fe-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e04fe-128">Response</span></span>
<span data-ttu-id="e04fe-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e04fe-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e04fe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e04fe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e04fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e04fe-131">Request</span></span>
<span data-ttu-id="e04fe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e04fe-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

### <a name="response"></a><span data-ttu-id="e04fe-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="e04fe-133">Response</span></span>
<span data-ttu-id="e04fe-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e04fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




