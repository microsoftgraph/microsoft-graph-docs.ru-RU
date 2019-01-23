---
title: Действие targetApps
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f671b7b5e2998aee9c0a53159def5c4766b3f58e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403415"
---
# <a name="targetapps-action"></a><span data-ttu-id="de2c7-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="de2c7-103">targetApps action</span></span>

> <span data-ttu-id="de2c7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de2c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="de2c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de2c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de2c7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de2c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2c7-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="de2c7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de2c7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="de2c7-108">Prerequisites</span></span>
<span data-ttu-id="de2c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="de2c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="de2c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de2c7-111">Permission type</span></span>|<span data-ttu-id="de2c7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de2c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de2c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de2c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de2c7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2c7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de2c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de2c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de2c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de2c7-116">Not supported.</span></span>|
|<span data-ttu-id="de2c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de2c7-117">Application</span></span>|<span data-ttu-id="de2c7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de2c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de2c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de2c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="de2c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de2c7-120">Request headers</span></span>
|<span data-ttu-id="de2c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de2c7-121">Header</span></span>|<span data-ttu-id="de2c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de2c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de2c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de2c7-123">Authorization</span></span>|<span data-ttu-id="de2c7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="de2c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de2c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de2c7-125">Accept</span></span>|<span data-ttu-id="de2c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de2c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de2c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de2c7-127">Request body</span></span>
<span data-ttu-id="de2c7-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de2c7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="de2c7-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="de2c7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="de2c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de2c7-130">Property</span></span>|<span data-ttu-id="de2c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de2c7-131">Type</span></span>|<span data-ttu-id="de2c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de2c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2c7-133">apps</span><span class="sxs-lookup"><span data-stu-id="de2c7-133">apps</span></span>|<span data-ttu-id="de2c7-134">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="de2c7-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="de2c7-135">Пока нет описания</span><span class="sxs-lookup"><span data-stu-id="de2c7-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="de2c7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="de2c7-136">Response</span></span>
<span data-ttu-id="de2c7-137">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de2c7-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="de2c7-138">Пример</span><span class="sxs-lookup"><span data-stu-id="de2c7-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="de2c7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="de2c7-139">Request</span></span>
<span data-ttu-id="de2c7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de2c7-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

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

### <a name="response"></a><span data-ttu-id="de2c7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="de2c7-141">Response</span></span>
<span data-ttu-id="de2c7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="de2c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




