---
title: Удаление Виндовсмикрософтеджеапп
description: Удаляет объект Виндовсмикрософтеджеапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d3ef4a0b5ff8a0e60a825969d3b5c0f8c14593c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247015"
---
# <a name="delete-windowsmicrosoftedgeapp"></a><span data-ttu-id="26e96-103">Удаление Виндовсмикрософтеджеапп</span><span class="sxs-lookup"><span data-stu-id="26e96-103">Delete windowsMicrosoftEdgeApp</span></span>

<span data-ttu-id="26e96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26e96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26e96-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26e96-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26e96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e96-107">Удаляет объект [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span><span class="sxs-lookup"><span data-stu-id="26e96-107">Deletes a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26e96-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="26e96-108">Prerequisites</span></span>
<span data-ttu-id="26e96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e96-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e96-111">Permission type</span></span>|<span data-ttu-id="26e96-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e96-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26e96-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e96-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26e96-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e96-116">Not supported.</span></span>|
|<span data-ttu-id="26e96-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="26e96-117">Application</span></span>|<span data-ttu-id="26e96-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e96-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e96-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="26e96-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="26e96-120">Request headers</span></span>
|<span data-ttu-id="26e96-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26e96-121">Header</span></span>|<span data-ttu-id="26e96-122">Значение</span><span class="sxs-lookup"><span data-stu-id="26e96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26e96-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26e96-123">Authorization</span></span>|<span data-ttu-id="26e96-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26e96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26e96-125">Accept</span></span>|<span data-ttu-id="26e96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26e96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e96-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26e96-127">Request body</span></span>
<span data-ttu-id="26e96-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26e96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26e96-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e96-129">Response</span></span>
<span data-ttu-id="26e96-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26e96-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="26e96-131">Пример</span><span class="sxs-lookup"><span data-stu-id="26e96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="26e96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e96-132">Request</span></span>
<span data-ttu-id="26e96-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e96-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="26e96-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e96-134">Response</span></span>
<span data-ttu-id="26e96-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26e96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




