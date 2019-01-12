---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 121ab846c29daf1eaf3c5b20cde8dbefc403e260
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941578"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="12fae-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="12fae-103">Delete deviceCategory</span></span>

> <span data-ttu-id="12fae-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12fae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12fae-105">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="12fae-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12fae-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12fae-106">Prerequisites</span></span>
<span data-ttu-id="12fae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fae-109">Permission type</span></span>|<span data-ttu-id="12fae-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fae-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="12fae-112">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="12fae-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="12fae-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fae-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12fae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fae-115">Not supported.</span></span>|
|<span data-ttu-id="12fae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fae-116">Application</span></span>|<span data-ttu-id="12fae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="12fae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12fae-119">Request headers</span></span>
|<span data-ttu-id="12fae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12fae-120">Header</span></span>|<span data-ttu-id="12fae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="12fae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12fae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12fae-122">Authorization</span></span>|<span data-ttu-id="12fae-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12fae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12fae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12fae-124">Accept</span></span>|<span data-ttu-id="12fae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12fae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fae-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12fae-126">Request body</span></span>
<span data-ttu-id="12fae-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12fae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12fae-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="12fae-128">Response</span></span>
<span data-ttu-id="12fae-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="12fae-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="12fae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="12fae-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="12fae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fae-131">Request</span></span>
<span data-ttu-id="12fae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fae-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="12fae-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="12fae-133">Response</span></span>
<span data-ttu-id="12fae-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12fae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



