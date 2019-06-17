---
title: Удаление windowsPhone81AppXBundle
description: Удаляет объект windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15b55d31aa880dcb90640ccc5eabc89ddd128acb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973028"
---
# <a name="delete-windowsphone81appxbundle"></a><span data-ttu-id="8d7c5-103">Удаление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="8d7c5-103">Delete windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="8d7c5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d7c5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d7c5-106">Удаляет объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="8d7c5-106">Deletes a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d7c5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d7c5-107">Prerequisites</span></span>
<span data-ttu-id="8d7c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d7c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d7c5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d7c5-110">Permission type</span></span>|<span data-ttu-id="8d7c5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d7c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d7c5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d7c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d7c5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d7c5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d7c5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d7c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d7c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-115">Not supported.</span></span>|
|<span data-ttu-id="8d7c5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d7c5-116">Application</span></span>|<span data-ttu-id="8d7c5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d7c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d7c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8d7c5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d7c5-119">Request headers</span></span>
|<span data-ttu-id="8d7c5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d7c5-120">Header</span></span>|<span data-ttu-id="8d7c5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d7c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d7c5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d7c5-122">Authorization</span></span>|<span data-ttu-id="8d7c5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d7c5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d7c5-124">Accept</span></span>|<span data-ttu-id="8d7c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d7c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d7c5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d7c5-126">Request body</span></span>
<span data-ttu-id="8d7c5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d7c5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d7c5-128">Response</span></span>
<span data-ttu-id="8d7c5-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d7c5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8d7c5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d7c5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d7c5-131">Request</span></span>
<span data-ttu-id="8d7c5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="8d7c5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d7c5-133">Response</span></span>
<span data-ttu-id="8d7c5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d7c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





