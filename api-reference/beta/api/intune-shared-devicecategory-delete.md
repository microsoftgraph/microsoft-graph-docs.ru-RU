---
title: Удаление deviceCategory
description: Удаление объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef1283329ac40356a4f81704b1969aebbb8b0dde
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571132"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="5c0be-103">Удаление deviceCategory</span><span class="sxs-lookup"><span data-stu-id="5c0be-103">Delete deviceCategory</span></span>

> <span data-ttu-id="5c0be-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c0be-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c0be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c0be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c0be-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c0be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c0be-107">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="5c0be-107">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c0be-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c0be-108">Prerequisites</span></span>
<span data-ttu-id="5c0be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c0be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c0be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c0be-111">Permission type</span></span>|<span data-ttu-id="5c0be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c0be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c0be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c0be-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5c0be-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="5c0be-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5c0be-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c0be-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5c0be-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c0be-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c0be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c0be-117">Not supported.</span></span>|
|<span data-ttu-id="5c0be-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c0be-118">Application</span></span>|<span data-ttu-id="5c0be-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c0be-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c0be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c0be-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="5c0be-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c0be-121">Request headers</span></span>
|<span data-ttu-id="5c0be-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c0be-122">Header</span></span>|<span data-ttu-id="5c0be-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5c0be-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c0be-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c0be-124">Authorization</span></span>|<span data-ttu-id="5c0be-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c0be-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c0be-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5c0be-126">Accept</span></span>|<span data-ttu-id="5c0be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5c0be-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c0be-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c0be-128">Request body</span></span>
<span data-ttu-id="5c0be-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c0be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c0be-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c0be-130">Response</span></span>
<span data-ttu-id="5c0be-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c0be-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5c0be-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5c0be-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c0be-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c0be-133">Request</span></span>

<span data-ttu-id="5c0be-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c0be-134">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="5c0be-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c0be-135">Response</span></span>

<span data-ttu-id="5c0be-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c0be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



