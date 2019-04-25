---
title: Действие targetApps
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: edafd2837cd0c8677ebd096f7ad50c4de1f1b8f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529760"
---
# <a name="targetapps-action"></a><span data-ttu-id="8390d-103">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="8390d-103">targetApps action</span></span>

> <span data-ttu-id="8390d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8390d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8390d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8390d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8390d-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8390d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8390d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8390d-107">Prerequisites</span></span>
<span data-ttu-id="8390d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8390d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8390d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8390d-110">Permission type</span></span>|<span data-ttu-id="8390d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8390d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8390d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8390d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8390d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8390d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8390d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8390d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8390d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8390d-115">Not supported.</span></span>|
|<span data-ttu-id="8390d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8390d-116">Application</span></span>|<span data-ttu-id="8390d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8390d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8390d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8390d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="8390d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8390d-119">Request headers</span></span>
|<span data-ttu-id="8390d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8390d-120">Header</span></span>|<span data-ttu-id="8390d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8390d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8390d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8390d-122">Authorization</span></span>|<span data-ttu-id="8390d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8390d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8390d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8390d-124">Accept</span></span>|<span data-ttu-id="8390d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8390d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8390d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8390d-126">Request body</span></span>
<span data-ttu-id="8390d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8390d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8390d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="8390d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8390d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8390d-129">Property</span></span>|<span data-ttu-id="8390d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8390d-130">Type</span></span>|<span data-ttu-id="8390d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8390d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8390d-132">apps</span><span class="sxs-lookup"><span data-stu-id="8390d-132">apps</span></span>|<span data-ttu-id="8390d-133">Коллекция [managedMobileApp](../resources/intune-mam-managedmobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8390d-133">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="8390d-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8390d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8390d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8390d-135">Response</span></span>
<span data-ttu-id="8390d-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8390d-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8390d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="8390d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="8390d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8390d-138">Request</span></span>
<span data-ttu-id="8390d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8390d-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8390d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8390d-140">Response</span></span>
<span data-ttu-id="8390d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8390d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





