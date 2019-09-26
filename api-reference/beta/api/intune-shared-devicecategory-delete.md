---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28bc560ca3d091b9c7b562d1414e0f1d510fff36
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194700"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="faab6-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="faab6-103">Delete deviceCategory</span></span>

> <span data-ttu-id="faab6-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="faab6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faab6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faab6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faab6-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faab6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faab6-107">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="faab6-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="faab6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="faab6-108">Prerequisites</span></span>
<span data-ttu-id="faab6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faab6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faab6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faab6-111">Permission type</span></span>|<span data-ttu-id="faab6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="faab6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faab6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faab6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="faab6-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="faab6-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="faab6-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab6-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="faab6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faab6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faab6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faab6-117">Not supported.</span></span>|
|<span data-ttu-id="faab6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faab6-118">Application</span></span>||
| <span data-ttu-id="faab6-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="faab6-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="faab6-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faab6-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="faab6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faab6-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="faab6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faab6-122">Request headers</span></span>
|<span data-ttu-id="faab6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faab6-123">Header</span></span>|<span data-ttu-id="faab6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="faab6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faab6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faab6-125">Authorization</span></span>|<span data-ttu-id="faab6-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faab6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faab6-127">Accept</span><span class="sxs-lookup"><span data-stu-id="faab6-127">Accept</span></span>|<span data-ttu-id="faab6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="faab6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faab6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="faab6-129">Request body</span></span>
<span data-ttu-id="faab6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="faab6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faab6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="faab6-131">Response</span></span>
<span data-ttu-id="faab6-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="faab6-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="faab6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="faab6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="faab6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="faab6-134">Request</span></span>

<span data-ttu-id="faab6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="faab6-135">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="faab6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="faab6-136">Response</span></span>

<span data-ttu-id="faab6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="faab6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```







