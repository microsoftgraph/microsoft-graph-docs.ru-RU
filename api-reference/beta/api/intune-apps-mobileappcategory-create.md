---
title: Создание объекта mobileAppCategory
description: Создание объекта mobileAppCategory.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e88632627569af8a77ff60b11b7319b2acdaf430
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423862"
---
# <a name="create-mobileappcategory"></a><span data-ttu-id="c95c9-103">Создание объекта mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="c95c9-103">Create mobileAppCategory</span></span>

> <span data-ttu-id="c95c9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c95c9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c95c9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c95c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c95c9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c95c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c95c9-107">Создание объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c95c9-107">Create a new [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c95c9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c95c9-108">Prerequisites</span></span>
<span data-ttu-id="c95c9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c95c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c95c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c95c9-111">Permission type</span></span>|<span data-ttu-id="c95c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c95c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c95c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c95c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c95c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c95c9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c95c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c95c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c95c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c95c9-116">Not supported.</span></span>|
|<span data-ttu-id="c95c9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c95c9-117">Application</span></span>|<span data-ttu-id="c95c9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c95c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c95c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c95c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="c95c9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c95c9-120">Request headers</span></span>
|<span data-ttu-id="c95c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c95c9-121">Header</span></span>|<span data-ttu-id="c95c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c95c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c95c9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c95c9-123">Authorization</span></span>|<span data-ttu-id="c95c9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c95c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c95c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c95c9-125">Accept</span></span>|<span data-ttu-id="c95c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c95c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c95c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c95c9-127">Request body</span></span>
<span data-ttu-id="c95c9-128">В тексте запроса добавьте представление объекта mobileAppCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c95c9-128">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="c95c9-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="c95c9-129">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="c95c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c95c9-130">Property</span></span>|<span data-ttu-id="c95c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c95c9-131">Type</span></span>|<span data-ttu-id="c95c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c95c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c95c9-133">id</span><span class="sxs-lookup"><span data-stu-id="c95c9-133">id</span></span>|<span data-ttu-id="c95c9-134">String</span><span class="sxs-lookup"><span data-stu-id="c95c9-134">String</span></span>|<span data-ttu-id="c95c9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c95c9-135">The key of the entity.</span></span>|
|<span data-ttu-id="c95c9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c95c9-136">displayName</span></span>|<span data-ttu-id="c95c9-137">String</span><span class="sxs-lookup"><span data-stu-id="c95c9-137">String</span></span>|<span data-ttu-id="c95c9-138">Имя категории приложений.</span><span class="sxs-lookup"><span data-stu-id="c95c9-138">The name of the app category.</span></span>|
|<span data-ttu-id="c95c9-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c95c9-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c95c9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c95c9-140">DateTimeOffset</span></span>|<span data-ttu-id="c95c9-141">Дата и время последнего изменения объекта mobileAppCategory.</span><span class="sxs-lookup"><span data-stu-id="c95c9-141">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c95c9-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c95c9-142">Response</span></span>
<span data-ttu-id="c95c9-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c95c9-143">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c95c9-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c95c9-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c95c9-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c95c9-145">Request</span></span>
<span data-ttu-id="c95c9-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c95c9-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c95c9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c95c9-147">Response</span></span>
<span data-ttu-id="c95c9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c95c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




