---
title: Создание объекта mobileAppContent
description: Создание объекта mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8904626782e6df7a0fd6f367f0e0878328a07faf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921894"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="1547a-103">Создание объекта mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="1547a-103">Create mobileAppContent</span></span>

> <span data-ttu-id="1547a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1547a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1547a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1547a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1547a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1547a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1547a-107">Создание объекта [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="1547a-107">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1547a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1547a-108">Prerequisites</span></span>
<span data-ttu-id="1547a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1547a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1547a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1547a-111">Permission type</span></span>|<span data-ttu-id="1547a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1547a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1547a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1547a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1547a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1547a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1547a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1547a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1547a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1547a-116">Not supported.</span></span>|
|<span data-ttu-id="1547a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1547a-117">Application</span></span>|<span data-ttu-id="1547a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1547a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1547a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1547a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="1547a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1547a-120">Request headers</span></span>
|<span data-ttu-id="1547a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1547a-121">Header</span></span>|<span data-ttu-id="1547a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1547a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1547a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1547a-123">Authorization</span></span>|<span data-ttu-id="1547a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1547a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1547a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1547a-125">Accept</span></span>|<span data-ttu-id="1547a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1547a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1547a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1547a-127">Request body</span></span>
<span data-ttu-id="1547a-128">В тексте запроса добавьте представление объекта mobileAppContent в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1547a-128">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="1547a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="1547a-129">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="1547a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1547a-130">Property</span></span>|<span data-ttu-id="1547a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1547a-131">Type</span></span>|<span data-ttu-id="1547a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1547a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1547a-133">id</span><span class="sxs-lookup"><span data-stu-id="1547a-133">id</span></span>|<span data-ttu-id="1547a-134">String</span><span class="sxs-lookup"><span data-stu-id="1547a-134">String</span></span>|<span data-ttu-id="1547a-135">Версия контента приложения.</span><span class="sxs-lookup"><span data-stu-id="1547a-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="1547a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1547a-136">Response</span></span>
<span data-ttu-id="1547a-137">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1547a-137">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1547a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="1547a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="1547a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1547a-139">Request</span></span>
<span data-ttu-id="1547a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1547a-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="1547a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="1547a-141">Response</span></span>
<span data-ttu-id="1547a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1547a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





