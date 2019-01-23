---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cff7aa7b7c290b37358cef413a0b17e54e91c83c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415707"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="c8140-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c8140-103">Delete deviceCategory</span></span>

> <span data-ttu-id="c8140-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8140-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8140-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8140-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8140-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8140-107">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="c8140-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8140-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8140-108">Prerequisites</span></span>
<span data-ttu-id="c8140-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8140-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8140-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8140-111">Permission type</span></span>|<span data-ttu-id="c8140-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8140-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8140-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c8140-114">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="c8140-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c8140-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8140-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8140-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8140-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8140-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8140-117">Not supported.</span></span>|
|<span data-ttu-id="c8140-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8140-118">Application</span></span>|<span data-ttu-id="c8140-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8140-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8140-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8140-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="c8140-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8140-121">Request headers</span></span>
|<span data-ttu-id="c8140-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8140-122">Header</span></span>|<span data-ttu-id="c8140-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c8140-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8140-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8140-124">Authorization</span></span>|<span data-ttu-id="c8140-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c8140-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8140-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c8140-126">Accept</span></span>|<span data-ttu-id="c8140-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c8140-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8140-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8140-128">Request body</span></span>
<span data-ttu-id="c8140-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8140-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8140-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8140-130">Response</span></span>
<span data-ttu-id="c8140-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c8140-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8140-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c8140-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8140-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8140-133">Request</span></span>

<span data-ttu-id="c8140-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8140-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="c8140-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8140-135">Response</span></span>

<span data-ttu-id="c8140-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8140-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



