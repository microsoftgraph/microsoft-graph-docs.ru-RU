---
title: Создание объекта mobileAppContent
description: Создание объекта mobileAppContent.
ms.openlocfilehash: 8aba68926a39a23e8adf0448679cb46ea4b79bb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028067"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="fd783-103">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="fd783-103">Create mobileAppContent</span></span>

> <span data-ttu-id="fd783-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd783-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd783-105">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="fd783-105">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd783-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd783-106">Prerequisites</span></span>
<span data-ttu-id="fd783-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd783-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd783-109">Permission type</span></span>|<span data-ttu-id="fd783-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd783-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd783-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd783-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd783-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd783-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd783-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd783-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd783-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd783-114">Not supported.</span></span>|
|<span data-ttu-id="fd783-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd783-115">Application</span></span>|<span data-ttu-id="fd783-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd783-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd783-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd783-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="fd783-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd783-118">Request headers</span></span>
|<span data-ttu-id="fd783-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd783-119">Header</span></span>|<span data-ttu-id="fd783-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fd783-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd783-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd783-121">Authorization</span></span>|<span data-ttu-id="fd783-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fd783-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd783-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fd783-123">Accept</span></span>|<span data-ttu-id="fd783-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd783-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd783-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd783-125">Request body</span></span>
<span data-ttu-id="fd783-126">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd783-126">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="fd783-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="fd783-127">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="fd783-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd783-128">Property</span></span>|<span data-ttu-id="fd783-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fd783-129">Type</span></span>|<span data-ttu-id="fd783-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fd783-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd783-131">id</span><span class="sxs-lookup"><span data-stu-id="fd783-131">id</span></span>|<span data-ttu-id="fd783-132">String</span><span class="sxs-lookup"><span data-stu-id="fd783-132">String</span></span>|<span data-ttu-id="fd783-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="fd783-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="fd783-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd783-134">Response</span></span>
<span data-ttu-id="fd783-135">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd783-135">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd783-136">Пример</span><span class="sxs-lookup"><span data-stu-id="fd783-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd783-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd783-137">Request</span></span>
<span data-ttu-id="fd783-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd783-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="fd783-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd783-139">Response</span></span>
<span data-ttu-id="fd783-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fd783-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



