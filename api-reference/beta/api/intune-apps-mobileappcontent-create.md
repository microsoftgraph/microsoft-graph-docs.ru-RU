---
title: Создание объекта mobileAppContent
description: Создание объекта mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82a8e0fdd96235f319685dec5223a358421ea8f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404745"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="4314b-103">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4314b-103">Create mobileAppContent</span></span>

> <span data-ttu-id="4314b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4314b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4314b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4314b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4314b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4314b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4314b-107">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="4314b-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4314b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4314b-108">Prerequisites</span></span>
<span data-ttu-id="4314b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4314b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4314b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4314b-111">Permission type</span></span>|<span data-ttu-id="4314b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4314b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4314b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4314b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4314b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4314b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4314b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4314b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4314b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4314b-116">Not supported.</span></span>|
|<span data-ttu-id="4314b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4314b-117">Application</span></span>|<span data-ttu-id="4314b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4314b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4314b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4314b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="4314b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4314b-120">Request headers</span></span>
|<span data-ttu-id="4314b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4314b-121">Header</span></span>|<span data-ttu-id="4314b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4314b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4314b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4314b-123">Authorization</span></span>|<span data-ttu-id="4314b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4314b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4314b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4314b-125">Accept</span></span>|<span data-ttu-id="4314b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4314b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4314b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4314b-127">Request body</span></span>
<span data-ttu-id="4314b-128">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4314b-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="4314b-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="4314b-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="4314b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4314b-130">Property</span></span>|<span data-ttu-id="4314b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4314b-131">Type</span></span>|<span data-ttu-id="4314b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4314b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4314b-133">id</span><span class="sxs-lookup"><span data-stu-id="4314b-133">id</span></span>|<span data-ttu-id="4314b-134">String</span><span class="sxs-lookup"><span data-stu-id="4314b-134">String</span></span>|<span data-ttu-id="4314b-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="4314b-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="4314b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4314b-136">Response</span></span>
<span data-ttu-id="4314b-137">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4314b-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4314b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="4314b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4314b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="4314b-139">Request</span></span>
<span data-ttu-id="4314b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4314b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="4314b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4314b-141">Response</span></span>
<span data-ttu-id="4314b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4314b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




