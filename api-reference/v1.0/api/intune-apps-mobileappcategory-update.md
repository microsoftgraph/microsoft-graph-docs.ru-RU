---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
ms.openlocfilehash: dee39cf60590f18547d54ea07f96fd7c194a631c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025534"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="58b6d-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="58b6d-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="58b6d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="58b6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58b6d-105">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="58b6d-105">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58b6d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58b6d-106">Prerequisites</span></span>
<span data-ttu-id="58b6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58b6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58b6d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58b6d-109">Permission type</span></span>|<span data-ttu-id="58b6d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58b6d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58b6d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58b6d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58b6d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58b6d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58b6d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58b6d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58b6d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58b6d-114">Not supported.</span></span>|
|<span data-ttu-id="58b6d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58b6d-115">Application</span></span>|<span data-ttu-id="58b6d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58b6d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58b6d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58b6d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="58b6d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58b6d-118">Request headers</span></span>
|<span data-ttu-id="58b6d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58b6d-119">Header</span></span>|<span data-ttu-id="58b6d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="58b6d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58b6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58b6d-121">Authorization</span></span>|<span data-ttu-id="58b6d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="58b6d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58b6d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="58b6d-123">Accept</span></span>|<span data-ttu-id="58b6d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58b6d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58b6d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58b6d-125">Request body</span></span>
<span data-ttu-id="58b6d-126">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58b6d-126">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="58b6d-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="58b6d-127">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="58b6d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="58b6d-128">Property</span></span>|<span data-ttu-id="58b6d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="58b6d-129">Type</span></span>|<span data-ttu-id="58b6d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="58b6d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b6d-131">id</span><span class="sxs-lookup"><span data-stu-id="58b6d-131">id</span></span>|<span data-ttu-id="58b6d-132">String</span><span class="sxs-lookup"><span data-stu-id="58b6d-132">String</span></span>|<span data-ttu-id="58b6d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58b6d-133">The key of the entity.</span></span>|
|<span data-ttu-id="58b6d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="58b6d-134">displayName</span></span>|<span data-ttu-id="58b6d-135">String</span><span class="sxs-lookup"><span data-stu-id="58b6d-135">String</span></span>|<span data-ttu-id="58b6d-136">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="58b6d-136">The name of the app category.</span></span>|
|<span data-ttu-id="58b6d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58b6d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="58b6d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b6d-138">DateTimeOffset</span></span>|<span data-ttu-id="58b6d-139">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="58b6d-139">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="58b6d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="58b6d-140">Response</span></span>
<span data-ttu-id="58b6d-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58b6d-141">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58b6d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="58b6d-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="58b6d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="58b6d-143">Request</span></span>
<span data-ttu-id="58b6d-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58b6d-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="58b6d-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="58b6d-145">Response</span></span>
<span data-ttu-id="58b6d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="58b6d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



