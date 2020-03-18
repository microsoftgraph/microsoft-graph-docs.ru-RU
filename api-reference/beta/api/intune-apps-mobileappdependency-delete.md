---
title: Удаление Мобилеаппдепенденци
description: Удаляет объект Мобилеаппдепенденци.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0297f592beb66b77280b1a5e06db361c6e48266f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761267"
---
# <a name="delete-mobileappdependency"></a><span data-ttu-id="dc995-103">Удаление Мобилеаппдепенденци</span><span class="sxs-lookup"><span data-stu-id="dc995-103">Delete mobileAppDependency</span></span>

> <span data-ttu-id="dc995-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc995-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc995-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc995-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc995-106">Удаляет объект [мобилеаппдепенденци](../resources/intune-apps-mobileappdependency.md).</span><span class="sxs-lookup"><span data-stu-id="dc995-106">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc995-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dc995-107">Prerequisites</span></span>
<span data-ttu-id="dc995-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc995-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc995-110">Permission type</span></span>|<span data-ttu-id="dc995-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc995-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc995-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc995-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc995-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc995-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc995-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc995-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc995-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc995-115">Not supported.</span></span>|
|<span data-ttu-id="dc995-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc995-116">Application</span></span>|<span data-ttu-id="dc995-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc995-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc995-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc995-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="dc995-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc995-119">Request headers</span></span>
|<span data-ttu-id="dc995-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc995-120">Header</span></span>|<span data-ttu-id="dc995-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dc995-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc995-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc995-122">Authorization</span></span>|<span data-ttu-id="dc995-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc995-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc995-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dc995-124">Accept</span></span>|<span data-ttu-id="dc995-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc995-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc995-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc995-126">Request body</span></span>
<span data-ttu-id="dc995-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc995-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc995-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc995-128">Response</span></span>
<span data-ttu-id="dc995-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc995-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc995-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dc995-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc995-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc995-131">Request</span></span>
<span data-ttu-id="dc995-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc995-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="dc995-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc995-133">Response</span></span>
<span data-ttu-id="dc995-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc995-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




