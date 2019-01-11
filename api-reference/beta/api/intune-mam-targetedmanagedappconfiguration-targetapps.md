---
title: Действие targetApps
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 957a1003554299e3dec52b05838fe58e0b2eea4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882070"
---
# <a name="targetapps-action"></a><span data-ttu-id="d118b-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="d118b-103">targetApps action</span></span>

> <span data-ttu-id="d118b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d118b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d118b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d118b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d118b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d118b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d118b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d118b-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d118b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d118b-108">Prerequisites</span></span>
<span data-ttu-id="d118b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d118b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d118b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d118b-111">Permission type</span></span>|<span data-ttu-id="d118b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d118b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d118b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d118b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d118b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d118b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d118b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d118b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d118b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d118b-116">Not supported.</span></span>|
|<span data-ttu-id="d118b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d118b-117">Application</span></span>|<span data-ttu-id="d118b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d118b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d118b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d118b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="d118b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d118b-120">Request headers</span></span>
|<span data-ttu-id="d118b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d118b-121">Header</span></span>|<span data-ttu-id="d118b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d118b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d118b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d118b-123">Authorization</span></span>|<span data-ttu-id="d118b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d118b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d118b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d118b-125">Accept</span></span>|<span data-ttu-id="d118b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d118b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d118b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d118b-127">Request body</span></span>
<span data-ttu-id="d118b-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d118b-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d118b-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d118b-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d118b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d118b-130">Property</span></span>|<span data-ttu-id="d118b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d118b-131">Type</span></span>|<span data-ttu-id="d118b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d118b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d118b-133">apps</span><span class="sxs-lookup"><span data-stu-id="d118b-133">apps</span></span>|<span data-ttu-id="d118b-134">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d118b-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="d118b-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="d118b-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d118b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d118b-136">Response</span></span>
<span data-ttu-id="d118b-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d118b-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d118b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d118b-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="d118b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d118b-139">Request</span></span>
<span data-ttu-id="d118b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d118b-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d118b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="d118b-141">Response</span></span>
<span data-ttu-id="d118b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d118b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





