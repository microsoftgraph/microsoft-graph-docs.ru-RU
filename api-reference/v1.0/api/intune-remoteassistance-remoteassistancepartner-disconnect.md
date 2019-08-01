---
title: Действие disconnect
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 84fae520e9e60f5227981aefbdb04820b38d71b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023596"
---
# <a name="disconnect-action"></a><span data-ttu-id="04650-103">Действие disconnect</span><span class="sxs-lookup"><span data-stu-id="04650-103">disconnect action</span></span>

> <span data-ttu-id="04650-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04650-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04650-105">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="04650-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04650-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04650-106">Prerequisites</span></span>
<span data-ttu-id="04650-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04650-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04650-109">Permission type</span></span>|<span data-ttu-id="04650-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04650-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04650-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04650-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04650-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04650-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04650-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04650-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04650-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04650-114">Not supported.</span></span>|
|<span data-ttu-id="04650-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04650-115">Application</span></span>|<span data-ttu-id="04650-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04650-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04650-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04650-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

## <a name="request-headers"></a><span data-ttu-id="04650-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04650-118">Request headers</span></span>
|<span data-ttu-id="04650-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04650-119">Header</span></span>|<span data-ttu-id="04650-120">Значение</span><span class="sxs-lookup"><span data-stu-id="04650-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04650-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04650-121">Authorization</span></span>|<span data-ttu-id="04650-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04650-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04650-123">Accept</span><span class="sxs-lookup"><span data-stu-id="04650-123">Accept</span></span>|<span data-ttu-id="04650-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04650-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04650-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04650-125">Request body</span></span>
<span data-ttu-id="04650-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04650-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04650-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="04650-127">Response</span></span>
<span data-ttu-id="04650-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04650-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04650-129">Пример</span><span class="sxs-lookup"><span data-stu-id="04650-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="04650-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="04650-130">Request</span></span>
<span data-ttu-id="04650-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04650-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/disconnect
```

### <a name="response"></a><span data-ttu-id="04650-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="04650-132">Response</span></span>
<span data-ttu-id="04650-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04650-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



