---
title: Удаление mobileAppInstallStatus
description: Удаляет объект mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d777dc972740324931141f9ac3402a59b900658
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972545"
---
# <a name="delete-mobileappinstallstatus"></a><span data-ttu-id="970af-103">Удаление mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="970af-103">Delete mobileAppInstallStatus</span></span>

> <span data-ttu-id="970af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="970af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="970af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="970af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="970af-106">Удаляет объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="970af-106">Deletes a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="970af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="970af-107">Prerequisites</span></span>
<span data-ttu-id="970af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="970af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="970af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="970af-110">Permission type</span></span>|<span data-ttu-id="970af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="970af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="970af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="970af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="970af-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="970af-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="970af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="970af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="970af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="970af-115">Not supported.</span></span>|
|<span data-ttu-id="970af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="970af-116">Application</span></span>|<span data-ttu-id="970af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="970af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="970af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="970af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="970af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="970af-119">Request headers</span></span>
|<span data-ttu-id="970af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="970af-120">Header</span></span>|<span data-ttu-id="970af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="970af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="970af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="970af-122">Authorization</span></span>|<span data-ttu-id="970af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="970af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="970af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="970af-124">Accept</span></span>|<span data-ttu-id="970af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="970af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="970af-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="970af-126">Request body</span></span>
<span data-ttu-id="970af-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="970af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="970af-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="970af-128">Response</span></span>
<span data-ttu-id="970af-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="970af-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="970af-130">Пример</span><span class="sxs-lookup"><span data-stu-id="970af-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="970af-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="970af-131">Request</span></span>
<span data-ttu-id="970af-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="970af-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="970af-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="970af-133">Response</span></span>
<span data-ttu-id="970af-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="970af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




