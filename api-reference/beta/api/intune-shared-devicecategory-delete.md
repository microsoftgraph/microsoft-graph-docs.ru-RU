---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b9630b5f3b86ec22a4a1be735fde91d14550fc1e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853398"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="5cac3-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5cac3-103">Delete deviceCategory</span></span>

> <span data-ttu-id="5cac3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5cac3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cac3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cac3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cac3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5cac3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cac3-107">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5cac3-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5cac3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5cac3-108">Prerequisites</span></span>
<span data-ttu-id="5cac3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cac3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cac3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cac3-111">Permission type</span></span>|<span data-ttu-id="5cac3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cac3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cac3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cac3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5cac3-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="5cac3-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5cac3-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cac3-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5cac3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cac3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cac3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cac3-117">Not supported.</span></span>|
|<span data-ttu-id="5cac3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cac3-118">Application</span></span>|<span data-ttu-id="5cac3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cac3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cac3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cac3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5cac3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cac3-121">Request headers</span></span>
|<span data-ttu-id="5cac3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cac3-122">Header</span></span>|<span data-ttu-id="5cac3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5cac3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cac3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cac3-124">Authorization</span></span>|<span data-ttu-id="5cac3-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5cac3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cac3-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5cac3-126">Accept</span></span>|<span data-ttu-id="5cac3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5cac3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cac3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5cac3-128">Request body</span></span>
<span data-ttu-id="5cac3-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5cac3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cac3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cac3-130">Response</span></span>
<span data-ttu-id="5cac3-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5cac3-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5cac3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5cac3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cac3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cac3-133">Request</span></span>

<span data-ttu-id="5cac3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cac3-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="5cac3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cac3-135">Response</span></span>

<span data-ttu-id="5cac3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5cac3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



