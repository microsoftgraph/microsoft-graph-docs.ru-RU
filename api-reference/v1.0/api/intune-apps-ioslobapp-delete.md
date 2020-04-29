---
title: Удаление объекта iosLobApp
description: Удаляет объект iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6207ef40ec2c0af75e472a37aac7859f1b3ab05
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446542"
---
# <a name="delete-ioslobapp"></a><span data-ttu-id="053ae-103">Удаление объекта iosLobApp</span><span class="sxs-lookup"><span data-stu-id="053ae-103">Delete iosLobApp</span></span>

<span data-ttu-id="053ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="053ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="053ae-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="053ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="053ae-106">Удаляет объект [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="053ae-106">Deletes a [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="053ae-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="053ae-107">Prerequisites</span></span>
<span data-ttu-id="053ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="053ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="053ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="053ae-110">Permission type</span></span>|<span data-ttu-id="053ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="053ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="053ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="053ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="053ae-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053ae-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="053ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="053ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="053ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="053ae-115">Not supported.</span></span>|
|<span data-ttu-id="053ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="053ae-116">Application</span></span>|<span data-ttu-id="053ae-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="053ae-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="053ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="053ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="053ae-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="053ae-119">Request headers</span></span>
|<span data-ttu-id="053ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="053ae-120">Header</span></span>|<span data-ttu-id="053ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="053ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="053ae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="053ae-122">Authorization</span></span>|<span data-ttu-id="053ae-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="053ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="053ae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="053ae-124">Accept</span></span>|<span data-ttu-id="053ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="053ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="053ae-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="053ae-126">Request body</span></span>
<span data-ttu-id="053ae-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="053ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="053ae-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="053ae-128">Response</span></span>
<span data-ttu-id="053ae-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="053ae-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="053ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="053ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="053ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="053ae-131">Request</span></span>
<span data-ttu-id="053ae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="053ae-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="053ae-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="053ae-133">Response</span></span>
<span data-ttu-id="053ae-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="053ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






