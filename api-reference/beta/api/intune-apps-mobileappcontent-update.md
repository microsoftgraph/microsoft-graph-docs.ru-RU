---
title: Обновление объекта mobileAppContent
description: Обновление свойств объекта mobileAppContent.
author: tfitzmac
ms.openlocfilehash: 478c01624c7b8bf42b71fa8224b31b38e8f0ae58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310516"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="086f1-103">Обновление объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="086f1-103">Update mobileAppContent</span></span>

> <span data-ttu-id="086f1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="086f1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="086f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="086f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="086f1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="086f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="086f1-107">Обновление свойств объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="086f1-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="086f1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="086f1-108">Prerequisites</span></span>
<span data-ttu-id="086f1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="086f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="086f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="086f1-111">Permission type</span></span>|<span data-ttu-id="086f1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="086f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="086f1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="086f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="086f1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="086f1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="086f1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="086f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="086f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="086f1-116">Not supported.</span></span>|
|<span data-ttu-id="086f1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="086f1-117">Application</span></span>|<span data-ttu-id="086f1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="086f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="086f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="086f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="086f1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="086f1-120">Request headers</span></span>
|<span data-ttu-id="086f1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="086f1-121">Header</span></span>|<span data-ttu-id="086f1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="086f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="086f1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="086f1-123">Authorization</span></span>|<span data-ttu-id="086f1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="086f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="086f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="086f1-125">Accept</span></span>|<span data-ttu-id="086f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="086f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="086f1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="086f1-127">Request body</span></span>
<span data-ttu-id="086f1-128">В тексте запроса добавьте представление объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="086f1-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="086f1-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="086f1-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="086f1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="086f1-130">Property</span></span>|<span data-ttu-id="086f1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="086f1-131">Type</span></span>|<span data-ttu-id="086f1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="086f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="086f1-133">id</span><span class="sxs-lookup"><span data-stu-id="086f1-133">id</span></span>|<span data-ttu-id="086f1-134">String</span><span class="sxs-lookup"><span data-stu-id="086f1-134">String</span></span>|<span data-ttu-id="086f1-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="086f1-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="086f1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="086f1-136">Response</span></span>
<span data-ttu-id="086f1-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="086f1-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="086f1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="086f1-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="086f1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="086f1-139">Request</span></span>
<span data-ttu-id="086f1-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="086f1-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="086f1-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="086f1-141">Response</span></span>
<span data-ttu-id="086f1-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="086f1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





