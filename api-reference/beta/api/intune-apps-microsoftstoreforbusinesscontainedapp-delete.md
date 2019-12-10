---
title: Удаление Микрософтсторефорбусинессконтаинедапп
description: Удаляет объект Микрософтсторефорбусинессконтаинедапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4ed4503151a921a9f8f46336c166eb9d4fab36d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936040"
---
# <a name="delete-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="4dbfc-103">Удаление Микрософтсторефорбусинессконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="4dbfc-103">Delete microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="4dbfc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dbfc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dbfc-106">Удаляет объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4dbfc-106">Deletes a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dbfc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4dbfc-107">Prerequisites</span></span>
<span data-ttu-id="4dbfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dbfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dbfc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dbfc-110">Permission type</span></span>|<span data-ttu-id="4dbfc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dbfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dbfc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dbfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dbfc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dbfc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4dbfc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dbfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dbfc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-115">Not supported.</span></span>|
|<span data-ttu-id="4dbfc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dbfc-116">Application</span></span>|<span data-ttu-id="4dbfc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dbfc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dbfc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dbfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="4dbfc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4dbfc-119">Request headers</span></span>
|<span data-ttu-id="4dbfc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dbfc-120">Header</span></span>|<span data-ttu-id="4dbfc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4dbfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dbfc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4dbfc-122">Authorization</span></span>|<span data-ttu-id="4dbfc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dbfc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4dbfc-124">Accept</span></span>|<span data-ttu-id="4dbfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dbfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dbfc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4dbfc-126">Request body</span></span>
<span data-ttu-id="4dbfc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dbfc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dbfc-128">Response</span></span>
<span data-ttu-id="4dbfc-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4dbfc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4dbfc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dbfc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dbfc-131">Request</span></span>
<span data-ttu-id="4dbfc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="4dbfc-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4dbfc-133">Response</span></span>
<span data-ttu-id="4dbfc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4dbfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





