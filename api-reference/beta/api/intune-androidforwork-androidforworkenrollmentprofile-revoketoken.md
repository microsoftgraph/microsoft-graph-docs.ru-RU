---
title: Действие revokeToken
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd23bc1b7a09428e97d010341530f0b940246c2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446193"
---
# <a name="revoketoken-action"></a><span data-ttu-id="0c853-103">Действие revokeToken</span><span class="sxs-lookup"><span data-stu-id="0c853-103">revokeToken action</span></span>

<span data-ttu-id="0c853-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c853-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c853-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c853-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c853-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c853-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c853-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0c853-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c853-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0c853-108">Prerequisites</span></span>
<span data-ttu-id="0c853-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c853-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c853-111">Permission type</span></span>|<span data-ttu-id="0c853-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c853-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c853-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c853-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c853-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c853-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c853-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c853-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c853-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c853-116">Not supported.</span></span>|
|<span data-ttu-id="0c853-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c853-117">Application</span></span>|<span data-ttu-id="0c853-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c853-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c853-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c853-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/revokeToken
```

## <a name="request-headers"></a><span data-ttu-id="0c853-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c853-120">Request headers</span></span>
|<span data-ttu-id="0c853-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c853-121">Header</span></span>|<span data-ttu-id="0c853-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c853-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c853-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c853-123">Authorization</span></span>|<span data-ttu-id="0c853-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c853-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c853-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c853-125">Accept</span></span>|<span data-ttu-id="0c853-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c853-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c853-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c853-127">Request body</span></span>
<span data-ttu-id="0c853-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c853-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c853-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c853-129">Response</span></span>
<span data-ttu-id="0c853-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0c853-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0c853-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0c853-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c853-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c853-132">Request</span></span>
<span data-ttu-id="0c853-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c853-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/revokeToken
```

### <a name="response"></a><span data-ttu-id="0c853-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c853-134">Response</span></span>
<span data-ttu-id="0c853-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c853-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





