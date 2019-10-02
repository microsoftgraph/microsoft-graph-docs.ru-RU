---
title: Действие disconnect
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd933189981b4a4c443cba1930aa4b4feb8ff222
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361639"
---
# <a name="disconnect-action"></a><span data-ttu-id="749aa-103">Действие disconnect</span><span class="sxs-lookup"><span data-stu-id="749aa-103">disconnect action</span></span>

> <span data-ttu-id="749aa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="749aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="749aa-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="749aa-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="749aa-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="749aa-106">Prerequisites</span></span>
<span data-ttu-id="749aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="749aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="749aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="749aa-109">Permission type</span></span>|<span data-ttu-id="749aa-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="749aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="749aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="749aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="749aa-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="749aa-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="749aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="749aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="749aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="749aa-114">Not supported.</span></span>|
|<span data-ttu-id="749aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="749aa-115">Application</span></span>|<span data-ttu-id="749aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="749aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="749aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="749aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

## <a name="request-headers"></a><span data-ttu-id="749aa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="749aa-118">Request headers</span></span>
|<span data-ttu-id="749aa-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="749aa-119">Header</span></span>|<span data-ttu-id="749aa-120">Значение</span><span class="sxs-lookup"><span data-stu-id="749aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="749aa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="749aa-121">Authorization</span></span>|<span data-ttu-id="749aa-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="749aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="749aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="749aa-123">Accept</span></span>|<span data-ttu-id="749aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="749aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="749aa-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="749aa-125">Request body</span></span>
<span data-ttu-id="749aa-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="749aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="749aa-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="749aa-127">Response</span></span>
<span data-ttu-id="749aa-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="749aa-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="749aa-129">Пример</span><span class="sxs-lookup"><span data-stu-id="749aa-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="749aa-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="749aa-130">Request</span></span>
<span data-ttu-id="749aa-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="749aa-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

### <a name="response"></a><span data-ttu-id="749aa-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="749aa-132">Response</span></span>
<span data-ttu-id="749aa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="749aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




