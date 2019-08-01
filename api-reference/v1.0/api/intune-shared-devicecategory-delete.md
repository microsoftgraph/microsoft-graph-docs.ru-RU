---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e242cc2e3e1992d37053b71d864207a94b2bf4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025930"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="61baf-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="61baf-103">Delete deviceCategory</span></span>

> <span data-ttu-id="61baf-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61baf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61baf-105">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="61baf-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61baf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="61baf-106">Prerequisites</span></span>
<span data-ttu-id="61baf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61baf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61baf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61baf-109">Permission type</span></span>|<span data-ttu-id="61baf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61baf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61baf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61baf-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="61baf-112">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="61baf-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="61baf-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61baf-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61baf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61baf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61baf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61baf-115">Not supported.</span></span>|
|<span data-ttu-id="61baf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61baf-116">Application</span></span>|<span data-ttu-id="61baf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61baf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61baf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61baf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="61baf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61baf-119">Request headers</span></span>
|<span data-ttu-id="61baf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61baf-120">Header</span></span>|<span data-ttu-id="61baf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="61baf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61baf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61baf-122">Authorization</span></span>|<span data-ttu-id="61baf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61baf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61baf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="61baf-124">Accept</span></span>|<span data-ttu-id="61baf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61baf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61baf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="61baf-126">Request body</span></span>
<span data-ttu-id="61baf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61baf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61baf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="61baf-128">Response</span></span>
<span data-ttu-id="61baf-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="61baf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61baf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="61baf-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="61baf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="61baf-131">Request</span></span>
<span data-ttu-id="61baf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61baf-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="61baf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="61baf-133">Response</span></span>
<span data-ttu-id="61baf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61baf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



