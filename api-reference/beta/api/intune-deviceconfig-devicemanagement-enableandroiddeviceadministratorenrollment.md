---
title: действие Енаблеандроиддевицеадминистраторенроллмент
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6437d769c1a88b23ac6e11368b8bba6bf3f295b8
ms.sourcegitcommit: 0f3e0bd7b57870a0f7b34cf52eaf4776ac82671e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2019
ms.locfileid: "36699088"
---
# <a name="enableandroiddeviceadministratorenrollment-action"></a><span data-ttu-id="8560f-103">действие Енаблеандроиддевицеадминистраторенроллмент</span><span class="sxs-lookup"><span data-stu-id="8560f-103">enableAndroidDeviceAdministratorEnrollment action</span></span>

> <span data-ttu-id="8560f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8560f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8560f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8560f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8560f-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8560f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8560f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8560f-107">Prerequisites</span></span>
<span data-ttu-id="8560f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8560f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8560f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8560f-110">Permission type</span></span>|<span data-ttu-id="8560f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8560f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8560f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8560f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8560f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8560f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8560f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8560f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8560f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8560f-115">Not supported.</span></span>|
|<span data-ttu-id="8560f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8560f-116">Application</span></span>|<span data-ttu-id="8560f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8560f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8560f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8560f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableAndroidDeviceAdministratorEnrollment
```

## <a name="request-headers"></a><span data-ttu-id="8560f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8560f-119">Request headers</span></span>
|<span data-ttu-id="8560f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8560f-120">Header</span></span>|<span data-ttu-id="8560f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8560f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8560f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8560f-122">Authorization</span></span>|<span data-ttu-id="8560f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8560f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8560f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8560f-124">Accept</span></span>|<span data-ttu-id="8560f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8560f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8560f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8560f-126">Request body</span></span>
<span data-ttu-id="8560f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8560f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8560f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8560f-128">Response</span></span>
<span data-ttu-id="8560f-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8560f-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8560f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8560f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8560f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8560f-131">Request</span></span>
<span data-ttu-id="8560f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8560f-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableAndroidDeviceAdministratorEnrollment
```

### <a name="response"></a><span data-ttu-id="8560f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8560f-133">Response</span></span>
<span data-ttu-id="8560f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8560f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




