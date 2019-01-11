---
title: Обновление объекта mobileAppCategory
description: Обновление свойств объекта mobileAppCategory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bb21e4e3b564f50538f7399f8715c7f55a56b58b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869778"
---
# <a name="update-mobileappcategory"></a><span data-ttu-id="13474-103">Обновление объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="13474-103">Update mobileAppCategory</span></span>

> <span data-ttu-id="13474-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13474-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13474-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13474-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13474-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="13474-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13474-107">Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="13474-107">Update the properties of a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13474-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13474-108">Prerequisites</span></span>
<span data-ttu-id="13474-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13474-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13474-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13474-111">Permission type</span></span>|<span data-ttu-id="13474-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13474-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13474-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13474-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13474-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13474-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13474-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13474-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13474-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13474-116">Not supported.</span></span>|
|<span data-ttu-id="13474-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13474-117">Application</span></span>|<span data-ttu-id="13474-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13474-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13474-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13474-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/categories/{mobileAppCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="13474-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13474-120">Request headers</span></span>
|<span data-ttu-id="13474-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13474-121">Header</span></span>|<span data-ttu-id="13474-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13474-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13474-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13474-123">Authorization</span></span>|<span data-ttu-id="13474-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="13474-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13474-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13474-125">Accept</span></span>|<span data-ttu-id="13474-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13474-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13474-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13474-127">Request body</span></span>
<span data-ttu-id="13474-128">В тексте запроса добавьте представление объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13474-128">In the request body, supply a JSON representation for the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

<span data-ttu-id="13474-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="13474-129">The following table shows the properties that are required when you create the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span></span>

|<span data-ttu-id="13474-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13474-130">Property</span></span>|<span data-ttu-id="13474-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13474-131">Type</span></span>|<span data-ttu-id="13474-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13474-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13474-133">id</span><span class="sxs-lookup"><span data-stu-id="13474-133">id</span></span>|<span data-ttu-id="13474-134">String</span><span class="sxs-lookup"><span data-stu-id="13474-134">String</span></span>|<span data-ttu-id="13474-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13474-135">The key of the entity.</span></span>|
|<span data-ttu-id="13474-136">displayName</span><span class="sxs-lookup"><span data-stu-id="13474-136">displayName</span></span>|<span data-ttu-id="13474-137">String</span><span class="sxs-lookup"><span data-stu-id="13474-137">String</span></span>|<span data-ttu-id="13474-138">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="13474-138">The name of the app category.</span></span>|
|<span data-ttu-id="13474-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13474-139">lastModifiedDateTime</span></span>|<span data-ttu-id="13474-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13474-140">DateTimeOffset</span></span>|<span data-ttu-id="13474-141">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="13474-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="13474-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="13474-142">Response</span></span>
<span data-ttu-id="13474-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13474-143">If successful, this method returns a `200 OK` response code and an updated [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13474-144">Пример</span><span class="sxs-lookup"><span data-stu-id="13474-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="13474-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="13474-145">Request</span></span>
<span data-ttu-id="13474-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13474-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories/{mobileAppCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="13474-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="13474-147">Response</span></span>
<span data-ttu-id="13474-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="13474-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





