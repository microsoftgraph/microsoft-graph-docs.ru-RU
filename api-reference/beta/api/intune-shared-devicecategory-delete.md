---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3f02bcad5c43ef787ad53ea59bb88853074db452
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161756"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="1aa5f-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1aa5f-103">Delete deviceCategory</span></span>

> <span data-ttu-id="1aa5f-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1aa5f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1aa5f-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aa5f-107">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1aa5f-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1aa5f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1aa5f-108">Prerequisites</span></span>
<span data-ttu-id="1aa5f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1aa5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="1aa5f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aa5f-111">Permission type</span></span>|<span data-ttu-id="1aa5f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aa5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aa5f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aa5f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1aa5f-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="1aa5f-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1aa5f-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aa5f-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1aa5f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aa5f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aa5f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-117">Not supported.</span></span>|
|<span data-ttu-id="1aa5f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aa5f-118">Application</span></span>|<span data-ttu-id="1aa5f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aa5f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aa5f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="1aa5f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aa5f-121">Request headers</span></span>
|<span data-ttu-id="1aa5f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1aa5f-122">Header</span></span>|<span data-ttu-id="1aa5f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1aa5f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aa5f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aa5f-124">Authorization</span></span>|<span data-ttu-id="1aa5f-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1aa5f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aa5f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1aa5f-126">Accept</span></span>|<span data-ttu-id="1aa5f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1aa5f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aa5f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1aa5f-128">Request body</span></span>
<span data-ttu-id="1aa5f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aa5f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aa5f-130">Response</span></span>
<span data-ttu-id="1aa5f-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1aa5f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1aa5f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1aa5f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aa5f-133">Request</span></span>

<span data-ttu-id="1aa5f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="1aa5f-135">Отклик
</span><span class="sxs-lookup"><span data-stu-id="1aa5f-135">Response</span></span>

<span data-ttu-id="1aa5f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1aa5f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



