---
title: Действие unshareForSchoolDataSyncService
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20e682286c2f825cc7f9392a817913cd176fa56b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813220"
---
# <a name="unshareforschooldatasyncservice-action"></a><span data-ttu-id="c184e-103">Действие unshareForSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="c184e-103">unshareForSchoolDataSyncService action</span></span>

> <span data-ttu-id="c184e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c184e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c184e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c184e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c184e-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c184e-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c184e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c184e-107">Prerequisites</span></span>
<span data-ttu-id="c184e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c184e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c184e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c184e-110">Permission type</span></span>|<span data-ttu-id="c184e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c184e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c184e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c184e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c184e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c184e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c184e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c184e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c184e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c184e-115">Not supported.</span></span>|
|<span data-ttu-id="c184e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c184e-116">Application</span></span>|<span data-ttu-id="c184e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c184e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c184e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c184e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/unshareForSchoolDataSyncService
```

## <a name="request-headers"></a><span data-ttu-id="c184e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c184e-119">Request headers</span></span>
|<span data-ttu-id="c184e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c184e-120">Header</span></span>|<span data-ttu-id="c184e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c184e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c184e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c184e-122">Authorization</span></span>|<span data-ttu-id="c184e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c184e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c184e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c184e-124">Accept</span></span>|<span data-ttu-id="c184e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c184e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c184e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c184e-126">Request body</span></span>
<span data-ttu-id="c184e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c184e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c184e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c184e-128">Response</span></span>
<span data-ttu-id="c184e-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c184e-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c184e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c184e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c184e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c184e-131">Request</span></span>
<span data-ttu-id="c184e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c184e-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/unshareForSchoolDataSyncService
```

### <a name="response"></a><span data-ttu-id="c184e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c184e-133">Response</span></span>
<span data-ttu-id="c184e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c184e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




