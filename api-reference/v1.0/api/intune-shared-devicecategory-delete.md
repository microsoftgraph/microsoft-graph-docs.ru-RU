---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35dffc1c280caeb10007dbf11d390ac7487d4a61
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249972"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="69285-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="69285-103">Delete deviceCategory</span></span>

> <span data-ttu-id="69285-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69285-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69285-105">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="69285-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69285-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="69285-106">Prerequisites</span></span>
<span data-ttu-id="69285-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69285-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69285-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69285-109">Permission type</span></span>|<span data-ttu-id="69285-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69285-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69285-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69285-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="69285-112">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="69285-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="69285-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69285-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69285-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69285-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69285-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69285-115">Not supported.</span></span>|
|<span data-ttu-id="69285-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69285-116">Application</span></span>|<span data-ttu-id="69285-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69285-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69285-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69285-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="69285-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69285-119">Request headers</span></span>
|<span data-ttu-id="69285-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69285-120">Header</span></span>|<span data-ttu-id="69285-121">Значение</span><span class="sxs-lookup"><span data-stu-id="69285-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69285-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69285-122">Authorization</span></span>|<span data-ttu-id="69285-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="69285-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69285-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69285-124">Accept</span></span>|<span data-ttu-id="69285-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69285-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69285-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69285-126">Request body</span></span>
<span data-ttu-id="69285-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69285-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69285-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="69285-128">Response</span></span>
<span data-ttu-id="69285-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69285-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="69285-130">Пример</span><span class="sxs-lookup"><span data-stu-id="69285-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="69285-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="69285-131">Request</span></span>
<span data-ttu-id="69285-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69285-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="69285-133">Отклик
</span><span class="sxs-lookup"><span data-stu-id="69285-133">Response</span></span>
<span data-ttu-id="69285-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="69285-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



