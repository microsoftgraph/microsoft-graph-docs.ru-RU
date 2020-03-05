---
title: Удаление Виндовсуниверсалаппксконтаинедапп
description: Удаляет объект Виндовсуниверсалаппксконтаинедапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10838f99ca8ca05dc0c8eceaf544d0105d5a7347
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450435"
---
# <a name="delete-windowsuniversalappxcontainedapp"></a><span data-ttu-id="f3965-103">Удаление Виндовсуниверсалаппксконтаинедапп</span><span class="sxs-lookup"><span data-stu-id="f3965-103">Delete windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="f3965-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f3965-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3965-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3965-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3965-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3965-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3965-107">Удаляет объект [виндовсуниверсалаппксконтаинедапп](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3965-107">Deletes a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3965-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3965-108">Prerequisites</span></span>
<span data-ttu-id="f3965-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3965-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3965-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3965-111">Permission type</span></span>|<span data-ttu-id="f3965-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3965-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3965-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3965-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3965-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3965-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3965-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3965-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3965-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3965-116">Not supported.</span></span>|
|<span data-ttu-id="f3965-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3965-117">Application</span></span>|<span data-ttu-id="f3965-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3965-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3965-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3965-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f3965-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3965-120">Request headers</span></span>
|<span data-ttu-id="f3965-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3965-121">Header</span></span>|<span data-ttu-id="f3965-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3965-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3965-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3965-123">Authorization</span></span>|<span data-ttu-id="f3965-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3965-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3965-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3965-125">Accept</span></span>|<span data-ttu-id="f3965-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3965-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3965-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3965-127">Request body</span></span>
<span data-ttu-id="f3965-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3965-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3965-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3965-129">Response</span></span>
<span data-ttu-id="f3965-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3965-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3965-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f3965-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3965-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3965-132">Request</span></span>
<span data-ttu-id="f3965-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3965-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
```

### <a name="response"></a><span data-ttu-id="f3965-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3965-134">Response</span></span>
<span data-ttu-id="f3965-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3965-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





