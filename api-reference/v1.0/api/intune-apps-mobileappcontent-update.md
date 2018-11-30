---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
ms.openlocfilehash: f3e764866165c544fee7120978a0cef872f98d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025636"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="6f6f1-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6f6f1-103">Update mobileAppContent</span></span>

> <span data-ttu-id="6f6f1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f6f1-105">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="6f6f1-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f6f1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6f6f1-106">Prerequisites</span></span>
<span data-ttu-id="6f6f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6f1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6f1-109">Permission type</span></span>|<span data-ttu-id="6f6f1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f6f1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f6f1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f6f1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f6f1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6f1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6f6f1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f6f1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f6f1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-114">Not supported.</span></span>|
|<span data-ttu-id="6f6f1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f6f1-115">Application</span></span>|<span data-ttu-id="6f6f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f6f1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f6f1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="6f6f1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f6f1-118">Request headers</span></span>
|<span data-ttu-id="6f6f1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f6f1-119">Header</span></span>|<span data-ttu-id="6f6f1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6f6f1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f6f1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f6f1-121">Authorization</span></span>|<span data-ttu-id="6f6f1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f6f1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f6f1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6f6f1-123">Accept</span></span>|<span data-ttu-id="6f6f1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f6f1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6f1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f6f1-125">Request body</span></span>
<span data-ttu-id="6f6f1-126">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="6f6f1-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="6f6f1-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="6f6f1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f6f1-128">Property</span></span>|<span data-ttu-id="6f6f1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6f6f1-129">Type</span></span>|<span data-ttu-id="6f6f1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6f1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f6f1-131">id</span><span class="sxs-lookup"><span data-stu-id="6f6f1-131">id</span></span>|<span data-ttu-id="6f6f1-132">String</span><span class="sxs-lookup"><span data-stu-id="6f6f1-132">String</span></span>|<span data-ttu-id="6f6f1-133">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="6f6f1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6f1-134">Response</span></span>
<span data-ttu-id="6f6f1-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6f1-136">Пример</span><span class="sxs-lookup"><span data-stu-id="6f6f1-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f6f1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f6f1-137">Request</span></span>
<span data-ttu-id="6f6f1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f6f1-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="6f6f1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f6f1-139">Response</span></span>
<span data-ttu-id="6f6f1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6f6f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



