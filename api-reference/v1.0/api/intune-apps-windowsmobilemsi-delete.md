---
title: Delete windowsMobileMSI
description: Удаляет объект windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d14b1c01f0888a6c2f76f00d0fd7634460ee5dc3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580263"
---
# <a name="delete-windowsmobilemsi"></a><span data-ttu-id="d9ffb-103">Delete windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d9ffb-103">Delete windowsMobileMSI</span></span>

> <span data-ttu-id="d9ffb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9ffb-105">Удаляет объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="d9ffb-105">Deletes a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9ffb-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ffb-106">Prerequisites</span></span>
<span data-ttu-id="d9ffb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9ffb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ffb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ffb-109">Permission type</span></span>|<span data-ttu-id="d9ffb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9ffb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9ffb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9ffb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9ffb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9ffb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9ffb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9ffb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9ffb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-114">Not supported.</span></span>|
|<span data-ttu-id="d9ffb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9ffb-115">Application</span></span>|<span data-ttu-id="d9ffb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9ffb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9ffb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d9ffb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9ffb-118">Request headers</span></span>
|<span data-ttu-id="d9ffb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9ffb-119">Header</span></span>|<span data-ttu-id="d9ffb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d9ffb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9ffb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9ffb-121">Authorization</span></span>|<span data-ttu-id="d9ffb-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9ffb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d9ffb-123">Accept</span></span>|<span data-ttu-id="d9ffb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9ffb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9ffb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9ffb-125">Request body</span></span>
<span data-ttu-id="d9ffb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9ffb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9ffb-127">Response</span></span>
<span data-ttu-id="d9ffb-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d9ffb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d9ffb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9ffb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9ffb-130">Request</span></span>
<span data-ttu-id="d9ffb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d9ffb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9ffb-132">Response</span></span>
<span data-ttu-id="d9ffb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9ffb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



